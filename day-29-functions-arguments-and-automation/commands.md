#function_name(){} this groups several commands together under one name so you can run them repeatedly without rewriting the commands. i.e greet() {
echo "Hello, how are you?"
echo "what is today?"}
greet
#$1 /$2 positional args represent arguments passed to a bash script or function,they are like inputs given to your script.
#$# /$* /$@ these are special bash variables that tell you about the arguments passed to a script.($# provides number of argurment; $* represents all positional arguments as one group; $@ it preserves each argument)
#$0 contains the name/path used to run the script.
#exit codes($?) shows the exit status of the most recently executed command.
#crontab syntax cron allows linux to automatically run commands or scripts at scheduled times.crontab is where those schedules are define.
#cron scheduling (O * * * *) this runs the command at minute od everyday hour.
#nohup script.sh & allows a command or script tp continue running even after you close the terminal or disconnect from the session. & puts the process in the background.
#trap tells bash when a particular signal or event happens, run this command.
#logger sends a message to the system logging facility,allowing your script to write messages into the system logs.
