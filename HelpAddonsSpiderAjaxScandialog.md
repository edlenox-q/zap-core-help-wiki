# AJAX Spider dialog #

This dialog launches the AJAX Spider.

## Scope ##

The first tab allows you to change key features like:

### Starting point ###

The URL which the AJAX spider will start crawling from, or a context (in which case it will be used one of the URLs that are in context as starting point).

### Context ###

Allows to select the Context to be spidered.

### User ###

Allows to select one of the users available from the selected context, to perform the spider scan as a user (ZAP will (re)authenticate as that user whenever necessary).

### Just in scope ###

If set then any URLs which are out of scope will be ignored.

**Note:** The option `Just in scope` is mutually exclusive with `Context` option, if one is used the other is ignored.

### Spider Subtree Only ###

If set then the spider will only access resources that are under the starting point (URI). When evaluating if a resource is found within the specified subtree, the spider considers only the scheme, host, port, and path components of the URI.

### Browser ###

The type of browser to use.
Browsers will only be shown if ZAP has sufficient configuration to run them.
They may still fail to run if the browsers cannot be found or if the configuration information is incorrect.

### Show advanced options ###

If selected then the Options tab will be shown.

## Options ##

This tab allows you to change options including:

### Number of browser windows to open ###

You can configure the number of windows to be used by AJAX Spider.
The more windows, the faster the process will be.

### Maximum crawl depth ###

The maximum depth that the crawler can reach. Zero means unlimited depth.

### Maximum crawl states ###

The maximum number of states that the crawler should crawl. Zero means unlimited crawl states.

### Maximum duration ###

The maximum time that the crawler is allowed to run. Zero means unlimited running time.

### Event wait time ###

The time to wait after a client side event is fired.

### Reload wait time ###

The time to wait after URL is loaded.

## See also ##

<table> 
 <tbody>
  <tr>
    &nbsp;&nbsp;&nbsp;&nbsp; 
   <td><a href="HelpAddonsSpiderAjaxConcepts" rel="nofollow">AJAX Spider</a></td> 
   <td>for an overview of the AJAX Spider</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsSpiderAjaxTab" rel="nofollow">AJAX Spider tab</a></td> 
   <td>for an overview of the AJAX Spider Tab</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsSpiderAjaxOptions" rel="nofollow">Options AJAX Spider screen</a></td> 
   <td>for an overview of the AJAX Spider Options</td> 
  </tr> 
 </tbody>
</table>