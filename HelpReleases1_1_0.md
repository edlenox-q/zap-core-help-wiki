# Release 1.1.0 #

The following changes were made in this release:

## Significant changes: ##

### OWASP rebranding ###

ZAP has been accepted as an OWASP project.
Its homepage is now: http://www.owasp.org/index.php/OWASP\_Zed\_Attack\_Proxy\_Project

### Brute Force ###

The ability to brute force files and directories based on code from the OWASP DirBuster project.
The new Brute Force tab shows the files and directories found.

### Port Scan ###

The ability to port scan sites.
The new Port Scan tab shows the ports found.

### Active Scan tab ###

The new [Active Scan tab][] shows the requests and responses as a result of actively scanning a site.

### Spider tab ###

The [Spider tab][] now allows you to continue using ZAP while spidering a site.
You can also pause and resume the spider.

### Smartcard support ###

Smart card support has been added c/o the Andiparos project.
The following smartcard devices have been tested on Windows:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Safeguard</td>
   <td>Aladdin eToken</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td></td>
   <td>Aladdin eToken Pro</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Omnikey</td>
   <td>Omnikey 3121</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td></td>
   <td>CardMan 6121</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Gemalto</td>
   <td>Reflex 20 V2</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td></td>
   <td>Swiss Stick</td>
  </tr> 
 </tbody>
</table>

The following smartcard devices are reported to work:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Omnikey</td>
   <td>CardMan 4040</td>
  </tr> 
 </tbody>
</table>

### Attack menu ###

The new [Sites tab][] right click 'Attack' menu allows you to start various scans.

### More internationalisation ###

All of the main tabs and menu items have now been internationalised.

### Localisation ###

Support for the following languages are built into this version:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>English</td>
   <td>The default language</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Brazilian Portuguese</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>German</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Polish</td>
   <td></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Spanish</td>
   <td></td>
  </tr> 
 </tbody>
</table>

### Language selection ###

On start up you will be prompted to choose the language to use.
New languages are automatically detected by the presence of files with names of the form Messages\_<locale>.properties in the ZAP directory.

## Minor changes: ##

### Disabled 'default file' plugins ###

The plugins which detect default files are effectively made redundant by the new brute force scanner.
These have therefore been disabled.

### Scanner summaries ###

Counts of the number and types of the current scans are now displayed in the [footer][].

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


[Active Scan tab]: HelpUiTabsAscan
[Spider tab]: HelpUiTabsSpider
[Sites tab]: HelpUiTabsSites
[footer]: HelpUiFooter