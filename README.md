# typing_tx
Transfer files by typing
------
Do you need to transfer files to another computer and your access/premissions are restricted such that you can't use FTP/SFTP/SCP and you only have access to a terminal or a VNC/NoMachine desktop?  If this is your conundrum, then this little script is for you.

This script will
* compress a file or directory
* convert the compressed binary data to characters available on your keyboard
* give you a few seconds to mouse over and click in an open editor on the remote machine
* automatically type out the data into the remote editor

This script can also decode the characters typed, decompressing them back into the original file or directory (the -d option).  However, this can also be done with the command:
```
% base64 -d <remote-text-file> | tar xJf -
```

The rate of typing can be controlled (-l and -k options) so as to not overflow your connection to the remote machine.

Tha amount of time, in seconds, provided to mouse over and click in an open editor on the remote machine can be adjusted with the -s option
