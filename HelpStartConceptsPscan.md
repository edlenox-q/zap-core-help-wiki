# Passive Scan #

ZAP passively scans all of the responses from the web application being tested.
Passive scanning does not change the responses in any way and is therefore safe to use.
Scanned is performed in a background thread to ensure that it does not slow down the exploration of an application.

In this release ZAP passive scanning is used for automatically adding [tags][] and raising [alerts][] for potential issues.

A set of rules for automatic tagging are provided by default.
These can be changed, deleted or added to via the [Options Passive Scan Tags screen][].


The alerts raised by passive scanning can be configured using the [Options Passive Scan Rules screen][].


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
   <td>provided by ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartConceptsAscan" rel="nofollow">Active scanning</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartChecks" rel="nofollow">Scanner Rules</a></td>
   <td>supported by default</td>
  </tr> 
 </tbody>
</table>


[tags]: HelpStartConceptsTags
[alerts]: HelpStartConceptsAlerts
[Options Passive Scan Tags screen]: HelpUiDialogsOptionsPscan
[Options Passive Scan Rules screen]: HelpUiDialogsOptionsPscanrules