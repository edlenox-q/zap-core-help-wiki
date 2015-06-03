# Scope #

The Scope is the set of URLs you are testing, and is defined by the [Contexts][] you have specified.

By default nothing is in scope.

The Scope potentially changes:

 *  What you can do, when you are in Protected [mode][]
 *  What is shown in the [History tab][]
 *  Protected - user can only perform (potentially) dangerous actions on URLs in the Scope
 *  Standard - as in previous releases, user can do anything
 *  ATTACK - new nodes that are in Scope are [actively scanned][] as soon as they are discovered

It is recommended that you define a new [Context][Contexts] for each web application that makes up the system you are testing, and set them in scope as you test each one.

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


[Contexts]: HelpStartConceptsContexts
[mode]: HelpStartConceptsModes
[History tab]: HelpUiTabsHistory
[actively scanned]: HelpStartConceptsAscan