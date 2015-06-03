# The File menu #

This menu handles the current session. By default the following menu items will be present:


### New Session ###

This creates a new session.
If you have not saved your current session then a warning will be displayed.
Starting a new session without saving the current session will loose all of the data in the current session.

### Open Session... ###

This opens a session that has been previously saved.
Opening a session without saving the current session will loose all of the data in the current session.

### Persist Session... ###

This persists the current session.
While the session is always stored in a database on disk, it will be lost when ZAP is stopped unless it has been persisted.
You only need to persist it once - after that all changes will be saved.

### Snapshot Session ###

This saves a snapshot of a session that has already been persisted.
It will use the same filename with a date-time string appended to it.


### Properties... ###

This displays the [Session Properties][] dialog.
This allows you to set the session name and description.

### Load Add-on file... ###

Load a local [add-on][] file.
Add-ons are typically installed from via the [Manage Add-ons][] dialog, but this option can be useful if you have downloaded an add-on manually or are testing one you have developed yourself.
Add-ons remain installed until you manually uninstall them.

### Exit and delete session... ###

This will exit ZAP and delete the session, even if you have previously persisted it.
The session will no longer be accessible when you restart ZAP, although any snapshots you took will still be available.
A warning dialog will be displayed to ensure you really meant to choose this option.

### Exit ###

This will exit ZAP.
If you have not saved the current session then you will be given the option to do so.

Note that [add-ons][add-on] can add additional menu items.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTlmenuTlmenu" rel="nofollow">The top level menu</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
 </tbody>
</table>


[Session Properties]: HelpUiDialogsSessionSessprop
[add-on]: HelpStartConceptsAddons
[Manage Add-ons]: HelpUiDialogsManageaddons