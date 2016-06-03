# Session Management #

ZAP handles multiple types of session management (called **Session Management Methods**) that can be used for websites / webapps. Each **[Context][]** has a Session Management Method defined which dictates how sessions are kept.

So far, just cookie based and HTTP authentication session management methods have been implemented, but the system supports easy addition of new methods, according to user needs.

### Cookie-Based Session Management ###

In the case of this method the session is being tracked through cookies. Currently, the session tokens that are used are imported from the [HTTP Sessions][] Extension.

### HTTP Authentication Session Management ###

In the case of this method the session is managed with HTTP request header `Authorization`.

## Configured via ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsSessionContexts#sm" rel="nofollow">Session Contexts Dialog</a></td> 
   <td></td> 
  </tr> 
 </tbody>
</table>

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="http://youtu.be/cR4gw-cPZOA" rel="nofollow">Youtube tutorial</a></td> 
   <td>of the Authentication, Session Management and Users Management features of ZAP [external link to http://youtu.be/cR4gw-cPZOA].</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td> 
   <td>for an overview of the user interface</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td> 
   <td>provided by ZAP</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsSessionContexts" rel="nofollow">Session Contexts Dialog</a></td> 
   <td>for an overview of the Session Properties</td> 
  </tr> 
 </tbody>
</table>


[Context]: HelpStartConceptsContexts
[HTTP Sessions]: HelpStartConceptsHttpsessions