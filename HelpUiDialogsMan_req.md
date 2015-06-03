# Manual Request Editor dialog #

This dialog allows you to create a request from scratch which will be submitted to the specified target.

## Request tab ##

This shows the request header and data, either in one or two panels depending on the options chosen.

A 'Method' pull down allows you to switch between the HTTP methods.
Note that when the method is changed to a POST then any URL parameters are moved into the body, and when the method is changed from a POST then any parameters in the body are moved to the URL.

Pull downs allow you to select different [Views][] for the Request header and body.

### ![view_split.png][]  Split display for header and body ###

This changes the display so that separate panes are used for the header and body.


### ![view_all.png][]  Combined display for header and body ###

This changes the display so that the header and body are shown in one pane.


### ![cookie.png][]  Use current tracking session ###

See the 'Enable session tracking (Cookie)' menu item in the [Edit menu][].


### ![118.png][]  Follow redirect ###

If selected automatically follows any redirects sent to the browser.


### ![layout_tabbed.png][]  Request and Response tabs side by side ###

This changes the display so that the request and response tabs are side by side.
This increases the information that can be displayed but means you cannot see both the request and response at the same time.

### ![layout_vertical_split.png][]  Request shown above Response ###

This changes the display so that the request panel is shown above the response panel.
This decreases the information that can be displayed but means you can see both the request and response at the same time.

### ![layout_horizontal_split.png][]  Request and Response panels side by side ###

This changes the display so that the request panel is shown to the left of the response panel.
This decreases the information that can be displayed but means you can see both the request and response at the same time.

## Response tab ##

This shows the data sent to your browser in response to the request that you submitted, either in one or two panels depending on the options chosen.

Pull downs allow you to select different [Views][] for the Response header and body.

## Right click menu ##

Right clicking will bring up a menu which will allow you to:

### Find... ###

This will bring up the [Find dialog][].

### Encode/Decode... ###

This will bring up the [Encode/Decode dialog][Encode_Decode dialog].
If you have highlighted any text then this will be automatically included in the dialog.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTlmenuTools" rel="nofollow">Top level Tools menu</a></td>
   <td>'Manual Request Editor ...' menu item</td>
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


[Views]: HelpUiViews
[view_split.png]: https://github.com/zaproxy/zap-core-help/wiki/images/view_split.png
[view_all.png]: https://github.com/zaproxy/zap-core-help/wiki/images/view_all.png
[cookie.png]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/cookie.png
[Edit menu]: HelpUiTlmenuEdit
[118.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/118.png
[layout_tabbed.png]: https://github.com/zaproxy/zap-core-help/wiki/images/layout_tabbed.png
[layout_vertical_split.png]: https://github.com/zaproxy/zap-core-help/wiki/images/layout_vertical_split.png
[layout_horizontal_split.png]: https://github.com/zaproxy/zap-core-help/wiki/images/layout_horizontal_split.png
[Find dialog]: HelpUiDialogsFind
[Encode_Decode dialog]: HelpUiDialogsEnc_dec