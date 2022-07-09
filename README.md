# unix-recycle-bin
UNIX recycle bin to safely delete and restore files


Problem:
UNIX has no recycle bin at the command line.  When you remove a file or directory, it is gone and cannot be restored. This project is to write a recycle script and a restore script. This will provide users with a recycle bin which can be used to safely delete and restore files.


Script 1 – Recycle				
A script called recycle that mimics the rm command. The recycle script is able to accept the name of a file as a command line argument as rm does, but instead of deleting the file, the script moves it to a recyclebin directory called recyclebin in the home directory.

The rm command can remove multiple files, for example rm file1 file2 file3. rm can also use wildcards, for example  rm file* .  The rm command can use the –i option, for interactive mode, and  the –v option for verbose mode. The rm command can remove directories and their contents using the –r option. 


Script 2 – Restore
A script called restore to restore individual files back to their original location. The user will determine which file is to be restored and use the file name with inode number in order to restore the file. The restore script can also restore files that were recycled recursively.
