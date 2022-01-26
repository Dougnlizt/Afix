# Afix
Android File Transfer Creation Date Fix Tool, or 'Afix', closes a gap created when using the Android File Transfer tool by Google.

When using the Android transfer tool, the 'created date' timestamp for files is not persistent, and instead has a new date based on when the transfer occurred.  In many cases, this may not be a big deal.  However, for things like pictures, the creation date may be important when determining the date of a picture being taken.

This tool allows you to select a directory, then reset all files within that directory (with the option to recurse through all sub directories) and re-assigns the created date timestamp to match the last modified timestamp.
