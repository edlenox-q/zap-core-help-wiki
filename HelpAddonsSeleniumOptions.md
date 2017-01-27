# Options Selenium screen #

This screen allows you to setup the requirements of some of the WebDrivers.


## Configuration option explanation ##

<table> 
 <tbody>
  <tr> 
   <th colspan="3">Configuration Options</th> 
  </tr> 
  <tr> 
   <th>Field</th> 
   <th>Details</th> 
   <th>Default</th> 
  </tr> 
  <tr> 
   <th colspan="3">WebDrivers</th> 
  </tr> 
  <tr> 
   <td>ChromeDriver</td> 
   <td>This allows you to select the location of ChromeDriver.</td> 
   <td align="center">The path to the bundled WebDriver, if available.</td> 
  </tr> 
  <tr> 
   <td>geckodriver</td> 
   <td>This allows you to select the location of geckodriver (Firefox driver).</td> 
   <td align="center">The path to the bundled WebDriver, if available.</td> 
  </tr> 
  <tr> 
   <td>IEDriverServer</td> 
   <td>This allows you to select the location of IEDriverServer.</td> 
   <td align="center">The path to the bundled WebDriver, if available.</td> 
  </tr> 
  <tr> 
   <th colspan="3">Binaries</th> 
  </tr> 
  <tr> 
   <td>Firefox</td> 
   <td>This allows you to select the location of Firefox binary (for example, to use a version other than the system default).</td> 
   <td align="center">(None)</td> 
  </tr> 
  <tr> 
   <td>PhantomJS</td> 
   <td>This allows you to select the location of PhantomJS binary.</td> 
   <td align="center">(None)</td> 
  </tr> 
 </tbody>
</table>

**Note:** It's also possible to set the above locations (binaries and WebDrivers) using Java system properties, in which case the above options will be overridden and those values shown instead.

## Bundled WebDrivers ##

ZAP provides add-ons with the WebDrivers, when those add-ons are installed ZAP will attempt to use the bundled WebDrivers by default. Some OSs might not have a WebDriver for some of the browsers, in those cases ZAP will inform there's no WebDriver available. The bundled WebDrivers can also be (re)set with the 'Bundled' button (for example, if another WebDriver was manually set).

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsSeleniumIntro" rel="nofollow">Selenium</a></td> 
   <td>for an overview of the Selenium add-on</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsSeleniumApi" rel="nofollow">API</a></td> 
   <td>for an overview of the Selenium API</td> 
  </tr> 
 </tbody>
</table>