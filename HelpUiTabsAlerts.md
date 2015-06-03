# Alerts tab #

The Alerts tab show the [Alerts][] that have been raised in this session.
The alerts are displayed in a tree in risk order in the left hand pane, and each node of the tree shows the total number of alerts underneath it.
Selecting an alert with one click will display it in the right hand pane.
Double clicking an alert will display the [Add Alert][] dialog which will allow you to change the alert details.

Alerts can either be raised by [Automated scanning][] or manually via the [History tab][].

## Filtering alerts ##

The filter buttons, shown immediately above the tree, allows you to restrict which alerts are displayed:

### ![target.png][] /  ![target-grey.png][]  Show only URLs in Scope / Show all URLs ###

Allows to show only the alerts of URLs that are in [scope][].

### ![094.png][] /  ![earth-grey.png][]  Link / Unlink with Sites selection ###

Allows to show only the alerts of the [Sites tab][] selected tree node.

**Note:** Selecting one filter will disable the other as they are mutually exclusive.

## Right click menu ##

Right clicking on a node will bring up a menu which will allow you to:

### Resend... ###

This will bring up the [Resend dialog][] which allows you to resend the request associated with the alert after making any changes to it that you want to.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
 </tbody>
</table>


[Alerts]: HelpStartConceptsAlerts
[Add Alert]: HelpUiDialogsAddalert
[Automated scanning]: HelpStartConceptsAscan
[History tab]: HelpUiTabsHistory
[target.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/target.png
[target-grey.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/target-grey.png
[scope]: HelpStartConceptsScope
[094.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/094.png
[earth-grey.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/earth-grey.png
[Sites tab]: HelpUiTabsSites
[Resend dialog]: HelpUiDialogsResend