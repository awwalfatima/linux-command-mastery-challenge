#kill sends a signal to a process, despite its name, it does not necessarily mean terminate immediately, it can send diffrenet signals that tell a process to perform different actions.
#kill -9 immediately terminates a process
#kill -HUP sends the sighup signal
#killall sends signal to processes based on their names rather than their PID. killall process name
#pkill similar to kill, but allows you to select processes using their names and other criteria, also can target processes belonging to a particular user (pkill -u username). i.e pkill sleep
#fg stands for foreground, this brings a suspended job back into the foreground of your current terminal.
#bg stands for background, it resumes a suspended job and allow it to continue running in the background.
#Ctrl+Z(suspend) suspends a process
#nohup stands for no hangup, it allows a command to continue running even after you log out or close the terminal. syntax nohup command &
#disown removes a job from the shells job table, is used after the command has already been started. 