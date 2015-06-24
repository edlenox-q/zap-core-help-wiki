# Options Forced Browse screen #

This screen allows you to configure the [Forced Browse][] options:

### Concurrent scanning threads per host ###

The number of threads the scanner will use per host.
Increasing the number of threads will speed up the scan but may put extra strain on the computer ZAP is running on and the target host.

### Recursive ###

If checked then the scanner will recurse through all of the sub-directories found.
This may take a long time.

### Default file ###

The default file selected when ZAP starts.

### Add custom Forced Browse file ###

Allows you to add your own files to be used when brute forcing files and directories.
These should be text files with one file or directory name per line.
Files are added to the 'dirbuster' directory underneath the ZAP home directory.


[Forced Browse]: HelpAddonsBruteforceConcepts