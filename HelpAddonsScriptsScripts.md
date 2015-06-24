# Scripts #

The ZAP Script Add-on allows you to run scripts that can be embedded within ZAP and can access internal ZAP data structures.
It supports any scripting language that supports JSR 223 (http://www.jcp.org/en/jsr/detail?id=223) , including:

 *  ECMAScript / Javascript (included by default)
 *  Zest https://developer.mozilla.org/en-US/docs/zest (included by default)
 *  Groovy http://groovy.codehaus.org/
 *  Python http://www.jython.org
 *  Ruby - http://jruby.org/
 *  and many more...

**WARNING - scripts run with the same permissions as ZAP, so do not run any scripts that you do not trust!**

## Script types ##

Different types of scripts are supported:

 *  Stand Alone - scripts that are self contained and are only run when your start them manually
 *  Active Rules - these run as part of the Active Scanner and can be individually enabled
 *  Passive Rules - these run as part of the Passive Scanner and can be individually enabled
 *  Proxy Rules - these run 'inline', can change every request and response and can be individually enabled. They can also trigger break points
 *  Targeted Rules - scripts that invoked with a target URL and are only run when your start them manually
 *  Authentication - scripts that invoked when authentication is performed for a Context. To be used, they need to be selected when configuring the Script-Based Authentication Method for a Context.
 *  Script Input Vectors - scripts for defining exactly what ZAP should attack

All scripts that are run automatically are initially 'disabled' - you must enable them via the [The Scripts 'tree' tab][The Scripts _tree_ tab] before they will run.
If an error occurs when they run then they will be disabled.
When you select the script then the last error will be shown in the [Script Console tab][].
Targeted scripts can be invoked by right clicking on a record in the Sites or History tabs and selecting the 'Invoke with script...' menu item.

All scripting languages can be used for all script types, but only those languages that have been downloaded from the ZAP Marketplace will typically have templates. However you may well be able to adapt a template for another language.
If your favourite language is not available on the Marketplace then please raise a new issue via the "Online/Report an issue" menu item.
In the meantime you can just place the relevant jars in the 'lib' directory (not the 'plugin' directory) and restart ZAP.


## Global Variables ##

Variables can be shared between all scripts via the class org.zaproxy.zap.extension.script.ScriptVars.
For example in Javascript you can use this class as follows:

`org.zaproxy.zap.extension.script.ScriptVars.setGlobalVar("var.name","value") org.zaproxy.zap.extension.script.ScriptVars.getGlobalVar("var.name")`

## Script Variables ##

Variables can be shared between separate invocations of the same script via the same org.zaproxy.zap.extension.script.ScriptVars class.
For example in Javascript you can use this class as follows:

`org.zaproxy.zap.extension.script.ScriptVars.setScriptVar(this.context, "var.name","value") org.zaproxy.zap.extension.script.ScriptVars.getScriptVar(this.context, "var.name")`
Note that these methods are only usable from scripting languages that provide access to the ScriptContext (like Javascript).

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsScriptsConsole" rel="nofollow">The Script Console tab</a></td>
   <td></td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsScriptsTree" rel="nofollow">The Scripts 'tree' tab</a></td>
   <td></td> 
  </tr> 
 </tbody>
</table>

## External links ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>https://github.com/zaproxy/zaproxy/wiki/InternalDetails</td> 
   <td>ZAP internal objects</td>
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td>https://github.com/zaproxy/zaproxy/wiki/JavaDocs</td> 
   <td>ZAP javadocs</td> 
  </tr> 
 </tbody>
</table>


[The Scripts _tree_ tab]: HelpAddonsScriptsTree
[Script Console tab]: HelpAddonsScriptsConsole