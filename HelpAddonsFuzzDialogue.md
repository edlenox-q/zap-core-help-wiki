# Fuzzer dialog #

This allows you to select the fuzzers to use when [fuzzing ][fuzzing] a request.

### Fuzz Locations tab ###

To configure the fuzzing:


 *  Highlight a string you wish to fuzz in the Fuzz Locations tab
 *  Click the 'Add...' button to launch the [Payloads dialog][]
 *  Add the payloads you want to use
 *  Click on the 'Processors...' button to launch the [Location Processors dialog][] (if required)
 *  Click on the 'Start Fuzzer' button to start the fuzzing
 *  The results will then be listed in the [Fuzzer tab][] select them to see the full requests and responses.

You can also search for strings in the fuzz results using the 'Search tab'.

### Options tab ###

This tab allows you to configure the options to be used when fuzzing.

### Message Processors tab ###

Message Processors can access and change the messages being fuzzed, control the fuzzing process and interact with the ZAP UI.
The message processors available depend on the type of message being fuzzed, this add-on includes the [default HTTP Messages processors][].

Add-ons can also define additional payload generators.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Request tab</td>
   <td>'Fuzz...' right click menu item</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Sites and History tab</td>
   <td>Attack &gt; Fuzz... menu items</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Tools menu </td>
   <td>Attack &gt; Fuzz... menu item</td>
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
[Payloads dialog]: HelpAddonsFuzzPayloads
[Location Processors dialog]: HelpAddonsFuzzLocations
[Fuzzer tab]: HelpAddonsFuzzTab
[default HTTP Messages processors]: HelpAddonsFuzzHttpmessageprocessors