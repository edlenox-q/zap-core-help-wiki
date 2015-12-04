# Search tab #

The Search tab allows you to search for regular expressions in all of the URLs, requests, responses, headers and in other functionalities provided by add-ons.

Enter the regular expression you would like to search for in the search box and either press return or click on the search button: ![049.png][]

A pull down allows you to choose whether to search across the URLs, the requests, the responses or everything.

All URLs, requests or responses which contain the search pattern will be displayed in the tab.
You may find it useful to add .\* to your search term - this will give you more context e.g. password.\*

You can use the ![107.png][] Next and ![108.png][] Previous buttons to view found search terms in the [Request][] and [Response tabs][].


You can also go directly to a specific instance by clicking on the relevant line in the results list.

## Right click menu ##

Right clicking on a node will bring up a menu which will allow you to:

### Attack ###

The Attack menu has the following submenus:

#### Active Scan Site ####

This will initiate an [active scan][] of the whole of the site containing the selected node.
The [Active Scan tab][] will be display and will show the progress of the scan.


#### Active Scan Node ####

This will initiate an [active scan][] of just the node selected.
The [Active Scan tab][] will be display and will show the progress of the scan.


#### Spider Site ####

This will initiate a [spider][] of the whole of the site containing the selected node.
The [Spider tab][] will be display and will show the progress of the scan.


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

### Resend... ###

This will bring up the [Resend dialog][] which allows you to resend the request after making any changes to it that you want to.

### New Alert... ###

This will bring up the [Add Alert dialog][] which allows you to manually record a new [alert][] against this request.

### Show in History tab ###

This will show the selected node in the [History tab][].

### Show in Sites tab ###

This will show the selected message in the [Sites tab][].

### Open URL in Browser ###

This will open the URL of the selected node in your default browser.

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


[049.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/049.png
[107.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/107.png
[108.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/108.png
[Request]: HelpUiTabsRequest
[Response tabs]: HelpUiTabsResponse
[active scan]: HelpStartConceptsAscan
[Active Scan tab]: HelpUiTabsAscan
[spider]: HelpStartConceptsSpider
[Spider tab]: HelpUiTabsSpider
[context]: HelpStartConceptsContexts
[Session Contexts]: HelpUiDialogsSessionContexts
[Session Context Authentication]: HelpUiDialogsSessionContext-auth
[Data driven content]: HelpStartConceptsDdc
[Session Context Structure]: HelpUiDialogsSessionContext-struct
[Session Properties]: HelpUiDialogsSessionSessprop
[Resend dialog]: HelpUiDialogsResend
[Add Alert dialog]: HelpUiDialogsAddalert
[alert]: HelpStartConceptsAlerts
[History tab]: HelpUiTabsHistory
[Sites tab]: HelpUiTabsSites