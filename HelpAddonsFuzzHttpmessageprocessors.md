# HTTP Message Processors #

The HTTP Message Processors can access and change the HTTP messages being fuzzed, control the fuzzing process and interact with the ZAP UI.

Built-in HTTP Message Processors include:

### Anti-CSRF Token Refresher ###

Allows to refresh anti-CSRF tokens contained in the request. The anti-CSRF tokens must be properly detected by ZAP to be able to select and add this processor.
For more information consult the help page "Getting Started" > "Features" > "Anti CSRF Tokens".

### Fuzzer HTTP Processor (Script) ###

Allows to select the enabled Fuzzer HTTP Processor scripts. The scripts allow you to:

 *  Obtain the list of payloads
 *  Stop fuzzing
 *  Increase the error count
 *  Send new messages
 *  Add messages to the Results tab
 *  Set custom ‘state’ messages in the [Fuzzer tab][]
 *  Raise alerts

### Payload Reflection Detector ###

Indicates in the State column of results table if one of the injected payloads were found in the response, using "![reflected_icon.png][] Reflected".

### Request Content-Length Updater ###

Updates (or adds, if not already present) the `Content-Length` request header with the length of the request body, for all request methods. No change is done if the size of the request body is zero and the header is not already present.

### Tag Creator ###

Allows to add custom ‘tags’, based on contents of the response, to the State column of the results table

### User Message Processor ###

Allows to fuzz as a user, using one of the users defined in the contexts that include the HTTP message being fuzzed. Users must exist to be able to select and add this processor.

Other add-ons can define additional HTTP Message Processors.

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpAddonsFuzzDialogue" rel="nofollow">Fuzzer dialog</a> under Message Processors tab</td>
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


[Fuzzer tab]: HelpAddonsFuzzTab
[reflected_icon.png]: https://github.com/zaproxy/zap-core-help/wiki/images/reflected_icon.png