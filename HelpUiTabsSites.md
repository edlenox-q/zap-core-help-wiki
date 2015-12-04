# Sites tab #

The Sites tab shows all of the URLs visited in a tree structure.
You can select any of the nodes in the tree to display the request and response for that URL in the relevant tabs.


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

#### *Context name* Form-based Auth Login request ####

This identifies the specified node as a login request for the specified context.
You may only have one node identified as such in any one context.
The [Session Context Authentication][] screen will be displayed to allow you to make any additional changes.

#### *Context name* Data driven node ####

This identifies the specified node as [Data driven content][] for the specified context.
The [Session Context Structure][] screen will be displayed to allow you to make any additional changes.

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

### Delete ###

This will remove the node and all of its children from ZAP.
However they can be added back in, to prevent this use the 'Exclude from' menus.

### Break... ###

This will bring up a new window which will allow you to set a [break point][] on that URL.
The break point is defined via a regular expression. If you visit a URL which matches this expression then ZAP will intercept it and allow you to change either the request and/or the response.

### Alerts for this node ###

If the URL selected has [alerts][] associated with it then they will be listed under this menu.
Selecting one of the alerts will cause it to be displayed.

### Resend... ###

This will bring up the [Resend dialog][] which allows you to resend the request after making any changes to it that you want to.

### New Alert... ###

This will bring up the [Add Alert dialog][] which allows you to manually record a new [alert][alerts] against this request.

### Show in History tab ###

This will show the selected node in the [History tab][].

### Open URL in Browser ###

This will open the URL of the selected node in your default browser.

### Generate anti CSRF test form ###

This will open a URL which will give you a generated form for testing for CSRF issues.
It will only be enabled for POST requests, if the API is enabled and if Java supports the opening of URLs in a browser on your platform.

### Refresh Sites tree ###

Occasionally the Sites tree can be displayed incorrectly - this option will redraw it.

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


[Active Scan]: HelpUiDialogsAdvascan
[active scan]: HelpStartConceptsAscan
[Spider]: HelpUiDialogsSpider
[spider]: HelpStartConceptsSpider
[context]: HelpStartConceptsContexts
[Session Contexts]: HelpUiDialogsSessionContexts
[Session Context Authentication]: HelpUiDialogsSessionContext-auth
[Data driven content]: HelpStartConceptsDdc
[Session Context Structure]: HelpUiDialogsSessionContext-struct
[Session Properties]: HelpUiDialogsSessionSessprop
[break point]: HelpStartConceptsBreakpoints
[alerts]: HelpStartConceptsAlerts
[Resend dialog]: HelpUiDialogsResend
[Add Alert dialog]: HelpUiDialogsAddalert
[History tab]: HelpUiTabsHistory