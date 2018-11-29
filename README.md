# windshield
Wrapper for GNU screen tool to provide better and faster operation
version: 0.1a

# Operation
1. Change SCREEN_NAME and COMMAND VARIABLES<br>
   A) SCREEN_NAME: Forms the base string of name of the screens to be generated<br>
   B) COMMAND: The default command string to run upon screen generation<br>
2. Make script executable, i.e. $chmod +x server-a; $chmod +x windshield
3. New screens are labeled via a number appended to "SCREEN_NAME-".
4. (Optional) Make a copies of windshield for different configs. 

# Shortcuts
1. sls: "screen -ls"           --List all running screens
2. sr:  "screen -r $arg"       --Rejoin running screen named $arg
3. sX:  "screen -X -S $arg"    --Kill screen named $arg

# Notes
1. Hope to expand features with...<br>
   A) command line args<br>
   B) consolidated config file or session profiles<br>
   C) smarter testing for existing screen polling?<br>
   D) local killall function: kill all screens with SCREEN_NAME $name<br>
   E) generate: generate $n number of screens<br>
