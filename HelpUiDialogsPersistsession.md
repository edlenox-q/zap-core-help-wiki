# Persist Session dialog #

This dialog is shown by default whenever you start a new session, which always happens when ZAP starts.
It allows you to specify how you would like this session persisted, you can also set the default choice so that you are not prompted again.

Persisting a session means it will be stored in a local database that you can access at a later date.
You do not need to keep 'saving' a session as everything that happens in the session is continually recorded.
It is much faster to persist a session at the start, but you can always persist a session later if you need to.
If you close ZAP without persisting your session then you will not be able to access it again.

### Yes, I want to persist this session with name based on the current timestamp ###

Chose this option if you would like ZAP to store the session in the default directory with a name based on the current time.

### Yes, I want to persist this session but I want to specify the name and location ###

Chose this option if you would like to specify exactly where ZAP should store the session.

### No, I do not want to persist this session at this moment in time ###

Chose this option if you do not want ZAP to store the session.
You can choose to store it at a later time using the [Persist Session...][] menu item.

### Remember my choice and do not ask me again. ###

Check this box if you want ZAP to remember your decision and not prompt you again.
You can change your decision via the [Options database][] screen.

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
   <td> <a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
 </tbody>
</table>


[Persist Session...]: HelpUiTlmenuFile
[Options database]: HelpUiDialogsOptionsDatabase