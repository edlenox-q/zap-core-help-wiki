# Options Database screen #

This screen allows you to configure the database options:

### Compact (on exit) ###

Allows to compact the database when ZAP is closed, compacting the database ensures a minimal space disk usage but it will also take longer to exit ZAP.

### Recovery Log ###

Controls whether or not database's recovery log is enabled.
Improves the performance of the database when disabled but might lead to data loss if ZAP is exited abruptly.
Note: current session will be unaffected, changes take effect on new and opened sessions.

### Maximum Request Body Size ###

The largest request body size in bytes that ZAP will allow.

### Maximum Response Body Size ###

The largest response body size in bytes that ZAP will allow.

### Prompt for persistence options on new session ###

If checked then the [Persist Session dialog][] will be shown when a new session is created.

### Default option ###

The default option for new sessions - if the above prompt is enabled then the default option will be selected.
If the prompt is not enabled then this is the action that will be taken.

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
   <td> <a href="HelpUiDialogsOptionsOptions" rel="nofollow">Options dialogs</a></td>
   <td>for details of the other Options dialog screens</td>
  </tr> 
 </tbody>
</table>


[Persist Session dialog]: HelpUiDialogsPersistsession