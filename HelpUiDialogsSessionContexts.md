# Session Context screens #

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

### Structure ###

See the [Session Context Structure screen][].

### Technology ###

This allows you to specify the technologies used in the context, if known.
By default all technologies are included.
If you exclude technologies that you know are not used then this may speed up [active scanning][] as rules specific to the excluded technologies can be skipped.

### Authentication ###

See the [Session Context Authentication screen][].

### Session Management ###

This allows you to manage the way in which Session Management is being done for the Context. After selecting the Session Management Method type, the options that need to be configured depend on the Session Management Method.

#### Cookie-Based Session Management ####

No configuration is needed for this session management method. Read [more][]...

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
[Session Context Structure screen]: HelpUiDialogsSessionContext-struct
[active scanning]: HelpStartConceptsAscan
[Session Context Authentication screen]: HelpUiDialogsSessionContext-auth
[more]: HelpStartConceptsSessionManagement#cbsm