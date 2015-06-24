# Options Applications screen #

This screen allows you to configure the [applications][] that can be invoked.
By default there are no applications available, you need to add all of the applications that you want to use.

### Display Name ###

The name that will be used for this application in ZAP.


### Full Command ###

The full path of the application you want to invoke.
Only one command can be specified. If you want to run multiple commands in one go, or set up environmental variables, then you should create a script or batch file and then invoke this from ZAP.

### Parameters ###

The parameters that ZAP should pass to the command.
The following tags may be used to pass parameters:

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>%url%</td> 
   <td>the full url, e.g. 'http://localhost/test?a=b'</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>%site%</td> 
   <td>the site, e.g. 'http://localhost:8080/'</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>%host%</td> 
   <td>the hostname, e.g. 'localhost'</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>%port%</td> 
   <td>the port, e.g. '80'</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>%cookie%</td> 
   <td>the first cookie field from the request header (if any)</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>%postdata%</td> 
   <td>the POST data sent, if any, with any newlines replaced with &quot;\n&quot;</td> 
  </tr> 
 </tbody>
</table>

So if a command accepted a URL using '-u' you would specify the parameters as: '-u %url%'

### Capture Output ###

If checked then the command run and any output it generates will be displayed on the *Output tab*.
You should always use this options when running scripts or commands that do not have a UI.
You can also use this options for troubleshooting - if an application does not run as expected then copy the command run and try it from a command line prompt.

### Output to Note ###

If checked then any output will be appended to a *Note* attached to the relevant *History tab* record.
Note that some nodes in the *Sites tab* do not have associated *History tab* records - for those nodes this option will have no effect.


[applications]: HelpAddonsInvokeConcepts