# Statistics #

ZAP maintains statistics which can help you understand what is really happening when interacting with large applications.

The statistics are available via the [API][] and can be also sent to a Statsd server when configured via the [Options Statistics screen][].

### Site based statistics ###

Statistics maintained on a per site basis include:

 *  response codes, eg:
    
     *  stats.code.200
     *  stats.code.302
 *  response times in ms (using a logarithmic scale), eg:
    
     *  stats.responseTime.1
     *  stats.responseTime.2
     *  stats.responseTime.4
     *  stats.responseTime.8
     *  stats.responseTime.16
 *  content types, eg:
    
     *  stats.contentType.text/css
     *  stats.contentType.text/html;charset=utf-8
 *  [tags][], eg:
    
     *  stats.tag.Password
     *  stats.tag.Hidden
 *  anticsrf tokens generated:
    
     *  stats.acsrf.anticsrf
 *  authentication info:
    
     *  stats.auth.success (number of authentication successes)
     *  stats.auth.failure (number of authentication failures)
     *  stats.auth.state.loggedin (number of responses that appear to be logged in)
     *  stats.auth.state.loggedout (number of responses that appear to be logged out)
     *  stats.auth.state.noindicator (number of responses where no logged in or out indicators have been set)
     *  stats.auth.state.unknown (number of responses which don't contain either logged in or out indicators)

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
   <td><a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td>
   <td>provided by ZAP</td>
  </tr> 
 </tbody>
</table>


[API]: HelpStartConceptsApi
[Options Statistics screen]: HelpUiDialogsOptionsStats
[tags]: HelpStartConceptsTags