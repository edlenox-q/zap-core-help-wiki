# Alerts #

An alert is a potential vulnerability and is associated with a specific request.
A request can have more than one alert.


Alerts are shown in the UI with a flag indicating the risk:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><img src="https://github.com/zaproxy/zap-core-help/wiki/images/16/071.png" align="bottom" width="16" height="16" />&nbsp; High</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><img src="https://github.com/zaproxy/zap-core-help/wiki/images/16/076.png" align="bottom" width="16" height="16" />&nbsp; Medium</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><img src="https://github.com/zaproxy/zap-core-help/wiki/images/16/074.png" align="bottom" width="16" height="16" />&nbsp; Low</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><img src="https://github.com/zaproxy/zap-core-help/wiki/images/16/073.png" align="bottom" width="16" height="16" />&nbsp; Informational</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><img src="https://github.com/zaproxy/zap-core-help/wiki/images/16/072.png" align="bottom" width="16" height="16" />&nbsp; False Positive</td>
   <td></td>
  </tr> 
 </tbody>
</table>

Alerts can be raised by various ZAP components, including but not limited to: [active scanning][], [passive scanning][], scripts, by addons (extensions), or manually using the [Add Alert dialog][] (which also allows you to update or change alert details/information).

Alerts are flagged in the [History tab][] with a flag which indicates the highest risk alert.
All alerts are listed in the [Alerts tab][] and a count of the total number of alerts by risk is shown in the [footer][].

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


[active scanning]: HelpStartConceptsAscan
[passive scanning]: HelpStartConceptsPscan
[Add Alert dialog]: HelpUiDialogsAddalert
[History tab]: HelpUiTabsHistory
[Alerts tab]: HelpUiTabsAlerts
[footer]: HelpUiFooter