# Scan Progress Dialog #

This shows you the status of an [active scan][].


### Progress tab ###

This shows which scan rules are running for each host being scanned, as well as other details such as the elapsed time they have been running and the number of requests made per rule.
It also allows you to skip the rule which is currently being run by clicking on the 'Skip current running active scan' button ![137.png][] in the Status column.

### Response Chart tab ###

This shows the number of responses per second received by ZAP while active scanning a site.
The responses are charted per 'HTTP response status code group':

 *  1xx Informational
 *  2xx Success
 *  3xx Redirection
 *  4xx Client Error
 *  5xx Server Error

You can zoom in by selecting an area of the chart using your mouse.
You can also right click the chart for more options.
Vertical bars indicate approximately when each scan rule starts (it is very difficult to be precise).
The chart will only be updated while open, if you close and then reopen the chart then the previous data will be lost.
By default the maximum time the chart will cover is 10 minutes, you can change that via the [Options Active Scan screen][].

## Accessed via ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiTabsAscan" rel="nofollow">Active Scan tab</a></td>
   <td></td>
  </tr> 
 </tbody>
</table>

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
   <td> <a href="HelpUiDialogsDialogs" rel="nofollow">Dialogs</a></td>
   <td>for details of the dialogs or popups </td>
  </tr> 
 </tbody>
</table>

## External Links ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="https://en.wikipedia.org/wiki/List_of_HTTP_status_codes" rel="nofollow">https://en.wikipedia.org/wiki/List_of_HTTP_status_codes</a></td>
   <td></td>
  </tr> 
 </tbody>
</table>


[active scan]: HelpStartConceptsAscan
[137.png]: https://github.com/zaproxy/zap-core-help/wiki/images/10/137.png
[Options Active Scan screen]: HelpUiDialogsOptionsAscan