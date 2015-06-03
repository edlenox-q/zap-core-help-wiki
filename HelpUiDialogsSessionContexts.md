# Session Contexts dialogs #

These screens allows you manage [contexts][].

There is a set of screens for each context you define.

### Top screen ###

This allows you to set the context name and description.

### Include in context ###

This allows you to manage the URLs which will be included in the context.
URLs which dont match any of the regexs will not be included in the context.

### Exclude from context ###

This allows you to manage the URLs which will be excluded from the context.
You only need to specify regexs for URLs that you do not want to include but which match one or more of the 'include' regexes.

### Technology ###

This allows you to specify the technologies used in the context, if known.
By default all technologies are included.
If you exclude technologies that you know are not used then this may speed up [active scanning][] as rules specific to the excluded technologies can be skipped.

### Authentication ###

This allows you to manage the way in which [Authentication][] is being done for the Context. Note that changing the authentication method after Users have been defined will cause them to be deleted, as the type of user credentials needs to match the authentication scheme. After selecting the Authentication Method type, the options that need to be configured depend on the Authentication Method.

#### Manual Authentication ####

No configuration is needed for this authentication method. Read [more][]...

#### Form-Based Authentication ####

To configure this authentication method, you need to supply the **login url**, to which the login request is performed, the **request body** (POST data), if needed, and identify the **parameters** used to supply the 'username' and 'password'. If no request body is supplied, the login request is performed as a HTTP GET, otherwise an HTTP POST is used. The credentials themselves are configured in the [Users][] tab. Read [more][more 1]...

#### HTTP/NTLM Authentication ####

To configure this authentication method, you need to supply the **hostname** and the **port** of the server the authentication is done with and the **realm** the credentials apply to. The credentials themselves are configured in the [Users][] tab. Read [more][more 2]...

#### Script-Based Authentication ####

To use this authentication method, you **first** need to write (and save) an **Authentication Script** using the **Scripts** tab (see the provided examples and templates for this script type in the Scripts tab). Then you need to supply the name of the script in the dropdown list. After selecting the script, you need to press the **Load** button, loading all the requirements of the script. Any parameters that you have specified as *required* or *optional* in the script will be shown in the interface to be defined. Their values are available to be used in the script, during the authentication, as seen in the provided examples for Authentication Scripts. Make sure that after doing any changes to the parameters required by the Authentication script you re-load the script. Otherwise, the parameters shown in the interface might not be the ones used during the authentication and errors might occur. The *credentials* used for each User during the authentication processed can be also specified in the Authentication Script and are configured in the [Users][] tab. Read [more][more 3]...

### Session Management ###

This allows you to manage the way in which Session Management is being done for the Context. After selecting the Session Management Method type, the options that need to be configured depend on the Session Management Method.

#### Cookie-Based Session Management ####

No configuration is needed for this session management method. Read [more][more 4]...

### Users ###

This allows you to configure a set of Users that may be used for various other actions throughout the application.

The credentials section of the Users depends on the Authentication Method configured for the Context.

## URL regexs ##

In the *Include in \**, *Exclude from \** panels and the *Logged in/out indicators* of the *Authentication* panel, you can enter regular expressions to define excluded URLs. While you can escape a single meta-character with a backslash, you can also use the **\\Q...\\E** escape sequence. All the characters between the **\\Q** and the **\\E** are interpreted as literal characters. E.g. \\Q\*\\d+\*\\E matches the literal text \*\\d+\*. This escape sequence is used in ZAP when you exclude URLs via some context menus.
**Note:** If your URL contains a "\\E", then you have to do the following steps when using the **\\Q...\\E** escape sequence:

 *  Open the escape sequence
 *  Close the escape sequence before the "character" \\E
 *  Escape the backslash
 *  Open after the "\\E" another escape sequence;
 *  Close the escape sequence as normally would.


Example: subdomain.example.com/path?a=**\\E**&moredata=2 should appear as *\\Qsubdomain.example.com/path?a=\\E***\\\\E***\\Q&moredata=2\\E*

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
   <td> <a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartConceptsAuthentication" rel="nofollow">Authentication</a></td>
   <td>for an overview of Authentication </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartConceptsSessionManagement" rel="nofollow">Session Management</a></td>
   <td>for an overview of Session Management </td>
  </tr> 
 </tbody>
</table>


[contexts]: HelpStartConceptsContexts
[active scanning]: HelpStartConceptsAscan
[Authentication]: HelpStartConceptsAuthentication
[more]: HelpStartConceptsAuthentication#manual
[Users]: HelpUiDialogsSessionContexts#users
[more 1]: HelpStartConceptsAuthentication#formBased
[more 2]: HelpStartConceptsAuthentication#httpAuth
[more 3]: HelpStartConceptsAuthentication#scriptBased
[more 4]: HelpStartConceptsSessionManagement#cbsm