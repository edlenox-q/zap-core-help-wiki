# Passive Scan Rules #

The following release quality passive scan rules are included in this add-on:

## Application Errors ##

## Cache Control ##

## Content Type Missing ##

## Cookie HTTP Only ##

## Cookie Secure Flag ##

## Cross Domain Script Inclusion ##

## Header XSS Protection ##

## Mixed Content ##

## Password Autocomplete ##

## Private Address Disclosure ##

## Session Id in URL Rewrite ##

This scanner checks for the existence of session token type parameters being rewritten to the URL. To help reduce false positives the scanner checks the length of the token value, if the value of the parameter is not greater than 8 characters in length then the parameter is ignored (i.e.: survey?sId=5 would not be flagged as vulnerable).

## X-Content-Type-Options ##

This scanner check for the Anti-MIME-Sniffing header X-Content-Type-Options and ensures it is set to 'nosniff'. At HIGH threshold this scanner does not alert on client or server error responses, for all other enabled thresholds it alerts on all response types if the header is missing or set to something other than 'nosniff'.

## X-Frame-Option ##

This scanner checks for the existence and validity of the X-FRAME-OPTIONS header. At HIGH threshold this scanner does not alert on client or server error responses, for all other enabled thresholds it alerts on all response types if the header is missing or invalid. Invalid meaning that the header is present with no value, or that the value is not as expected (i.e.: other than "DENY", "SAMEORIGIN", or "ALLOW-FROM").