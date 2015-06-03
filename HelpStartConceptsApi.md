# API #

ZAP provides an Application Programming Interface (API) which allows you to interact with ZAP programmatically.

The API is available in JSON, HTML and XML formats.
The API documentation is available via the URL http://zap/ when you are proxying via ZAP.


It should be noted that there is minimal security built into the API, which is why it is disabled by default.
If enabled then the API is available to all machines that are able to use ZAP as a proxy.
By default ZAP listens only on 'localhost' and so can only be used from the host machine.

The API provides access to the core ZAP features such as the [active scanner][] and [spider][].
Future versions of ZAP will increase the functionality available via the APi.

The API is configured using the [Options API screen][].

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
   <td> <a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td>
   <td>provided by ZAP</td>
  </tr> 
 </tbody>
</table>


[active scanner]: HelpStartConceptsAscan
[spider]: HelpStartConceptsSpider
[Options API screen]: HelpUiDialogsOptionsApi