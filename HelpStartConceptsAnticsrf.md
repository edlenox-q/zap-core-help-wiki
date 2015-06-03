# Anti CSRF Tokens #

Anti CSRF tokens are (pseudo) random parameters used to protect against Cross Site Request Forgery (CSRF) attacks.
However they also make a penetration testers job harder, especially if the tokens are regenerated every time a form is requested.


ZAP detects anti CSRF tokens purely by attribute names - the list of attribute names considered to be anti CSRF tokens is configured using the [Options Anti CSRF screen][].
When ZAP detects these tokens it records the token value and which URL generated the token.
Other scanners, like [active scanner][], have options which cause ZAP to automatically regenerate the tokens when required.

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


[Options Anti CSRF screen]: HelpUiDialogsOptionsAnticsrf
[active scanner]: HelpStartConceptsAscan