# Break tab #

The Break tab allows you to change a request or response when it has been caught by ZAP via a [break point][].
It allows you to change elements that you would not normally be able to change via your browser, including:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The header</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Hidden fields</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Disabled fields</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Fields that use javascript to filter out illegal characters</td>
  </tr> 
 </tbody>
</table>

This functionality is key to effectively pen testing your application.

The 2 panels will only contain anything if ZAP has caught a request or response.
You can change anything in these 2 panels and then forward the request or response using the buttons on the [Top Level Toolbar][].

Pull downs allow you to select different [Views][] for the request or response header and body.

While the Break tab is not in use its icon is a grey cross:   ![101grey.png][] .
When a [break point][] is hit the tab icon is changed to a red cross:   ![101.png][] .


## Right click menu ##

Right clicking on a node will bring up a menu which will allow you to:

### Find... ###

This will bring up the [Find dialog][].

### Encode/Decode/Hash... ###

This will bring up the [Encode/Decode/Hash dialog][Encode_Decode_Hash dialog].
If you have highlighted any text then this will be automatically included in the dialog.

### Copy ###

This will copy the selected string to the clipboard.

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
   <td> <a href="HelpUiTabsBreakpoints" rel="nofollow">Break Points tab</a></td>
   <td>for details of how to change or delete break points</td>
  </tr> 
 </tbody>
</table>


[break point]: HelpStartConceptsBreakpoints
[Top Level Toolbar]: HelpUiTltoolbar
[Views]: HelpUiViews
[101grey.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/101grey.png
[101.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/101.png
[Find dialog]: HelpUiDialogsFind
[Encode_Decode_Hash dialog]: HelpUiDialogsEnc_dec