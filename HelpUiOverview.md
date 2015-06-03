# UI Overview #

The UI is made up of:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTlmenuTlmenu" rel="nofollow">Top Level Menu</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTltoolbar" rel="nofollow">Top Level Toolbar</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Three windows which contain multiple tabs, detailed below</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiFooter" rel="nofollow">Footer</a></td>
   <td></td>
  </tr> 
 </tbody>
</table>

Each of the three windows has a set of one or more tabs.
By default only the essential tabs are now shown when ZAP starts up.
The remaining tabs are revealed when they are used (e.g. for the spider and active scanner) or when you display them via the special tab on the far right of each window with the green '+' icon. This special tab disappears if there are no hidden tabs.
Tabs can be closed via a small 'x' icon which is shown when the tab is selected.
Tabs can also be 'pinned' using a small 'pin' icon that is also shown when the tab is selected - pinned tabs will be shown when ZAP next starts up.

### The 'tree' window ###

This is displayed on the left hand side and allows you to navigate around the URLs visited.

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsSites" rel="nofollow">Sites tab</a></td>
   <td>This shows all of the URLs visited in a tree structure</td>
  </tr> 
 </tbody>
</table>

### The 'workspace' window ###

This is displayed on the top right hand side and is where requests and responses are displayed. You can also make changes here when a [break point][] has been hit.

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsRequest" rel="nofollow">Request tab</a></td>
   <td>This shows the data your browser sends to the application</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsResponse" rel="nofollow">Response tab</a></td>
   <td>This shows the data the application sends back to your browser</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsBreak" rel="nofollow">Break tab</a></td>
   <td>This allows you to manipulate the data</td>
  </tr> 
 </tbody>
</table>

### The 'information' window ###

This is displayed on the bottom and is where useful information is displayed.

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsHistory" rel="nofollow">History tab</a></td>
   <td>This shows the requests in the order they were made</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsSearch" rel="nofollow">Search tab</a></td>
   <td>This allows you to search all of the requests and responses</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsBreakpoints" rel="nofollow">Break points tab</a></td>
   <td>This shows the Break Points set</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsAlerts" rel="nofollow">Alerts tab</a></td>
   <td>This shows the alerts raised on the application</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsAscan" rel="nofollow">Active Scan tab</a></td>
   <td>This shows the active scans</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsSpider" rel="nofollow">Spider tab</a></td>
   <td>This shows the URLs not yet visited</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsParams" rel="nofollow">Params tab</a></td>
   <td>This shows a summary of the parameters a site uses</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsOutput" rel="nofollow">Output tab</a></td>
   <td>This shows various informational messages</td>
  </tr> 
 </tbody>
</table>

All but the most essential tabs can be hidden by clicking on the grey 'x' on the tab title.
You can display tabs you have hidden via the [View Menu][].
Hidden tabs may also appear when 'activated' by another action.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartStart" rel="nofollow">Getting Started</a></td>
   <td>for details of how to start using ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpIntro" rel="nofollow">Introduction</a></td>
   <td>the introduction to ZAP</td>
  </tr> 
 </tbody>
</table>


[break point]: HelpStartConceptsBreakpoints
[View Menu]: HelpUiTlmenuView