# Options Active Scan Input Vectors screen #

This screen allows you to configure the [active scan][] input vectors.
These are the elements that the active scanner will attack.
Scanning all of the elements supported will take longer, but not scanning some elements may cause some vulnerabilities to be missed.

### Injectable Targets ###

The request element that the active scanner will target:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>URL Query String</td>
   <td>Key value pairs in the request URL query, ie after the '?'</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>POST Data</td>
   <td>Key value pairs in the request POST data</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>URL Path</td>
   <td>Path elements in the request URL, ie the elements separated by '/'</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>HTTP Headers</td>
   <td>Request HTTP Headers</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Cookie data</td>
   <td>Request cookies</td>
  </tr> 
 </tbody>
</table>

### Build-in Input Vector Handlers ###

The data formats that the active scanner will target:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Multipart Form Data</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>XML tag/attribute</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>JSON</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Google Web Toolkit</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>OData id/filter</td>
   <td></td>
  </tr> 
 </tbody>
</table>

### Enable Script Input Vectors ###

If this option is selected then the active scanner will use any enabled script input vectors.
Script input vectors are scripts which you have written or imported into ZAP and allow you to target elements which are not supported by default.

This screen also allows you to configure the parameters which will be ignored by the active scanner.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsOptionsOptions" rel="nofollow">Options dialogs</a></td>
   <td>for details of the other Options dialog screens</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsOptionsAscaninput" rel="nofollow">Active Scan Input Vectors</a></td>
   <td></td>
  </tr> 
 </tbody>
</table>


[active scan]: HelpStartConceptsAscan