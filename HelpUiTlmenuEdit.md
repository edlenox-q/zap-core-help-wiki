# The Edit menu #

This menu handles finding strings in specific tabs, searching for strings across all requests and responses and managing session tracking.

### Find... ###

This opens the [Find dialog][] which allows you to find a string in the currently selected window.


### Enable Session Tracking (Cookie) ###

This allows session details stored in cookies to be tracked.
This option must be selected to enable the "Use current tracking session" checkbox in the [Resend][] and [Manual Request Editor dialogs][].
Session tracking ensures that any requests are sent with the latest session details.
For example you may record a session when logged in as one user and then logout and login as another user.
If you resend a request from the first session without session tracking then it will use the cookies from the first session.
If you resend the same request with session tracking then it will use the cookies from the second session.

### Reset Session State ###

This clears the session tracking.


### Search... ###

This selects the [Search tab][] which allows you to search for regular expressions in all URLs, requests and responses..

### Next ###

This selects the next occurrence of the last string searched for.
The relevant message will be selected in the Search tab and the string will be displayed and highlighted in the [Request][] or [Response][] tab as appropriate.

### Previous ###

This selects the previous occurrence of the last string searched for.
The relevant message will be selected in the Search tab and the string will be displayed and highlighted in the [Request][] or [Response][] tab as appropriate.

### Encode/Decode/Hash... ###

This displays the [Encode/Decode/Hash dialog][Encode_Decode_Hash dialog].

Note that [add-ons][] can add additional menu items.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiTlmenuTlmenu" rel="nofollow">The top level menu</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
 </tbody>
</table>


[Find dialog]: HelpUiDialogsFind
[Resend]: HelpUiDialogsResend
[Manual Request Editor dialogs]: HelpUiDialogsMan_req
[Search tab]: HelpUiTabsSearch
[Request]: HelpUiTabsRequest
[Response]: HelpUiTabsResponse
[Encode_Decode_Hash dialog]: HelpUiDialogsEnc_dec
[add-ons]: HelpStartConceptsAddons