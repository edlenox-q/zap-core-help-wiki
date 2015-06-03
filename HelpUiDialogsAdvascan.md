# Active Scan dialog #

This dialog launches the [active scanner][].


### Scope ###

The first tab allows you to select or change the starting point.
If you have more that one [scan policies][] then you will be able to select the one to use.
If the starting point is in one or more [Contexts][] then you will be able to choose one of them.
If that context has any [Users][] defined then you will be able to select one of them.
If you select one of the users then the active scan will be performed as that user, with ZAP (re)authenticating as that user whenever necessary.

If you select 'recurse' then all of the nodes underneath the one selected will also be scanned.
Custom input vectors are only supported if this option is not selected.

If you select 'Show advanced options' then the following tabs will be shown which provide fine grain control over the active scanning process.

Clicking on the 'Reset' button will reset all of the options to their default values.

### Input Vectors ###

The Input Vectors tab allows you override the default input vectors which are defined in the [Options Active Scan Input Vectors screen][].
Clicking on the 'Reset' button will reset the input vectors to the default options.

### Custom Vectors ###

The Custom Vectors tab allows you specify specific locations in the request to attack.
Custom Vectors are only available if the 'recurse' option on the first tab is not selected.
To add custom input vectors highlight the characters you want to attack in the request and lick the 'Add' button.
You can add as many custom input vectors as you want.
To remove custom input vectors highlight any of the selected characters and click the 'Remove' button.
Checking the 'Disable non custom input vectors' box disables all of the input vectors except those you manually define on this tab.

### Technology ###

The Technology tab allows you to specify which types of technologies to scan.
Un-selecting technologies that you know are not present in the target application may speed up the scan as rules which target that technology can skip those tests.

### Policy ###

The Policy tab allows you to override any of the settings specified in the selected [scan policy][scan policies].



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
   <td><a href="HelpUiTlmenuTools" rel="nofollow">Top level Tools menu</a></td>
   <td>'Active Scan...' menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsSites" rel="nofollow">Sites tab</a></td>
   <td>'Attack / Active Scan... right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsHistory" rel="nofollow">History tab</a></td>
   <td>'Attack / Active Scan...' right click menu item</td>
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
   <td> <a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
 </tbody>
</table>


[active scanner]: HelpStartConceptsAscan
[scan policies]: HelpStartConceptsScanpolicy
[Contexts]: HelpStartConceptsContexts
[Users]: HelpStartConceptsUsers
[Options Active Scan Input Vectors screen]: HelpUiDialogsOptionsAscaninput