# Spider dialog #

This dialog launches the [spider][].


## Scope ##

The first tab allows you to select or change the starting point.
If the starting point is in one or more [Contexts][] then you will be able to choose one of them.
If that context has any [Users][] defined then you will be able to select one of them.
If you select one of the users then the spider will be performed as that user, with ZAP (re)authenticating as that user whenever necessary.

If you select 'recurse' then all of the nodes underneath the one selected will also be used to seed the spider.

If you select 'Show advanced options' then the following tab will be shown which provide fine grain control over the spider process.

Clicking on the 'Reset' button will reset all of the options to their default values.

## Advanced ##

Most of the parameters on this tab correspond to the same parameters on the [Options Spider screen][].


### Maximum children to crawl ###

This parameter limits the number of children that will be crawled at every node in the tree.
This is useful for data driven applications that have large numbers of 'pages' that are in fact exactly the same code but containing different data, for example from a database.
By default this is set to zero which means there are no limits applied to the number of child nodes crawled.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsSpider" rel="nofollow">Spider tab</a></td>
   <td>'New Scan' button</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsSites" rel="nofollow">Sites tab</a></td>
   <td>'Attack / Spider...' right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsHistory" rel="nofollow">History tab</a></td>
   <td>'Attack / Spider...' right click menu item</td>
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


[spider]: HelpStartConceptsSpider
[Contexts]: HelpStartConceptsContexts
[Users]: HelpStartConceptsUsers
[Options Spider screen]: HelpUiDialogsOptionsSpider