# Passive Scan Rules #

The following release quality passive scan rules are included in this add-on:

## Application Errors ##

Check server responses for HTTP 500 - Internal Server Error type responses or those that contain a known error string.

## Cache Control ##

Checks "Cache-Control" and "Pragma" response headers against general industry best practice settings for protection of sensitive content.
At MEDIUM and HIGH thresholds only non-error or non-redirect text responses (excluding JavaScript) are considered.
At LOW threshold all responses apart from images and CSS are considered including errors and redirects.

## Content Type Missing ##

Raises an alert if the response is lacking a Content-Type header or if the header exists but the value is empty.

## Cookie HttpOnly ##

Ensures that as cookies are set they are flagged HttpOnly. The HttpOnly flag indicates to browsers that the cookie being set should not be acted upon by client side script (such as JavaScript).

## Cookie Secure Flag ##

Looks for cookies set during HTTPS sessions, raises an alert for those that are set but do not include the secure flag. A cookie set with the secure flag will not be sent during a plain HTTP session.

## Cross Domain Script Inclusion ##

Validates whether or not scripts are included from domains other than the domain hosting the content. By looking at the "src" attributes of "script" tags in the response.
Allowed Cross-Domain scripts:

 *  Any script with a non-empty "integrity" attribute is ignored - the integrity value is not checked as this will be checked by the browser
 *  At MEDIUM and HIGH thresholds if a script URL falls within a context that also includes the URL of the base message no alerts will be raised.

## Header XSS Protection ##

Checks for the existence of and value/setting of the X-XSS-Protection header. This response header can be used to configure a user-agent's built-in reflective XSS protection.
At MEDIUM and HIGH thresholds only non-error or non-redirect HTML responses are considered.
At LOW threshold all text responses are considered including errors and redirects.

## Mixed Content ##

For content served via HTTPS analyse all the src attributes in the response looking for those sourced via plain HTTP.

## Password Autocomplete ##

Looks for "password" type input fields and checks for the setting "autocomplete=off".

## Private Address Disclosure ##

Checks response content for inclusion of RFC 1918 IPv4 addresses. A malicious user might leverage knowledge of internal addressing to perform social engineering attacks or other exploits.

## Session Id in URL Rewrite ##

This scanner checks for the existence of session token type parameters being rewritten to the URL. To help reduce false positives the scanner checks the length of the token value, if the value of the parameter is not greater than 8 characters in length then the parameter is ignored (i.e.: survey?sId=5 would not be flagged as vulnerable).

## X-Content-Type-Options ##

This scanner check for the Anti-MIME-Sniffing header X-Content-Type-Options and ensures it is set to 'nosniff'.
At MEDIUM and HIGH thresholds this scanner does not alert on client or server error responses or redirects.
At LOW threshold it will alert on all responses including errors and redirects.
thresholds it alerts on all response types if the header is missing or set to something other than 'nosniff'.

## X-Frame-Options Header Scanner ##

This scanner checks for the existence and validity of the X-Frame-Options header.
At MEDIUM and HIGH thresholds this only looks at non-error or non-redirect HTML responses.
At LOW threshold it looks at all text responses including errors and redirects.
The following conditions may result in an alert:

 *  **X-Frame-Options Header Not Set:**  If the X-Frame-Options header is missing from the response completely.
 *  **Multiple X-Frame-Options Header Entries:**  When more than one X-Frame-Options header is detected on the response.
 *  **X-Frame-Options Defined via META (Non-compliant with Spec):**  A "http-equiv" entry was found in the response that attempts to define X-Frame-Options, which is not supported by the specification.
 *  **X-Frame-Options Setting Malformed:**  The header is present with no value, or the value is not as expected (i.e.: other than "DENY", "SAMEORIGIN", or "ALLOW-FROM").

By default no alerts will be raised in the response includes a Content-Security-Policy 'frame-ancestors' element as this take precedence over the X-Frame-Options header. However at LOW threshold the above issues will still be reported but at a LOW risk.