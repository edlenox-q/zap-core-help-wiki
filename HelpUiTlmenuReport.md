# The Report menu #

This menu handles the reports.

### Generate HTML Report ... ###

This generates a new HTML report containing the alerts raised.

### Generate XML Report ... ###

This generates a new XML report containing the alerts raised.

### Export Messages to File... ###

This allows you to save requests and responses to a text file.
Select the messages to save in the History tab - use the shift key to select multiple messages.

### Export Response to File... ###

This allows you to save a specific response to a file.
Select the relevant message in the History tab - note that binary responses (such as images) can be saved as well as test responses.

### Export All URLs to File... ###

This allows you to save all of the URLs accessed to a text or HTML file.
The URLs will be preceded by the HTTP method used.
This can be used, amongst other things, to compare the URLs available to users with different roles or permissions on the same system.

### Compare with another Session... ###

This prompts you for a ZAP session that you have previously saved.
It then prompts you for an output file into which is written all of the URLs accessed by the current session and the session you have selected to compare it with.
The file will contain a table listing the URLs and the HTTP responses for the URLs in the 2 sessions.
JavaScript buttons allow you to display all of the URLs, just those accessed in the first session, the second session and those accessed by both sessions.
This is particularly useful for comparing 2 sessions which access the same application using different users. You will be able to see which URLs are visible to the users and will be able to try to access all of the URLs when logged in as either of the users.

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


[add-ons]: HelpStartConceptsAddons