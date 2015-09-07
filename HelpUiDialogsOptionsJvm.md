# Options JVM screen #

This screen allows you to configure the JVM options used when starting ZAP.

### JVM Options ###

A free format text field which will be added to the Java command line call when invoking ZAP via either zap.sh or zap.bat.

The option was added so that the Java maximum memory allocation pool size can be set, which is of the form: -Xmx*n* where *n* is the size in bytes.
Good values for this field could be:

 *  \-Xmx256m
 *  \-Xmx512m
 *  \-Xmx1024m

Unlike the other ZAP options these are held in the file ".ZAP\_JVM.properties" in the user's default ZAP directory, which depends on the OS being used:

 *  Windows 7/8: C:\\Users\\*<username>*\\OWASP ZAP
 *  Windows XP: C:\\Documents and Settings\\*<username>*\\OWASP ZAP
 *  Linux: ~/.ZAP
 *  Mac OS: ~/Library/Application Support/ZAP

If you make a mistake when setting these options then ZAP may fail to start.
If that happens then deleting this file should fix the problem.

Note that these options are not used when starting ZAP via the Windows exe.

## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td>
   <td>for an overview of the user interface</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="HelpUiDialogsOptionsOptions" rel="nofollow">Options dialogs</a></td>
   <td>for details of the other Options dialog screens</td>
  </tr> 
 </tbody>
</table>

## External links ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="http://docs.oracle.com/javase/7/docs/technotes/tools/windows/java.html#CBBIJCHG" rel="nofollow">Java 7 options</a></td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td><a href="http://docs.oracle.com/javase/8/docs/technotes/tools/windows/java.html#BABDJJFI" rel="nofollow">Java 8 options</a></td>
  </tr> 
 </tbody>
</table>