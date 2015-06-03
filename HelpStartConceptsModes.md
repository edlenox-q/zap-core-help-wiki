# Modes #

The ZAP UI has a 'mode' which can be:

 *  Safe - no potentially dangerous operations permitted
 *  Protected - you can only perform (potentially) dangerous actions on URLs in the [Scope][]
 *  Standard - as in previous releases, you can do anything
 *  ATTACK - new nodes that are in [Scope][] are [actively scanned][] as soon as they are discovered

It is recommended that you use the Protected mode to ensure that you only attack sites that you mean to.

The mode can be changed via the [toolbar][] and is persisted between sessions.
It does not apply to the API.

Examples of the things that will not be possible in either Safe mode or in Protected mode when not acting on URLs in the Scope:

 *  Spidering
 *  Active Scanning
 *  Fuzzing
 *  Force Browsing
 *  Breaking (intercepting)
 *  Resending requests

You can define the [Scan Policy][] to be used for the Attack mode the [Options Active Scan screen][].


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
 </tbody>
</table>


[Scope]: HelpStartConceptsScope
[actively scanned]: HelpStartConceptsAscan
[toolbar]: HelpUiTltoolbar
[Scan Policy]: HelpStartConceptsScanpolicy
[Options Active Scan screen]: HelpUiDialogsOptionsAscan