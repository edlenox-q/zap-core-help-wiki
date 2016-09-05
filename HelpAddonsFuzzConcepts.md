# Fuzzing #

Fuzzing is a technique of submitting lots of invalid or unexpected data to a target.

ZAP allows you to fuzz any request still using:

 *  A build in set of payloads
 *  Payloads defined by optional add-ons
 *  Custom scripts

To access the [Fuzzer dialog][] you can either:

 *  Right click a request in one of the ZAP tabs (such as the History or Sites) and select “Attack / Fuzz…”
 *  Highlight a string in the Request tab, right click it and select “Fuzz…”
 *  Select the “Tools / Fuzz…” menu item and then select the request you want to fuzz

### Payload Generators ###

Payload Generators generate the raw attacks that the fuzzer submits to the target application.

They are managed via the [Payloads dialog][]

### Payload Processors ###

Payload Processors can be used to change specific payloads before they are submitted.

They are managed via the [Payload Processors dialog][]

### Fuzz Location Processors ###

Fuzz Location Processors can be used to change all of the payloads before they are submitted.

They are managed via the [Location Processors dialog][]

### Message Processors ###

Message Processors can access and change the messages being fuzzed, control the fuzzing process and interact with the ZAP UI.

They are managed via the [Fuzzer dialog][] 'Message Processors' tab.

This functionality is based on code from the OWASP JBroFuzz project and includes files from the fuzzdb project.
Note that some fuzzdb files have been left out as they cause common anti virus scanners to flag them as containing viruses.
You can replace them (and upgrade fuzzdb) by downloading the latest version of fuzzdb and expanding it in the 'fuzzers' library.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpAddonsFuzzOptions" rel="nofollow">Fuzzer options screen</a></td>
  </tr> 
 </tbody>
</table>


[Fuzzer dialog]: HelpAddonsFuzzDialogue
[Payloads dialog]: HelpAddonsFuzzPayloads
[Payload Processors dialog]: HelpAddonsFuzzProcessors
[Location Processors dialog]: HelpAddonsFuzzLocations