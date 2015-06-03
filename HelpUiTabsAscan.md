# Active Scan tab #

The Active Scan tab allows you to perform an [active scan][].

The 'New Scan' button launches the [Active Scan dialog][] which allows you to specify exactly what should be scanned.

The toolbar provides a set of buttons which allow you to start, stop, pause and resume the scan selected.
A progress bar shows how far the scan of the selected site has progressed.
The 'Current scans' value shows how many scans are currently active - hovering over this value will show a list of the sites being scanned in a popup.

## Right click menu ##

Right clicking on a node will bring up a menu which will allow you to:

### Exclude from ###

This menu has the following submenus:

#### Proxy ####

This will exclude the selected nodes from the proxy. They will still be proxied via ZAP but will not be shown in any of the tabs.
This can be used to ignore URLs that you know are not relevant to the system you are currently testing.
The nodes can be included again via the [Session Properties][] dialog

#### Scanner ####

This will prevent the selected nodes from being actively scanned.
The nodes can be included again via the [Session Properties][] dialog

#### Spider ####

This will prevent the selected nodes from being spidered.
The nodes can be included again via the [Session Properties][] dialog

### Resend... ###

This will bring up the [Resend dialog][] which allows you to resend the request after making any changes to it that you want to.

### New Alert... ###

This will bring up the [Add Alert dialog][] which allows you to manually record a new [alert][] against this request.

### Show in Sites tab ###

This will show the selected message in the [Sites tab][].

### Open URL in Browser ###

This will open the URL of the selected node in your default browser.

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
   <td> <a href="HelpUiDialogsOptionsAscan" rel="nofollow">Options Active Scan screen</a></td>
   <td>for details of the active scan configuration</td>
  </tr> 
 </tbody>
</table>


[active scan]: HelpStartConceptsAscan
[Active Scan dialog]: HelpUiDialogsAdvascan
[Session Properties]: HelpUiDialogsSessionSessprop
[Resend dialog]: HelpUiDialogsResend
[Add Alert dialog]: HelpUiDialogsAddalert
[alert]: HelpStartConceptsAlerts
[Sites tab]: HelpUiTabsSites