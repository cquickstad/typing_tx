# typing_tx
Transfer files by typing
------
Have you ever needed to transfer files to another computer and you didn't have FTP/SFTP/SCP and you only had access to a terminal or a VNC or NoMachine desktop?  If this is your conundrum, then this little script is for you.

This script will
* compress a file or directory
* convert the binary data to characters available on your keyboard
* then give you a few seconds to mouse over and click in an open editor on the remote machine
* type out the data into the remote editor

This script can also decode the characters typed, decompressing them back into the original file or directory (the '-d' option).

The rate of typing can be controlled (-l and -k options) so as to not overflow your connection to the remote machine.
