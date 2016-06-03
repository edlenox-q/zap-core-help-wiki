# HTTP Sessions tab #

This tab shows you the set of identified HTTP sessions for each Site, as detected by the [HTTP Sessions extension][].

The current Site the information is referring to can be selected via the toolbar or the [Sites tab][].

The toolbar provides a button ("New Session") which allows you to start a new session, forcing all outgoing request messages to be without the session tokens set, so the server considers it's a new session. This allows the creation of a new session, without destroying the old one.

Each of the entries in the Sessions table (each session) initially has a generated name, but it can be changed by selecting the 'Name' cell and editing it.

Each of the entries in the Sessions table can be right clicked, which activates the Popup Menu, with the following options:

 *  Remove Session - deletes the session
 *  Set as active (available only on non-active sessions) - marks this session as active. If any session was previously set as active, it will be unset as active and, if it doesn't specify any token values, it is deleted.
 *  Unset as active (available only on the active session) - marks this session as not being active anymore. If the session doesn't specify any token values, it is deleted.

*Regarding the active session, more details can be read on the general concepts help page of the [HTTP Sessions extension][]*

For each session you can see:

 *  Active - Whether this is the active session or not
 *  Name - The session name
 *  Session Tokens' Values - the list of values associated to each of the session tokens. The entries are separated by the ';' symbol.
 *  Messages Matched - the number of HTTP messages that have been matched by the extension with this session

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
   <td><a href="HelpStartConceptsHttpsessions" rel="nofollow">HTTP Sessions Extension</a></td> 
   <td>for an overview of the extension</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsOptionsHttpsessions" rel="nofollow">HTTP Sessions Options screen</a></td> 
   <td>for an overview of the extension's Options</td> 
  </tr> 
 </tbody>
</table>


[HTTP Sessions extension]: HelpStartConceptsHttpsessions
[Sites tab]: HelpUiTabsSites