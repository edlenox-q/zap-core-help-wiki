# Release 1.3.1 #

The following changes were made in this release:

## Bug fixes: ##

### Issue 97: Working Directory for Applications ###

### Issue 98: Not possible to cancel check for updates ###

### Issue 100: Alerts tab has 2 'Resend...' right click popups ###

### Issue 104: Display warning dialog, when no root CA certificate exists ###

### Issue 110: Choosing user's language by default, when starting the first time ###

### Issue 112: Provide a way to apply language packs on Mac OS ###

### Issue 121: Session compare report javascript broken in Firefox 3 ###

### Issue 123: Cant select https site from Active scan window if theres an http equivalent ###

### Issue 127: CSRF token feature does not work in fuzz - added help explanation for partial fix ###

### Issue 140: The Display options shouldnt include the advanced or windows manager options ###

### SSL Bug which prevented SSL connections from being established in any browser ###

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