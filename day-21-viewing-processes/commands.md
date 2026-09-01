#ps aux displays a snapshot of almost all running processes on the system,including processess running in the background.
#ps -ef displays runnig processess with parent child relationship.
#ps -u displays processess belonging to a specific user, i.e ps -u xahramas 
#top gives a live, continuously updating view of running processes, it keeps refreshing.
#htop similar to top but displays processes with more visual interface.
#pgrep searches for processes based on thier name or other attributes and returns their PID. syntax pgrep processname
#pstree displays processes in a tree structure, showing parent and child relationships. syntax pstree
#lsof -i list open files, this command show network related open files/connections.
#jobs shows background and suspended jobs started from your current shell.
#nice / renice nice starts a new process with a specified cpu scheduling  priority. renice changes the nice value of a process that is already running.