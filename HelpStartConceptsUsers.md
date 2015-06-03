# Users #

Users are the ZAP representations of websites/webapps' users. They allow certain actions to be performed from the point of view of an user of the webapps. For each **[Context][]**, a set of Users can be defined, which can then be used in actions related to the context. Most commonly, during various scans the request messages can be sent from the point of view of an User.

The concept of Users is tightly tied to the concepts of [Session Management][] and [Authentication][]. When a User is first used somewhere in ZAP, an authentication is performed (according to the Authentication Method defined for the Context) and a Session is created and configured for this user (according to the Session Management defined for the Context). After that, requests sent from the point of view of an User are modified (if necessary) and sent in such a way that the web server identifies them as being sent by an authenticated webapp/website user. If anytime a message is sent from the perspective of a User and the response received seems unauthenticated (as identified using the *Logged In* and *Logged Out* [Authentication indicators][Authentication]), a new authentication is performed and the Session is updated accordingly.

In order to perform the authentication of an user on a website / in a webapp, the Authentication Method defines how the authentication is done (the process), while the necessary credentials (the exact identifiers) are dependent on the user, so, in ZAP, they are configured in the Users.

## Configured via ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsSessionContexts#users" rel="nofollow">Session Contexts Dialog</a></td> 
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
   <td><a href="HelpStartConceptsAuthentication" rel="nofollow">Authentication Overview</a></td> 
   <td>for an overview of Authentication in ZAP</td> 
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
[Session Management]: HelpStartConceptsSessionManagement
[Authentication]: HelpStartConceptsAuthentication