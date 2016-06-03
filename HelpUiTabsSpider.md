# Spider tab #

The Spider tab shows you the set of unique URIs found by the [Spider][] during the scans.

The 'New Scan' button launches the [Spider dialog][] which allows you to specify exactly what should be scanned.
The Spider can be run on multiple Sites in parallel and the results for each scan are shown by selecting the scan via the 'Progress' pull-down.

The toolbar shows information about a scan and allows to control it. It provides a set of buttons which allows to:

 *  ![pause button][] Pause (and ![resume button][] resume) the selected spider scan;
 *  ![stop button][] Stop the selected spider scan;
 *  ![clean scans button][] Clean completed scans;
 *  ![show messages button][] Show/Hide Messages - shows/hides a tab (called Messages) that displays all HTTP messages sent by the selected spider scan;
 *  ![spider options button][] Open the [Spider Options screen][].

The progress bar shows how far the selected spider scan has progressed. It is also shown the number of active spider scans and the number of URIs found for the selected scan.

For each URI found you can see:

 *  Processed - Whether the URI was processed by the Spider or was skipped from fetching because of a rule (e.g. it was out of scope)
 *  Method - The HTTP method, e.g. GET or POST, through which the resource should be accessed
 *  URI - the resource found
 *  Flags - any information about the URI (e.g. if it's a seed or why was it not processed)

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
   <td><a href="HelpStartConceptsSpider" rel="nofollow">Spider</a></td> 
   <td>for an overview of the Spider</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsOptionsSpider" rel="nofollow">Spider Options screen</a></td> 
   <td>for an overview of the Spider Options</td> 
  </tr> 
 </tbody>
</table>


[Spider]: HelpStartConceptsSpider
[Spider dialog]: HelpUiDialogsSpider
[pause button]: https://github.com/zaproxy/zap-core-help/wiki/images/16/141.png
[resume button]: https://github.com/zaproxy/zap-core-help/wiki/images/16/131.png
[stop button]: https://github.com/zaproxy/zap-core-help/wiki/images/16/142.png
[clean scans button]: https://github.com/zaproxy/zap-core-help/wiki/images/fugue/broom.png
[show messages button]: https://github.com/zaproxy/zap-core-help/wiki/images/16/178.png
[spider options button]: https://github.com/zaproxy/zap-core-help/wiki/images/16/041.png
[Spider Options screen]: HelpUiDialogsOptionsSpider