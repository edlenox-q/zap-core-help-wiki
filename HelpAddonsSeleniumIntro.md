# Selenium #

The Selenium add-on provides WebDrivers, for other add-ons, to invoke and remotely control web browsers. It's also bundled the HtmlUnit web browser, an headless Java based web browser.

The following web browsers are supported:

 *  Chrome
 *  Firefox - the following versions are known to work: 45 (ESR), 46 and 47.0.1 (older version might work too). Some versions are known to not work, for example, 47.0. Newer versions (≥ 48) require geckodriver.
 *  HtmlUnit
 *  Internet Explorer
 *  Opera
 *  PhantomJS
 *  Safari

To use Firefox, Chrome, Internet Explorer, Opera, PhantomJS and Safari, you must have them installed in your system.

Some of the web browsers require extra configurations, done in [Options Selenium screen][], to access and control them:

 *  Chrome - requires ChromeDriver, if not on the system's PATH, it can be set in the options. For more information on ChromeDriver and how to obtain it refer to the [ChromeDriver website][].
 *  Firefox - requires geckodriver for versions ≥ 48, it can be set in the options. For more information on geckodriver and how to obtain it refer to the [geckodriver website][] (see footer note for caveat when using geckodriver).
 *  PhantomJS - requires PhantomJS binary, if not on the system's PATH, it can be set in the options. For more information on PhantomJS and how to obtain it refer to the [PhantomJS website][] (see footer note for caveat when using PhantomJS).
 *  Internet Explorer - requires IEDriverServer, if not on the system's PATH, it can be set in the options. For more information on IEDriverServer refer to the [IEDriverServer website][] (see footer note for caveat when using Internet Explorer).

**Firefox/geckodriver Note:** There's an issue ([Bug 1103196][]) that prevents HTTPS sites from being used in versions ≥ 48 and < 52.

**PhantomJS Note:** There's an issue ([Issue \#11342][Issue _11342]) that prevents sites at localhost, 127.0.0.1 and ::1 from being proxied through ZAP. Until a fix is available is advised to not use it in those cases. Some add-ons might choose to show warning message when that happens. As workaround one could define, in the `hosts` file, a domain name mapping to the local address and use that domain name instead.

**Internet Explorer Note:** Not all versions of Internet Explorer work out of the box, refer to the [IEDriverServer website][IEDriverServer website 1] for more details on how to configure them.

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsSeleniumOptions" rel="nofollow">Options Selenium screen</a></td> 
   <td>for an overview of the Selenium Options</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpAddonsSeleniumApi" rel="nofollow">API</a></td> 
   <td>for an overview of the Selenium API</td> 
  </tr> 
 </tbody>
</table>


[Options Selenium screen]: HelpAddonsSeleniumOptions
[ChromeDriver website]: https://sites.google.com/a/chromium.org/chromedriver/
[geckodriver website]: https://github.com/mozilla/geckodriver
[PhantomJS website]: http://phantomjs.org/
[IEDriverServer website]: https://code.google.com/p/selenium/wiki/InternetExplorerDriver
[Bug 1103196]: https://bugzilla.mozilla.org/show_bug.cgi?id=1103196
[Issue _11342]: https://github.com/ariya/phantomjs/issues/11342
[IEDriverServer website 1]: https://code.google.com/p/selenium/wiki/InternetExplorerDriver#Required_Configuration