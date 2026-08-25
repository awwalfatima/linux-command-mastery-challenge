Day 16: Environment Variables
Phase 4 - Shell & Environment | Day 16 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does. 

#What I practiced

I practiced creating and checking temporary environment variables with export, viewing variables with printenv and echo, removing them with unset, and working with the PATH variable.
For the practice drill, I created a temporary variable, confirmed its value, and then unset it. I also created ~/newdir, added it to my PATH for the current shell with export PATH=$PATH:$HOME/newdir, and created a greetings.sh script inside the directory. I used which greetings.sh and
command -v greetings.sh to prove that the shell could find the script through the updated PATH.

#What surprised me

I expected the script to run after adding its directory to PATH, but I got Permission denied because the script did not have execute permission. I learned that PATH only helps the shell locate a command, the file must also have the appropriate execute permission to run it.

#Evidence

Terminal screenshots in evidence/ 

Related

Previous day: ../day-15-Users-and-Packages-Checkpoint/
Next day: ../day-17-Persisting-Configuration/