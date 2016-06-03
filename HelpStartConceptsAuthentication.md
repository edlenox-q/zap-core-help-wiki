# Authentication #

ZAP handles multiple types of authentication (called **Authentication Methods**) that can be used for websites / webapps. Each **[Context][]** has an Authentication Method defined which dictates how authentication is handled. The authentication is used to create Web Sessions that correspond to authenticated webapp [Users][].

In order to detect when response messages from web servers correspond to authenticated requests, a set of indicators can be configured. The **Logged in indicator**, when present in a response message (either the header or the body), signifies that the response message corresponds to an authenticated request (e.g. presence of a 'logout link' or a 'Welcome back, User X' pattern). Similarly, the **Logged out indicator** indicates an unauthenticated request (e.g. presence of a 'login link'). Only the presence of one of the 2 indicators is sufficient for proper functionality. In the case neither of the indicators has been specified, all messages are considered, by default, authenticated.

To set one of the **Logged in/out Indicators**, either type the regex directly in the *[Session Properties][] dialog -> Authentication panel -> Logged In/Out Indicator field*, either find an authenticated message in the Sites Tree, select it, open the Response View and select the text you wish to define as the indicator using the mouse and select the *Flag as Context... Logged in/out indicator* right-click menu option.

In order to perform the authentication of a user on a website / in a webapp, the Authentication Method defines how the authentication is done (the process), while the necessary credentials (the exact identifiers) are dependent on the user, so, in ZAP, they are configured in the Users.

The generic **main steps** that are needed to configure authentication for a web application are the following:

1.  properly configure a ZAP [Context][] for the web application
2.  set up the [session management method][] for the context to the one that is used in your app
3.  set up the authentication method for the context:
    
    1.  set up at least one of the *Logged In Indicator* or the *Logged out indicator*, as described above
    2.  configure the authentication method for your application, specifying all the requirements (as seen below)
4.  configure a set of [users][Users] for the context that directly correspond to the authentication method for the context

Authentication methods can be used in multiple places around ZAP. Some of the examples include:

 *  defining Users and automatic login
 *  detection of authenticated/unauthenticated states
 *  performing automatic re-authentication

Multiple authentication methods have been implemented and the system supports easy addition of new methods, according to user needs. They main ones are described below.

### Manual Authentication ###

This method allows users to perform the authentication manually (e.g. authenticate in the browser while proxy-ing through ZAP) and then select the corresponding HTTP session. As the actual authentication is being performed by you, this method does not support re-authentication in case the webapp logs a user out.

When using this authentication method, configuring a User for the context require choosing an authenticated HTTP session.

### Form-Based Authentication ###

This method is used for websites / webapps where authentication is done by submitting a form or performing a GET request to a 'login url' using a 'username/password' pair of authentication credentials. Re-authentication is possible. Configuration can be done using the [Session Contexts Dialog][Session Properties] or using the contextual PopupMenu: *Flag as... Form-Based Authentication Login Request*.

When using this authentication method, configuring a User for the context requires setting up the *username/password* pair of credentials that are used for the form based authentication.

### HTTP/NTLM Authentication ###

This method is used for websites / webapps where authentication is enforced using the HTTP or NTLM Authentication mechanisms employing HTTP message headers. Three authentication schemes are supported: Basic, Digest and NTLM. Re-authentication is possible, as the authentication headers are sent with every authenticated request. Configuration can be done using the [Session Contexts Dialog][Session Properties].

When using this authentication method, configuring a User for the context requires setting up the *username/password* pair of credentials that are used for the HTTP/NTLM authentication.

### Script-Based Authentication ###

This method is useful for websites / webapps where the authentication is a more complex one and some custom scripts that handle the authentication process are beneficial. To use this method, you must first define an Authentication script which sends messages or performs other actions as needed by your web-application. This script is then selected for use for a given Context and it is called whenever an authentication is performed. Re-authentication is possible. Configuration can be done using the [Session Contexts Dialog][Session Properties] and requires you to have the Scripts Console ZAP Addon installed from the Marketplace.

When using this authentication method, configuring a User for the context requires setting up the a set of parameters defined in the script. For more details, see the provided Authentication Script examples.

## Configuration example ##

A configuration example showing how to fully configure a webapp that uses *form-based authentication* and *cookie-based session management* is seen below:

1.  set up a context for the web application
2.  set up the session management method to *Cookie-based Session Management*
3.  make sure your browser proxies everything through ZAP and log into your application using the browser
4.  go to ZAP and identify the request that was done for the login (most usually it's a HTTP POST request containing the username and the password and possibly other elements)
5.  right click on the request and Flag as Context... Form-based Auth Login Request
6.  a window will be opened already containing the request URL and the parameters (if any). Use the dropdown options to select which of the parameters correspond to the username and to the password
7.  then you need to tell ZAP how to identify whether an authentication succeeded or not. You can do this by setting logged in or logged indicators. These are regex patterns which, if found in a response, tell ZAP whether it's authenticated or not (e.g. presence of a http://example.com/logout link or the presence of a 'Welcome, User X'). Only one of them is necessary. To set one of them, either type the regex directly in the Session Properties -> Authentication -> Logged In Indicator, either find an authenticated message in the Sites Tree, select it, open the Response View and select the text you wish to define as the indicator using the mouse and select the Flag as Context... Logged in indicator right-click menu option.
8.  define as many users as you need in the Session Properties -> Users section.
9.  after this step, various actions are available in ZAP. For example, you now have a new right click option: Attack -> Spider Context As User. Or, using the Forced User Mode, you can force all the interactions that go through ZAP for a given Context to be from the perspective of a User. The User Forced Mode is enabled via the previous-to-last button in the toolbar (the one with the user and the lock) and is configured via Session Properties -> Forced User Mode.

Most of the steps above apply as well for other authentication methods. The only things that change when trying to configure authentication using a different method are steps 3, 4, 5 and 6. Instead of these, select the authentication method required from the drop-down list and configure it as needed. More details about configuring each type of authentication can be above and [here][].

## Configured via ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsSessionContexts#auth" rel="nofollow">Session Properties dialog</a></td> 
   <td></td> 
  </tr> 
 </tbody>
</table>

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="http://youtu.be/cR4gw-cPZOA" rel="nofollow">Youtube tutorial</a></td> 
   <td>of the Authentication, Session Management and Users Management features of ZAP [external link to http://youtu.be/cR4gw-cPZOA].</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td> 
   <td>for an overview of the user interface</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td> 
   <td>provided by ZAP</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsSessionContexts" rel="nofollow">Session Contexts Dialog</a></td> 
   <td>for an overview of the Session Properties</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpStartConceptsUsers" rel="nofollow">Users</a></td> 
   <td>for an overview of Users</td> 
  </tr> 
 </tbody>
</table>


[Context]: HelpStartConceptsContexts
[Users]: HelpStartConceptsUsers
[Session Properties]: HelpUiDialogsSessionContexts#auth
[session management method]: HelpStartConceptsSessionManagement
[here]: HelpUiDialogsSessionContexts