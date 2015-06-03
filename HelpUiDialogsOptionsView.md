# Options Display screen #

The Display screen allows you to configure:

### Images ###

If ZAP processes images.

### Display ###

The layout of the 3 main windows.

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

### Font Size ###

The default text size used for the ZAP display. If you set this to -1 then the system default size will be used.
The 'Font Example' field will show you how large the default text will appear.
This setting will only take effect when ZAP is restarted.

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
   <td> https://code.google.com/p/zaproxy/downloads/list</td> 
   <td> ZAP download page</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> http://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html</td>
   <td>For details of Java's SimpleDateFormat.</td>
  </tr> 
 </tbody>
</table>