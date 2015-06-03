# History tab #

The History tab shows a list of all of the requests in the order in which they were made.
For each request you can see:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The request index - each request is numbered, starting at 1</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The HTML method, e.g. GET or POST</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The URL requested</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The HTTP response code</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>A short summary of what the HTTP response code means</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The length of time the whole request took</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Any <a href="HelpStartConceptsAlerts" rel="nofollow">Alerts</a> on the request</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Any <a href="HelpStartConceptsNotes" rel="nofollow">Notes</a> you have added to request</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Any <a href="HelpStartConceptsTags" rel="nofollow">Tags</a> on the request</td>
  </tr> 
 </tbody>
</table>

Selecting a requests will display it in the [Request tab][] and [Response tab][] above.


## The filter toolbar ##

A filter toolbar is provided which allows you to restrict which requests are displayed.
Clicking on the ![054.png][] Filter button displays the [History Filter dialog][].
A summary of the filter currently applied is displayed to the right of the button.

## Right click menu ##

Right clicking on a node will bring up a menu which will allow you to:

### Attack ###

The Attack menu has the following submenus:

#### Active Scan... ####

This will launch the [Active Scan][] dialog which allows you to initiate an [active scan][] with the starting point set to the request you selected.


#### Spider... ####

This will launch the [Spider][] dialog which allows you to initiate the [spider][] with the starting point set to the request you selected.


### Include in Context ###

This menu allows you to include the selected nodes and all of their subordinates in the specified [context][].
You also have the option to create a new context.
The [Session Contexts][] dialog will be displayed to allow you to make any additional changes.

### Exclude from Context ###

This menu allows you to exclude the selected nodes and all of their subordinates from the specified [context][].
The [Session Contexts][] dialog will be displayed to allow you to make any additional changes.

### Flag as context ###

This menu has the following submenus for each of the [contexts][context] you have defined:

#### Login request ####

This identifies the specified node as a login request.
You may only have one node identified as such in any one context.
The [Session Contexts][] dialog will be displayed to allow you to make any additional changes.

#### Logout request ####

This identifies the specified node as a logout request.
You may only have one node identified as such in any one context.
The [Session Contexts][] dialog will be displayed to allow you to make any additional changes.

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

### Manage Tags... ###

This will bring up the [Manage Tags dialog][] which allows you to change the [tags][] associated with the request.

### Note... ###

This will bring up the [Add Note dialog][] which allows you to record [notes][] related to the request.

### Delete ###

This will remove the node and all of its children from ZAP.
However they can be added back in, to prevent this use the 'Exclude from' menus.

### Break... ###

This will bring up the [Add Break Point dialog][] which allows you to set a break point on that URL.


### Scan this History ###

This will perform an [active scan][] against the URL related to the selected request.

### Alerts for this node ###

If the URL selected has [alerts][] associated with it then they will be listed under this menu.
Selecting one of the alerts will cause it to be displayed.

### Resend... ###

This will bring up the [Resend dialog][] which allows you to resend the request after making any changes to it that you want to.

### New Alert... ###

This will bring up the [Add Alert dialog][] which allows you to manually record a new [alert][alerts] against this request.

### Show in Sites tab ###

This will show the selected message in the [Sites tab][].

### Open URL in Browser ###

This will open the URL of the selected node in your default browser.

### Generate anti CSRF test form ###

This will open a URL which will give you a generated form for testing for CSRF issues.
It will only be enabled for POST requests, if the API is enabled and if Java supports the opening of URLs in a browser on your platform.

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


[Request tab]: HelpUiTabsRequest
[Response tab]: HelpUiTabsResponse
[054.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/054.png
[History Filter dialog]: HelpUiDialogsHist_filter
[Active Scan]: HelpUiDialogsAdvascan
[active scan]: HelpStartConceptsAscan
[Spider]: HelpUiDialogsSpider
[spider]: HelpStartConceptsSpider
[context]: HelpStartConceptsContexts
[Session Contexts]: HelpUiDialogsSessionContexts
[Session Properties]: HelpUiDialogsSessionSessprop
[Manage Tags dialog]: HelpUiDialogsManagetags
[tags]: HelpStartConceptsTags
[Add Note dialog]: HelpUiDialogsAddnote
[notes]: HelpStartConceptsNotes
[Add Break Point dialog]: HelpUiDialogsAddbreak
[alerts]: HelpStartConceptsAlerts
[Resend dialog]: HelpUiDialogsResend
[Add Alert dialog]: HelpUiDialogsAddalert
[Sites tab]: HelpUiTabsSites