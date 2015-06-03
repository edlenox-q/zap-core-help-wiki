# Active Scan #

Active scanning attempts to find potential vulnerabilities by using known attacks against the selected targets.

Active scanning is an attack on those targets.
You should NOT use it on web applications that you do not own.

It should be noted that active scanning can only find certain types of vulnerabilities.
Logical vulnerabilities, such as broken access control, will not be found by any active or automated vulnerability scanning.
Manual penetration testing should always be performed in addition to active scanning to find all types of vulnerabilities.

Active scanning is configured using the [Options Active Scan screen][].
The rules that run are configured via [Scan Policies][] \- you can have as many of these as you like.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsAscan" rel="nofollow">Active Scan tab</a></td>
   <td>'New Scan' button</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsSites" rel="nofollow">Sites tab</a></td>
   <td>'Attack/Active Scan...' right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsHistory" rel="nofollow">History tab</a></td>
   <td>'Attack/Active Scan...' right click menu item</td>
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


[Options Active Scan screen]: HelpUiDialogsOptionsAscan
[Scan Policies]: HelpStartConceptsScanpolicy