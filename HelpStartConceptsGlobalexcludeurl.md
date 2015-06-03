# Globally Excluded URLs #

*Note: this feature is beta.*

Globally Excluded URLs are a set of Regular Expressions (regex) that ZAP ignores completely throughout the application. These URLs will not show up in the Proxy, Scanner, or Spider for ZAP. In addition, the URL regexs will be saved in the global configuration for ZAP and not inside of the session file. These URLs will persist between each use of ZAP.

The regex for URLs are configured using the [Global Exclude URL screen][] in the ZAP Options.

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


[Global Exclude URL screen]: HelpUiDialogsOptionsGlobalexcludeurl