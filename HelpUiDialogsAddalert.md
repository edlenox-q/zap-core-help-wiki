# Add Alert dialog #

This dialog allows you to manually add or change an [Alert][] associated with a specific request.


## Fields ##

The dialog has the following fields:

### Type ###

The type of the alert is a pull down field which allows you to select one of a prepopulated set of issue types.
You can also enter your own text or change the text of one of the items you selected.
If you select on of the existing types then the Description, Solution and Other Info fields will be populated with text associated with the item you chose.

### Risk ###

A pull down field which allows you to specify how serious you think the risk is:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Informational</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Low</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Medium</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>High</td>
   <td></td>
  </tr> 
 </tbody>
</table>

### Confidence ###

A pull down field which allows you to specify how confident you are in the validity of the finding:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>False Positive</td>
   <td>for potential issues that you later find are not exploitable</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Low</td>
   <td>for unconfirmed issues</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Medium</td>
   <td>for issues you are somewhat confident of</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>High</td>
   <td>for findings you are highly confident in</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Confirmed</td>
   <td>for confirmed issues</td>
  </tr> 
 </tbody>
</table>

### Parameter ###

A pull down field which allows you to specify which parameter the issue is associated with.
The field is prepopulated with any URL and FORM parameters found, but you can also enter your own parameter name.

### Description ###

A general description of the type of issue found.
This is populated when you select one of the predefined types, but you can also change it as required.
Note that any changes you make will be lost if you select another type.

### Other Info ###

Information specific to the particular issue you have found.
This is not prepopulated.

### Solution ###

Recommendations about how to fix the issue.
This is populated when you select one of the predefined types, but you can also change it as required.
Note that any changes you make will be lost if you select another type.

### Reference ###

One or more URLs pointing to more information on the internet about the selected type of alert.
This is populated when you select one of the predefined types, but you can also change it as required.
Note that any changes you make will be lost if you select another type.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsHistory" rel="nofollow">History tab</a></td>
   <td>'New Alert...' right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTabsAlerts" rel="nofollow">Alerts tab</a></td>
   <td>double clicking on an existing alert</td>
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


[Alert]: HelpStartConceptsAlerts