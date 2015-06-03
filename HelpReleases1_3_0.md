# Release 1.3.0 #

The following changes were made in this release:

## Significant changes: ##

### Fuzzing ###

Strings in a response can now be fuzzed to try to find vulnerabilities.
Anti CRSF tokens can be detected and automatically regenerated when fuzzing.
This functionality is based on code from the OWASP JBroFuzz project.

### Dynamic SSL certificates ###

The support for SSL connections was improved and simplified.
User's can now create their own root certificate and distribute this into their HTTP clients.
See [Option: Dynamic SSL Certificates][Option_ Dynamic SSL Certificates] for more details.

### Daemon mode and API ###

Starting ZAP with the "-daemon" command line option will cause it to run in the background in 'headless' mode, meaning that no UI is displayed.
An initial API has been implemented in XML, JSON and HTML.
If ZAP is running as a daemon then the API is automatically enabled, otherwise the API must be enabled via the Options API screen.
The API can be navigated by opening http://zap/ in your browser when proxying via ZAP.

### Beanshell integration ###

The [BeanShell][] is an interactive Java shell that can be used to execute BeanShell scripts.
These scripts are a simplified form of Java that use many elements from Java syntax, but in a simpler scripting format.
All Java code is also valid BeanShell code.
BeanShell integration in OWASP ZAP enables you to write scripts using the ZAP functions and data set.
This can be a very powerful feature for analyzing web applications.


### Full internationalisation ###

All display string are now fully internationalised.

### Localisation ###

Out of the box support for the following languages:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>English</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Brazilian Portuguese</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Chinese</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>French</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>German</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Greek</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Indonesian</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Japanese</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Polish</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Spanish</td>
  </tr> 
 </tbody>
</table>

## Minor changes: ##

### Hex view ###

The [Request][], [Response][] tabs now provide a 'Hex View' option which will display the request and response bodies in hex format.

### Search results ###

The [Search tab ][Search tab] now displays all instances of a string found rather than just the first instance in each request or response.

### Exclude URLs ###

URLs can be explicitly excluded from the active scanner, spider and from the proxy.

### Copy support ###

Most of the panels now provide a 'right click' 'Copy' menu option, including the Port Scan and Brute Force panels.

### Undo/Redo support ###

All of the input fields now support Undo/Redo actions using the operating systems default Undo/Redo accelerators:

 *  Windows/Linux: Ctrl+Z / Ctrl+Y
 *  Mac OS X: Cmd+Z / Cmd+Shift+Z

### Port scanner proxy support and timeout option ###

The Port Scanner can now use the outgoing proxy (if configured) and the timeout in milliseconds can also now be set.

### Request and response break buttons ###

There are now 2 'Set Break' buttons to allow breaks to be set on all requests and all responses independently.

### Expand Sites and Information tab buttons ###

There are now 2 buttons which allow you to switch between having the Sites and Information tabs expanded.

### Break tab icon changes colour when break point hit ###

While the Break tab is not in use its icon is a grey cross:   ![101grey.png][] .
When a [break point][] is hit the tab icon is changed to a red cross:   ![101.png][] .


### Adjustable timeout ###

The [Option: Connection][Option_ Connection] screen allows you to set the timeout in seconds to make it easier to test slow applications.

### Library updates ###

Most of the libraries used by ZAP have been updated to the latest versions.

### A new icon :) ###

Thanks to Simon Egli and all others for submitting cool icon suggestions.

## Known issues: ##

### Mac OS X: Dynamic SSL and Google Chrome ###

Currently Dynamic SSL is not working when using Google Chrome. This is because of an unresolved known issue with Google Chrome and Mac OS X Keychain. When importing OWASP ZAP's Root CA into the keychain and requesting a SSL website, an "Invalid certificate" error message is shown.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpIntro" rel="nofollow">Introduction</a></td>
   <td>the introduction to ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpReleasesReleases" rel="nofollow">Releases</a></td>
   <td>the full set of releases</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpCredits" rel="nofollow">Credits</a></td>
   <td>the people and groups who have made this release possible</td>
  </tr> 
 </tbody>
</table>


[Option_ Dynamic SSL Certificates]: HelpUiDialogsOptionsDynsslcert
[BeanShell]: http://www.beanshell.org/
[Request]: HelpUiTabsRequest
[Response]: HelpUiTabsResponse
[Search tab]: HelpUiTabsSearch
[101grey.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/101grey.png
[break point]: HelpStartConceptsBreakpoints
[101.png]: https://github.com/zaproxy/zap-core-help/wiki/images/16/101.png
[Option_ Connection]: HelpUiDialogsOptionsConnection