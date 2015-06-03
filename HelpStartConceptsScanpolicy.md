# Scan Policy #

A scan policy defines exactly which [rules][] are run as part of an [active scan][].
It also defines how these rules run influencing how many requests are made and how likely potential issues are to be flagged.
You can define as many scan policies as you like and select the most appropriate one when you start the scan via the [Active Scan Dialog][].
You can define the default scan policy to be used for active scans and for the [Attack mode][] via the [Options Active Scan screen][].


Active scanning is an attack on those targets.
You should NOT use it on web applications that you do not own.

It should be noted that active scanning can only find certain types of vulnerabilities.
Logical vulnerabilities, such as broken access control, will not be found by any active or automated vulnerability scanning.
Manual penetration testing should always be performed in addition to active scanning to find all types of vulnerabilities.

Active scanning is configured using the [Options Active Scan screen][].
You can also define as many scan policies as you like - these define exactly which rules are run and how they work.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsAscan" rel="nofollow">Active Scan tab</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsSites" rel="nofollow">Sites tab</a></td>
   <td>'Attack/Active Scan site' right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsSites" rel="nofollow">Sites tab</a></td>
   <td>'Attack/Active Scan node' right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsHistory" rel="nofollow">History tab</a></td>
   <td>'Scan this History' right click menu item</td>
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
   <td> <a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td>
   <td>provided by ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartConceptsPscan" rel="nofollow">Passive scanning</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiDialogsScanpolicymgr" rel="nofollow">Scan Policy Manager Dialog</a></td>
   <td>which allows you to manage the scan policies</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartChecks" rel="nofollow">Scanner Rules</a></td>
   <td>supported by default</td>
  </tr> 
 </tbody>
</table>


[rules]: HelpStartChecks
[active scan]: HelpStartConceptsAscan
[Active Scan Dialog]: HelpUiDialogsAdvascan
[Attack mode]: HelpStartConceptsModes
[Options Active Scan screen]: HelpUiDialogsOptionsAscan