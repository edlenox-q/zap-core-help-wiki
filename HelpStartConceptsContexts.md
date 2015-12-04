# Contexts #

Contexts are a way of relating a set of URLs together.
You can define any contexts you like, but it is expected that a context will correspond to a web application.
It is recommended that you define a new contexts for each web application that makes up the system you are testing, and set them in scope as you test each one.

Contexts are defined as a set of regular expressions (regexs) which are applied to all of the URLs in the [Sites tab][].
You can configure contexts via:

 *  Right click menu items in the in the Sites or History tab
 *  The [Session Contexts dialogs][].

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
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpStartConceptsStructmods" rel="nofollow">Structural Modifiers</a></td>
   <td>controls which change how ZAP represents the structure of the application</td>
  </tr> 
 </tbody>
</table>


[Sites tab]: HelpUiTabsSites
[Session Contexts dialogs]: HelpUiDialogsSessionContexts