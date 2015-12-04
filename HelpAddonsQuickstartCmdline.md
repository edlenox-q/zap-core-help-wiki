# Command Line #

Quick Start add-on supports the following command line options:

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>-quickurl</td> 
   <td>Specifies the URL of the target application that will be attacked.</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>-quickout</td> 
   <td>Specifies the file to write the XML report to. If not set in 'inline' and daemon modes the report is written to default output stream.</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>-quickprogress</td> 
   <td>Show ascii progress bars, if started with the -cmd flag.</td> 
  </tr> 
 </tbody>
</table>


Examples:

 *  Start ZAP in 'inline' mode with ascii progress bars, attack the target application http://example.com/ and write the report to default output stream:
    
    ``````````
    -cmd -quickurl http://example.com/ -quickprogress
    ``````````
 *  Start ZAP with UI, attack the target application http://example.com/ and save the report to a file:
    
    ``````````
    -quickurl http://example.com/ -quickout /path/to/report.xml
    ``````````

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsQuickstartQuickstart" rel="nofollow">Quick Start</a></td> 
   <td>the introduction to Quick Start</td> 
  </tr> 
 </tbody>
</table>