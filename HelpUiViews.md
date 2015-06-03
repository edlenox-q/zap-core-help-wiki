# Views #

ZAP provides a set of plugable views which allows you to display the requests and responses in different ways.
The following views are included by default:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Text</td>
   <td>The data in text format</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Hex</td>
   <td>A table showing the hex representation of all of the characters in the header and body. <br /> For editable screens this allows you to add control characters via their hex codes.<br /> You cannot add or delete characters in this view - to do that switch to one of the other views and then back to carry on in hex view.</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Image</td>
   <td>The image - only available for bodys containing images</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Table</td>
   <td>A table with one row per attribute and value.<br /> For editable screens all values will automatically be URL encoded when they are submitted. </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Table (adv)</td>
   <td>A table with one row per attribute and value plus additional functions.<br /> For editable screens values will not be automatically be URL encoded when they are submitted, but this can be done 'manually' via 'URLEncode' function. </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Large Request</td>
   <td>A placeholder view used to prevent the UI trying to load a very large request body.<br /> You will need to switch to a different view to display the actual contents.<br /> The threshold for the view can be changed via the <a href="HelpUiDialogsOptionsView" rel="nofollow">Display Options screen</a></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Large Response</td>
   <td>A placeholder view used to prevent the UI trying to load a very large response body.<br /> You will need to switch to a different view to display the actual contents.<br /> The threshold for the view can be changed via the <a href="HelpUiDialogsOptionsView" rel="nofollow">Display Options screen</a></td>
  </tr> 
 </tbody>
</table>

Note that [add-ons][] can add additional views.

## Used in ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsBreak" rel="nofollow">Break tab</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsRequest" rel="nofollow">Request tab</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsResponse" rel="nofollow">Response tab</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsMan_req" rel="nofollow">Manual Request dialog</a></td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsResend" rel="nofollow">Resend dialog</a></td>
   <td></td>
  </tr> 
 </tbody>
</table>

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
 </tbody>
</table>


[add-ons]: HelpStartConceptsAddons