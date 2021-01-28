# Python-Reverse-Shell
A python reverse shell designed to be converted into an .exe file and run on a windows machine. Includes persistence and some other features

USAGE:
1. run server.py on your own machine to listen for connections
2. run reverse_shell.py on the target machine and wait 20 seconds for timeout to finsish

NOTES:
-This shell shoud be converted into a .exe file with pyinstaller for the best results. As it is primarily designed fror windows10.

-This shell includes persistence. Meaning when the reverse_shell.py is ran for the first time it will copy the shell to a hidden location rename it to
 win32.exe and add to this to the registry. resulting in it being run when the PC is turned on, It will try to connect to the host machine every 20 seconds 
 until it finally connects then once disconnected the PC must be turned off and on again for it to try and connect again.
