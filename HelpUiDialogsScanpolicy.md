# Scan Policy Dialog #

This allows you to enable and disable the rules that are run when performing an [active scan][].
The first screen allows you to define the default levels as well as the levels for all of the rules in a specific category.

The category screens allow you to define the levels for every individual rule.


Note that [passive scan][] rules are no longer managed via this dialog but are instead managed via the [Options Passive Scan Rules][].

### Threshold ###

This controls how likely ZAP is to report potential vulnerabilities.


 *  If you select Off then the scanner won't run.
 *  If you select Low then more potential issues will be raised which may increase the number of false positives.
 *  If you select High then fewer potential issues will be raised which may mean that some real issues are missed (false negatives).

### Strength ###

This controls the number of attacks that ZAP will perform.
If you select Low then fewer attacks will be used which will be quicker but may miss some issues.
If you select High then more attacks will be used which may find more issues but will take longer.
The Insane level should typically only be used for small parts of an application as it can result in a very large number of attacks being used, which can take a considerable length of time.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsScanpolicymgr" rel="nofollow">Scan Policy Manager dialog</a></td>
   <td></td>
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


[active scan]: HelpStartConceptsAscan
[passive scan]: HelpStartConceptsPscan
[Options Passive Scan Rules]: HelpUiDialogsOptionsPscanrules