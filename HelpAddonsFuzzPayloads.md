# Payloads dialog #

This allows you to select the payload generators to use when [fuzzing][] a request.

Payload generators generate the raw attacks that the fuzzer submits to the target application.

The following types of generators are provided by default:

 *  File - select any local file for one off attacks
 *  File Fuzzers - select any combination of the fuzzing files registered with ZAP, eg via add-ons like fuzzdb
 *  Regex - generate attacks based on regex patterns
 *  Strings - raw strings, which can be entered manually ir pasted in
 *  Script - custom scripts that can generate any payloads required

You can write custom payload generator scripts - these can supply any payloads that you need.

Add-ons can also define additional payload generators.

The 'Processors...' button launches the [Payload Processors dialog][] which allows you to configure payload processors that just apply to the palyload generator you have selected.


## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpAddonsFuzzDialogue" rel="nofollow">Fuzzer dialog</a> 'Add...' button</td>
  </tr> 
 </tbody>
</table>

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpAddonsFuzzConcepts" rel="nofollow">Fuzzer concepts</a></td>
  </tr> 
 </tbody>
</table>


[fuzzing]: HelpAddonsFuzzConcepts
[Payload Processors dialog]: HelpAddonsFuzzProcessors