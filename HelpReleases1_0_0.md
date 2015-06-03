# Release 1.0.0 #

The following changes were made in this release:

## Significant changes: ##

### Help screens ###

Help screens have been added for all of the functionality now provided by ZAP.
Context sensitive help has also been implemented so that when you press the F1 key then the help screen associated with the tab you have selected will be displayed.

### Break Points ###

The implementation of [Break Points][] has been changed to be closer to that provided by software Integrated Development Environments.
The break point controls have been moved to the new [Top Level Toolbar][].
Break points can now also be set by right clicking nodes in the [Sites][] and [History tabs][].

### Report menu ###

The [Report Menu][] has been significant changed and now includes the following menu items:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Generate Report...</td>
   <td>Which now generates reports on demand</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Export Messages to File...</td>
   <td>Moved from the <a href="HelpUiTlmenuFile" rel="nofollow">File Menu</a></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Export Response to File...</td>
   <td>Moved from the <a href="HelpUiTlmenuFile" rel="nofollow">File Menu</a></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Export ALL URLs to File...</td>
   <td>New functionality</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Compare with another session...</td>
   <td>New functionality</td>
  </tr> 
 </tbody>
</table>

### Improved history searching ###

The new [Search tab][] allows you to search for regular expressions in all of the URLs, requests and responses.
Next and previous buttons allow you view the found search terms in the [Request][] and [Response tabs][].


### History filter ###

[The History Filter Toolbar][History tabs] has been added which allows you to restrict which requests are displayed.
Requests can be filtered based on the HTTP methods, the HTTP result codes, and any [tags][], [alerts][], or [notes][] that have been applied.

### Notes ###

You can now associate [notes][] with any request.

### Multiple Tags ###

You can now associate multiple [tags][] with any request.

### More control over the alerts ###

The [Add Alert dialog][] allows you to manually add or change an alert.

### New encoder/decoder ###

A new [Encode/Decode/Hash dialog][Encode_Decode_Hash dialog] has replaced the previous Encoder/Decoder.

### Passive scanning ###

[Passive scanning][] has been added.
In this release ZAP will only use passive scanning for automatically adding [tags][].
In future releases it may also raise [alerts][] for potential issues.

## Minor changes: ##

### The Top Level Toolbar ###

[The Top Level Toolbar][Top Level Toolbar] has been added which provides a set up buttons for commonly used functionality.

### Alert footer summaries ###

Counts of the High, Medium, Low and Informational [alerts][] are now displayed in the [footer][].

### New look and feel ###

A new look and feel 'Nimbus' is used.

### Proxy password handling ###

[The Options Connection screen][] has a new option to 'Prompt for proxy credentials on start up'.
If this option is selected then your proxy password will not be stored on the hard disk.

### Resend from the Sites tab ###

The [Sites tab][Sites] has a new right click menu item that allows you to resend the request after making any changes to it that you want to.

### User directory maintained between sessions ###

The last directory used by the user is now stored in the config file so that it is maintained between sessions.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpIntro" rel="nofollow">Introduction</a></td>
   <td>the introduction to ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpReleasesReleases" rel="nofollow">Releases</a></td>
   <td>the full set of releases</td>
  </tr> 
 </tbody>
</table>


[Break Points]: HelpStartConceptsBreakpoints
[Top Level Toolbar]: HelpUiTltoolbar
[Sites]: HelpUiTabsSites
[History tabs]: HelpUiTabsHistory
[Report Menu]: HelpUiTlmenuReport
[Search tab]: HelpUiTabsSearch
[Request]: HelpUiTabsRequest
[Response tabs]: HelpUiTabsResponse
[tags]: HelpStartConceptsTags
[alerts]: HelpStartConceptsAlerts
[notes]: HelpStartConceptsNotes
[Add Alert dialog]: HelpUiDialogsAddalert
[Encode_Decode_Hash dialog]: HelpUiDialogsEnc_dec
[Passive scanning]: HelpStartConceptsPscan
[footer]: HelpUiFooter
[The Options Connection screen]: HelpUiDialogsOptionsConnection