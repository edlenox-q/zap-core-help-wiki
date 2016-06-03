# Options Display screen #

The Display screen allows you to configure:

### Images ###

If ZAP processes images.

### Show (local) CONNECT requests ###

If the HTTP CONNECT requests received by the [Local Proxy][] should be persisted in the current [session][] and shown in the [History tab][]. The default is to not show those requests, they happen frequently (in preparation for TLS/SSL, WebSocket... connections) and, unless inspecting the behaviour of the client application, are not (usually) of much interest.

### Display ###

The layout of the 3 main panels.
The following options are available:

 *  Maximise left (Sites) tab - The 'tree' panel containing the Sites tab extends for the full length of the left hand side. This will reduce the amount of space available to the 'information' panel.
 *  Maximise bottom (History etc) tabs - The 'information' panel extends for the full length of the bottom. This will reduce the amount of space available to the 'tree' panel.
 *  Full Layout - The selected tab takes up the full screen. This is useful when using ZAP on small screens.

### Response Panel Position ###

Allows to configure the position of the Response tab with respect to Request tab.
The following options are available:

 *  Tabs Side by Side - The Request and Response tabs are side by side. This increases the information that can be displayed but means you cannot see both the request and response at the same time.
 *  Panels Side by Side - The Request panel is shown to the left of the Response panel. This decreases the information that can be displayed but means you can see both the request and response at the same time.
 *  Request Shown Above Response - The Request panel is shown above the Response panel. This decreases the information that can be displayed but means you can see both the request and response at the same time.

The Response Panel Position option does not apply when the Display option is set to Full Layout.

### Show break buttons ###

The location of the break buttons.

### Large request view min size ###

The minimum size of a request body in bytes at which point a 'large request body' message will be shown instead of the actual body.
This is to prevent very large bodies from slowing down the UI.
Setting this value to -1 will result in request always being displayed no matter how large it is.

### Large response view min size ###

The minimum size of a response body in bytes at which point a 'large response body' message will be shown instead of the actual body.
This is to prevent very large bodies from slowing down the UI.
Setting this value to -1 will result in response always being displayed no matter how large it is.

### Output Tabs Time Stamp Options ###

Once you've enabled time stamps on the output tab you can configure the format you would like those time stamps to appear in. Either select a pre-defined format from the drop-down list or enter one of your own choosing. The format is based on Java's SimpleDateFormat. After choosing or entering a time stamp format if you press enter the example on the right will be updated to reflect your choice. If ZAP is unable to use a format you've entered then the example is displayed based on the Default format.

<table> 
 <tbody>
  <tr> 
   <td> Long &amp; Default </td> 
   <td> yyyy-MM-dd HH:mm:ss </td> 
  </tr> 
  <tr> 
   <td> ISO8601 </td> 
   <td> yyyy-MM-dd'T'HH:mm:ssZ </td> 
  </tr> 
  <tr> 
   <td> Time Only </td> 
   <td> HH:mm:ss </td> 
  </tr> 
 </tbody>
</table>

### Font Size ###

The default text size used for the ZAP display. If you set this to -1 then the system default size will be used.
The 'Font Example' field will show you how large the default text will appear.
This setting will only take effect when ZAP is restarted.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface.</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiDialogsOptionsOptions" rel="nofollow">Options dialogs</a></td>
   <td>for details of the other Options dialog screens.</td>
  </tr> 
 </tbody>
</table>

## External Links ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> http://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html</td>
   <td>For details of Java's SimpleDateFormat.</td>
  </tr> 
 </tbody>
</table>


[Local Proxy]: HelpUiDialogsOptionsLocalproxy
[session]: HelpUiTlmenuFile
[History tab]: HelpUiTabsHistory