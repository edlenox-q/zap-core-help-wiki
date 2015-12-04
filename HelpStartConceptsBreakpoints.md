# Break Points #

A break point allows you to intercept a request from your browser and to change it before is is submitted to the web application you are testing.
You can also change the responses received from the application
The request or response will be displayed in the [Break tab][] which allows you to change disabled or hidden fields, and will allow you to bypass client side validation (often enforced using javascript).
It is an essential penetration testing technique.

You can set a 'global' break point on requests and/or responses using the buttons on the [top level toolbar][].
All requests and/or responses will then be intercepted by ZAP allowing you to change anything before allowing the request or response to continue.

You can also set break points on specific criteria using the "Break..." right click menu on the [Sites][] and [History tabs][] and the 'Add a custom HTTP break point' button on the [top level toolbar][].
Only requests and responses which match those criteria will be intercepted by ZAP.
Custom break points are shown in the [Break Points tab][]

Break point option are configured using the [Options Break Points screen][].


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
   <td> <a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td>
   <td>provided by the UI</td>
  </tr> 
 </tbody>
</table>


[Break tab]: HelpUiTabsBreak
[top level toolbar]: HelpUiTltoolbar
[Sites]: HelpUiTabsSites
[History tabs]: HelpUiTabsHistory
[Break Points tab]: HelpUiTabsBreakpoints
[Options Break Points screen]: HelpUiDialogsOptionsBreakpoints