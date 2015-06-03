# Getting Started #

The quickest way to get going with ZAP is to use the Quick Start add-on, which is installed by default.
This allows you to enter a URL which ZAP will first [spider][] and then [active scan][].
For a more in depth test you should explore your application using your browser or automated regression tests while proxying through ZAP.

At its heart ZAP is an [intercepting proxy][].
You need to configure your browser to connect to the web application you wish to test through ZAP.
If required you can also configure ZAP to connect through another proxy - this is often necessary in a corporate environment.


If you know how to set up proxies in your web browser then go ahead and give it a go!
If you are unsure then have a look at the [Configuring proxies][] section.

Once you have configured ZAP as your browser's proxy then try to connect to the web application you will be testing.
If you can not connect to it then check your proxy settings again. You will need to check your browser's proxy settings, and also ZAP's proxy settings.
Its also worth checking that the application that you are trying to test is running!

When you have successfully connected to your application via your browser then have a look at ZAP again. You should now see one or more lines in the [Sites][] and [History][] tabs.
If so we're in business. If not then you'll need to check your proxy settings again.

The next thing to do is to start a [basic penetration test][].


## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartProxies" rel="nofollow">Configuring Proxies</a></td>
   <td>for details of how to set up ZAP as a proxy in your web browser</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpIntro" rel="nofollow">Introduction</a></td>
   <td>the introduction to ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td>
   <td>provided by ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpStartChecks" rel="nofollow">Scanner Rules</a></td>
   <td>supported by default</td>
  </tr> 
 </tbody>
</table>


[spider]: HelpStartConceptsSpider
[active scan]: HelpStartConceptsAscan
[intercepting proxy]: HelpStartConceptsIntercept
[Configuring proxies]: HelpStartProxies
[Sites]: HelpUiTabsSites
[History]: HelpUiTabsHistory
[basic penetration test]: HelpPentestPentest