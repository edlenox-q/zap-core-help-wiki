# Options API screen #

This screen allows you to configure the [API][] options:

### Enabled ###

If enabled then the API is available to all machines that are able to use ZAP as a proxy.


### Secure Only ###

If enabled then the API will only be available via HTTPS. Otherwise it will be available via both HTTP and HTTPS.


### API Key ###

A key that must be specified on all API 'actions' and some 'other' operations.
The API key is used to prevent malicious sites from accessing the ZAP API.
It is strongly recommended that you set a key unless you are using ZAP in a completely isolated environment.


### Disable the API Key ###

Selecting this option disables the API key.
This is not recommended unless you are using ZAP in a completely isolated environment, as it allows malicious sites to access the ZAP API.

### Report error details via API ###

If this option is selected then more error details are returned via the API.
This is not recommended except for debugging purposes as these error messages can leak information to malicious sites.
Note that the full error details are always written to the ZAP log file.

### Autofill API key in the API UI ###

If this option is selected then the API key is automatically included in the API UI.
This is not recommended unless you are using ZAP in a completely isolated environment, as it allows malicious sites to access the ZAP API Key.


### Enable JSONP ###

Selecting this option enables the JSONP format.
This can be useful for some applications, but it is generally not recommended as it increases the ZAP attack surface area, ie the features that a malicious site can abuse.
If JSONP is enabled then all API operations using JSONP (including views) will require the API key to prevent malicious sites from accessing sensitive information maintained by ZAP, such as session keys.

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
   <td> <a href="HelpUiDialogsOptionsOptions" rel="nofollow">Options dialogs</a></td>
   <td>for details of the other Options dialog screens</td>
  </tr> 
 </tbody>
</table>


[API]: HelpStartConceptsApi