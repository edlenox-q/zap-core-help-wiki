# Fuzzer tab #

The Fuzzer tab shows you the requests and responses performed when you [fuzz][] a string.
Selecting a row see the full requests and responses. You can also search for strings in the fuzz results using the Search tab.


## HTTP Fuzzer results ##

The results have to be manually assessed to know if any vulnerability was found.
Meaning of values of the "State" column:

 *  "Error" - an error occurred while creating or sending/receiving the message (for example: malformed HTTP message, time out while reading the response)
 *  "Reflected" - the injected fuzz string (value of "Fuzz" column) was found in the response body.

If this field is blank then it means that the message was successfully sent/received and the injected string was not detected in the response.


## Right click menu ##

Right clicking on a row will bring up a menu which has the same options as the History tab.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpAddonsFuzzConcepts" rel="nofollow">Fuzzer concepts</a></td>
  </tr> 
 </tbody>
</table>


[fuzz]: HelpAddonsFuzzConcepts