# Params tab #

This shows a summary of the parameters a site uses.

Sites can be selected via the toolbar or the [Sites tab][].
For each parameter you can see:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The type - Cookie, FORM or URL</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The name of the parameter</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The number of times it has been used</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The number of unique values</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The percentage change, where 0 means only one value has been used and 100 means all values are unique</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>The flags - including cookie flags and anticsrf and session</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>Some of the values - the full set of values may not all be visible</td>
  </tr> 
 </tbody>
</table>

## Right click menu ##

Right clicking on a node will bring up a menu which will allow you to:

### Search ###

This will show all examples of the parameter selected in the [Search tab][].

### Flag as Anti CSRF token ###

This will flag the parameter as an [Anti CSRF token][].

### Unflag as Anti CSRF token ###

This will remove the Anti CSRF token flag from the parameter.


### Flag as Session token ###

This will mark the parameter as a Session token for the current Site and will notify the [HTTP Sessions][] tool accordingly.


### Unflag as Session token ###

This will unmark the parameter as a Session token for the current site and will notify the [HTTP Sessions][] tool accordingly.


## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
 </tbody>
</table>


[Sites tab]: HelpUiTabsSites
[Search tab]: HelpUiTabsSearch
[Anti CSRF token]: HelpStartConceptsAnticsrf
[HTTP Sessions]: HelpStartConceptsHttpsessions