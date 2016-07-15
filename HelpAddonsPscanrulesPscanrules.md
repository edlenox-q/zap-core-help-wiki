# Passive Scan Rules #

The following release quality passive scan rules are included in this add-on:

## Application Errors ##

Check server responses for HTTP 500 - Internal Server Error type responses or those that contain a known error string.

## Cache Control ##

Checks "Cache-Control" and "Pragma" response headers against general industry best practice settings for protection of sensitive content.

## Content Type Missing ##

Raises an alert if the response is lacking a Content-Type header or if the header exists but the value is empty.

## Cookie HttpOnly ##

Ensures that as cookies are set they are flagged HttpOnly. The HttpOnly flag indicates to browsers that the cookie being set should be acted upon by client side script (such as JavaScript).

## Cookie Secure Flag ##

Looks for cookies set during HTTPS sessions, raises an alert for those that are set but do not include the secure flag. A cookie set with the secure flag will not be sent during a plain HTTP session.

## Cross Domain Script Inclusion ##

Validates whether or not scripts are included from domains other than the domain hosting the content. By looking at the "src" attributes of "script" tags in the response.

 *  Allowed Cross-Domain Hosts: At HIGH threshold if a script URL falls within a context that also includes the URL of the base message no alerts will be raised.

## Header XSS Protection ##

Checks for the existence of and value/setting of the X-XSS-Protection header. This response header can be used to configure a user-agent's built in reflective XSS protection.

## Mixed Content ##

For content served via HTTPS analyse all the src attributes in the response looking for those sourced via plain HTTP.

## Password Autocomplete ##

Looks for "password" type input fields and checks for the setting "autocomplete=off".

## Private Address Disclosure ##

Checks response content for inclusion of RFC 1918 IPv4 addresses. A malicious user might leverage knowledge of internal addressing to perform social engineering attacks or other exploits.

## Session Id in URL Rewrite ##

This scanner checks for the existence of session token type parameters being rewritten to the URL. To help reduce false positives the scanner checks the length of the token value, if the value of the parameter is not greater than 8 characters in length then the parameter is ignored (i.e.: survey?sId=5 would not be flagged as vulnerable).

## X-Content-Type-Options ##

This scanner check for the Anti-MIME-Sniffing header X-Content-Type-Options and ensures it is set to 'nosniff'. At HIGH threshold this scanner does not alert on client or server error responses, for all other enabled thresholds it alerts on all response types if the header is missing or set to something other than 'nosniff'.

## X-Frame-Options Header Scanner ##

This scanner checks for the existence and validity of the X-Frame-Options header. At HIGH threshold this scanner does not alert on client or server error responses, for all other enabled thresholds it alerts on all response types. The following conditions may result in an alert:

 *  **X-Frame-Options Header Not Set:**  If the X-Frame-Options header is missing from the response completely.
 *  **Multiple X-Frame-Options Header Entries:**  When more than one X-Frame-Options header is detected on the response.
 *  **X-Frame-Options Defined via META (Non-compliant with Spec):**  A "http-equiv" entry was found in the response that attempts to define X-Frame-Options, which is not supported by the specification.
 *  **X-Frame-Options Setting Malformed:**  The header is present with no value, or the value is not as expected (i.e.: other than "DENY", "SAMEORIGIN", or "ALLOW-FROM").