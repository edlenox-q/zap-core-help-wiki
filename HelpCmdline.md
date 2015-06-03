# Command Line #

ZAP supports the following command line options:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-cmd</td>
   <td>Runs ZAP 'inline', ie without starting the UI or a daemon</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-config</td>
   <td>Overrides the specified key=value pair in the configuration file</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-daemon</td>
   <td>Starts ZAP in 'daemon' mode, ie without a UI</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-dir</td>
   <td>Uses the specified directory instead of the default one</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-installdir</td>
   <td>Overrides the code that detects where ZAP has been installed with the specified directory</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-h</td>
   <td>Shows all of the command line options available, including those added by add-ons</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-help</td>
   <td>The same as -h </td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-host</td>
   <td>Overrides the host used for proxying specified in the configuration file</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-port</td>
   <td>Overrides the port used for proxying specified in the configuration file</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-version</td>
   <td>Reports the ZAP version</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-newsession</td>
   <td>Creates a new session at the given location (it expects the full path to the session)</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>-session</td>
   <td>Opens the given session after starting ZAP (it expects the full path to the session).</td>
  </tr> 
 </tbody>
</table>


The options '-session' and '-newsession' are mutually exclusive. An error will be shown and ZAP exit (if not in GUI) when both options are set.
Configuration keys should be specified using the dot notation based their location in the XML of the configuration file, eg:


``````````
-config api.key=12345 -config connection.timeoutInSecs=60
``````````

Note that add-ons can add extra command line options.

Examples:

 *  Start ZAP in 'daemon' mode with a new session created at a given path:
    
    ``````````
    -daemon -newsession /path/to/new/session
    ``````````
 *  Create a report of the last scan of an existing session and exit ZAP once finished:
    
    ``````````
    -last_scan_report /path/to/save/report.xml -session /path/to/existing/session -cmd
    ``````````

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
   <td> <a href="HelpStartConceptsApi" rel="nofollow">API</a></td>
   <td>to control ZAP programmatically</td>
  </tr> 
 </tbody>
</table>