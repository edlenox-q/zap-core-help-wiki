# Session Properties dialog #

This allows you to set the session properties and is made up of the following screens:

### General screen ###

This allows you to set the session name and description.

### Exclude from proxy ###

This allows you to manage the URLs which will be ignored by the proxy.

### Exclude from scanner ###

This allows you to manage the URLs which will be ignored by the scanner.

### Exclude from spider ###

This allows you to manage the URLs which will be ignored by the spider.

### Contexts ###

A set of screens for managing [contexts][]

## URL regexs ##

In the *Exclude from \** dialogs, you can enter regular expressions to define excluded URLs. While you can escape a single meta-character with a backslash, you can also use the **\\Q...\\E** escape sequence. All the characters between the **\\Q** and the **\\E** are interpreted as literal characters. E.g. \\Q\*\\d+\*\\E matches the literal text \*\\d+\*. This escape sequence is used in ZAP when you exclude URLs via some context menus.
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
 </tbody>
</table>


[contexts]: HelpStartConceptsContexts