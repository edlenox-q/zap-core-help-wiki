# Session Context Authentication screen #

This is one of the [Session Context screens][] which allows you to manage the way in which [Authentication][] is being done for the Context. Note that changing the authentication method after Users have been defined will cause them to be deleted, as the type of user credentials needs to match the authentication scheme. After selecting the Authentication Method type, the options that need to be configured depend on the Authentication Method.

#### Manual Authentication ####

No configuration is needed for this authentication method. Read [more][]...

#### Form-Based Authentication ####

To configure this authentication method, you need to supply the **login url**, to which the login request is performed, the **request body** (POST data), if needed, and identify the **parameters** used to supply the 'username' and 'password'. If no request body is supplied, the login request is performed as a HTTP GET, otherwise an HTTP POST is used. The credentials themselves are configured in the [Users][] tab. Read [more][more 1]...

#### HTTP/NTLM Authentication ####

To configure this authentication method, you need to supply the **hostname** and the **port** of the server the authentication is done with and the **realm** the credentials apply to. The credentials themselves are configured in the [Users][] tab. Read [more][more 2]...

#### Script-Based Authentication ####

To use this authentication method, you **first** need to write (and save) an **Authentication Script** using the **Scripts** tab (see the provided examples and templates for this script type in the Scripts tab). Then you need to supply the name of the script in the dropdown list. After selecting the script, you need to press the **Load** button, loading all the requirements of the script. Any parameters that you have specified as *required* or *optional* in the script will be shown in the interface to be defined. Their values are available to be used in the script, during the authentication, as seen in the provided examples for Authentication Scripts. Make sure that after doing any changes to the parameters required by the Authentication script you re-load the script. Otherwise, the parameters shown in the interface might not be the ones used during the authentication and errors might occur. The *credentials* used for each User during the authentication processed can be also specified in the Authentication Script and are configured in the [Users][] tab. Read [more][more 3]...

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTlmenuFile" rel="nofollow">Top level File menu</a></td>
   <td>'Properties...' menu item</td>
  </tr> 
 </tbody>
</table>

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsSessionContexts" rel="nofollow">Session Context screens</a></td>
   <td>for details of the other Context screens</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpStartConceptsAuthentication" rel="nofollow">Authentication</a></td>
   <td>for an overview of Authentication </td>
  </tr> 
 </tbody>
</table>


[Session Context screens]: HelpUiDialogsSessionContexts
[Authentication]: HelpStartConceptsAuthentication
[more]: HelpStartConceptsAuthentication#manual
[Users]: HelpUiDialogsSessionContexts#users
[more 1]: HelpStartConceptsAuthentication#formBased
[more 2]: HelpStartConceptsAuthentication#httpAuth
[more 3]: HelpStartConceptsAuthentication#scriptBased