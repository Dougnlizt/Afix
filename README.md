# Afix
Android File Transfer Creation Date Fix Tool, or 'Afix', closes a gap created when using the Android File Transfer tool by Google.

When using the Android transfer tool, the 'created date' timestamp for files is not persistent, and instead has a new date based on when the transfer occurred.  In many cases, this may not be a big deal.  However, for things like pictures, the creation date may be important when determining the date of a picture being taken.

This tool allows you to select a directory, then reset all files within that directory (with the option to recurse through all sub directories) and re-assigns the created date timestamp to match the last modified timestamp.

Note that while this is intended for Pictures and MP4 video files, it will work for other files as well if the file modified time is sonner than the file created time.  In the case of downloading from something like Google Photos, the created and modified times get recreated and are the same.  In that event, an attempt is made to find the 'actual' created time attribute from the file's meta data.  The format of meta data is not consistent between file formats, so this does not always work.  Files that cannot be correctly updated are identified in the output accordingly.