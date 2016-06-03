# Top Level Toolbar #

This toolbar provides a set of controls for commonly used functionality.

## Mode pulldown ##

This allows you to change the current [mode][].

## ![171.png][]  New Session ##

This button is the same as the [File menu][] 'New Session' menu item.

## ![047.png][]  Open Session ##

This button is the same as the [File menu][] 'Open Session' menu item.

## ![096.png][]  Persist Session... ##

This button is the same as the [File menu][] 'Persist Session...' menu item.

## ![camera.png][]  Snapshot Session ##

This button is the same as the [File menu][] 'Snapshot Session' menu item.

## ![024.png][]  Session Properties... ##

This button is the same as the [File menu][] 'Properties...' menu item.

## ![041.png][]  Options... ##

This button is the same as the [Tools menu][] 'Options...' menu item.

## ![ui-tab-show.png][]  Show all tabs ##

This button reveals all of the hidden tabs.

## ![ui-tab-hide.png][]  Hide unpinned tabs ##

This button hides all of the tabs that are 'unpinned'. Tabs can be pinned and unpinned via the small 'pin' icon that is shown when the tab is selected.

## ![ui_tab_text.png][]  Show tab names and icons ##

This button toggles the displaying of the tab names.

## ![expand_sites.png][]  Expand Sites Tab ##

This changes the display so that the 'tree' window containing the Sites tab extends for the full length of the left hand side.
This will reduce the amount of space available to the 'information' window.

## ![expand_info.png][]  Expand Information Tabs ##

This changes the display so that the 'information' window extends for the full length of the bottom.
This will reduce the amount of space available to the 'tree' window.

## ![expand_full.png][]  Full Layout ##

This changes the display so that the selected tab takes up the full screen.
This is useful when using ZAP on small screens.

## ![layout_tabbed.png][]  Request and Response tabs side by side ##

This changes the display so that the request and response tabs are side by side.
This increases the information that can be displayed but means you cannot see both the request and response at the same time.

## ![layout_vertical_split.png][]  Request shown above Response ##

This changes the display so that the request panel is shown above the response panel.
This decreases the information that can be displayed but means you can see both the request and response at the same time.

## ![layout_horizontal_split.png][]  Request and Response panels side by side ##

This changes the display so that the request panel is shown to the left of the response panel.
This decreases the information that can be displayed but means you can see both the request and response at the same time.

## ![152.png][] /  ![151.png][]  Set / Unset break on all requests and responses ##

This sets and unsets a 'global' [break point][] that will trap and display the next request or response in the [Break tab][].
You can then change any part of the request or response that you want to and send it to the target application by pressing either of the 'Step' or 'Continue' buttons.
Alternatively you can press the 'Drop' button to dispose of the request or response.
You can switch between a single 'combined' break button and separates ones for requests and responses via the [Options breakpoints screen][]

## ![105.png][] /  ![105r.png][]  Set / Unset break on all requests ##

This sets and unsets a 'global' [break point][] that will trap and display the next request in the [Break tab][].
You can then change any part of the request that you want to and send it to the target application by pressing either of the 'Step' or 'Continue' buttons.
Alternatively you can press the 'Drop' button to dispose of the request.
You can switch between a single 'combined' break button and separates ones for requests and responses via the [Options breakpoints screen][]

## ![106.png][] /  ![106r.png][]  Set / Unset break on all responses ##

This sets and unsets a 'global' [break point][] that will trap and display the next response in the [Break tab][].
You can then change any part of the response that you want to and send it to your browser by pressing either of the 'Step' or 'Continue' buttons.
Alternatively you can press the 'Drop' button to dispose of the request.
You can switch between a single 'combined' break button and separates ones for requests and responses via the [Options breakpoints screen][]

## ![143.png][]  Step ##

This allows the trapped request or response to continue to the application or your browser with any changes that you have made to it.
The 'global' [break point][] will remain set so that the next request or response will also be caught.
This button is only enabled when a request or response is trapped.

## ![131.png][]  Continue ##

The 'global' [break point][] will be unset so that subsequent requests and responses will no longer be caught by ZAP unless you have set break points on specific URLs.
This button is only enabled when a request or response is trapped.

## ![150.png][]  Drop ##

This drops the trapped request or response so that it is not passed on to the application or your browser.
This button is only enabled when a request or response is trapped.

## ![break_add.png][]  Add a custom HTTP break point ##

This displays the [Add break point][] dialog which allows you to specify the criteria for a [break point][].

## ![block.png][]  Manage Add-ons ##

This shows the [Manage Add-ons][] dialog which allows you to discover, install and update add-ons from the online marketplace.
It also allows you to uninstall add-ons.

## ![forcedUserOff.png][] /  ![forcedUserOn.png][]  Force User Mode On / Off ##

This switches forced user mode on and off.
The button is only enabled when you have defined a forced user for at least one [context][], which can be done via the [Session Contexts][] dialog.

Note that [add-ons][] can add additional buttons.

## See also ##

    [The user interface overview][]


<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartStart" rel="nofollow">Getting Started</a></td>
   <td>for details of how to start using ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpIntro" rel="nofollow">Introduction</a></td>
   <td>the introduction to ZAP</td>
  </tr> 
 </tbody>
</table>


[mode]: HelpStartConceptsModes
[171.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/171.png
[File menu]: HelpUiTlmenuFile
[047.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/047.png
[096.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/096.png
[camera.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/camera.png
[024.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/024.png
[041.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/041.png
[Tools menu]: HelpUiTlmenuTools
[ui-tab-show.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/ui-tab-show.png
[ui-tab-hide.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/ui-tab-hide.png
[ui_tab_text.png]: https://github.com/zaproxy/zap-core-help/wiki/images/ui_tab_text.png
[expand_sites.png]: https://github.com/zaproxy/zap-core-help/wiki/images/expand_sites.png
[expand_info.png]: https://github.com/zaproxy/zap-core-help/wiki/images/expand_info.png
[expand_full.png]: https://github.com/zaproxy/zap-core-help/wiki/images/expand_full.png
[layout_tabbed.png]: https://github.com/zaproxy/zap-core-help/wiki/images/layout_tabbed.png
[layout_vertical_split.png]: https://github.com/zaproxy/zap-core-help/wiki/images/layout_vertical_split.png
[layout_horizontal_split.png]: https://github.com/zaproxy/zap-core-help/wiki/images/layout_horizontal_split.png
[152.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/152.png
[151.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/151.png
[break point]: HelpStartConceptsBreakpoints
[Break tab]: HelpUiTabsBreak
[Options breakpoints screen]: HelpUiDialogsOptionsBreakpoints
[105.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/105.png
[105r.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/105r.png
[106.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/106.png
[106r.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/106r.png
[143.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/143.png
[131.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/131.png
[150.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/150.png
[break_add.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/break_add.png
[Add break point]: HelpUiDialogsAddbreak
[block.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/block.png
[Manage Add-ons]: HelpUiDialogsManageaddons
[forcedUserOff.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/forcedUserOff.png
[forcedUserOn.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/forcedUserOn.png
[context]: HelpStartConceptsContexts
[Session Contexts]: HelpUiDialogsSessionContexts
[add-ons]: HelpStartConceptsAddons
[The user interface overview]: HelpUiOverview