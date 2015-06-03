# Options Active Scan screen #

This screen allows you to configure the [active scan][] options:

### Number of hosts scanned concurrently ###

The maximum number of hosts that will be scanned at the same time. Increasing this may put extra strain on the computer ZAP is running on.

### Concurrent scanning threads per host ###

The number of threads the scanner will use per host.
Increasing the number of threads will speed up the scan but may put extra strain on the computer ZAP is running on and the target host.

### Max results to list ###

The number of results that will be shown in the Active Scan tab.
Displaying a large number of results can significantly increase the time a scan takes.

### Delay when scanning in milliseconds ###

The delay in milliseconds between each request.
Setting this to a non zero value will increase the time an active scan takes, but will put less of a strain on the target host.

### Handle anti CSRF tokens ###

If this option is selected then the active scanner will attempt to automatically request [anti CSRF][] tokens when required.
Note that this is experimental functionality and will slow down the scanning process as only one thread will be used to ensure that anti CSRF token requests dont get out of step.

### In Attack mode prompt to rescan nodes when scope changed ###

If this option is selected then when you select Attack [mode][] you will be prompted to choose whether to rescan nodes in scope.
If the option is not selected then the following option will control whether the nodes are rescanned.

### In Attack mode always rescan nodes when scope changed ###

If this option is selected then when running in Attack [mode][] all nodes in scope will be rescanned if the scope changes.
This is not recommended for large sites as it could take a long time.

### Default active scan policy ###

The [Scan Policy][] that is used by default when you start an active scan.

### Attack mode scan policy ###

The [Scan Policy][] that is used for scanning in Attack [mode][].

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
   <td><a href="HelpUiDialogsOptionsAscan" rel="nofollow">Active Scan options</a></td>
   <td></td>
  </tr> 
 </tbody>
</table>


[active scan]: HelpStartConceptsAscan
[anti CSRF]: HelpStartConceptsAnticsrf
[mode]: HelpStartConceptsModes
[Scan Policy]: HelpStartConceptsScanpolicy