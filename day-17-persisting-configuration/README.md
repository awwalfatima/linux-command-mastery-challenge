Day 17: Persisting Configuration
Phase 4 - Shell Environment & Configuration | Day 17 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

Today’s practical drill was about making shell customizations persistent.

I edited my ~/.bashrc file and added a custom environment variable named variables and an alias. I then used source ~/.bashrc to reload the configuration without closing or opening another terminal.

For the alias, I created:

alias drill="ls -lah"

After reloading .bashrc, I ran drill and confirmed that it worked by displaying a detailed listing of my home directory.

I also practiced checking how Bash interprets a command using type, and explored the system-wide Bash configuration files such as /etc/environment and /etc/bash.bashrc.

The final part of the drill was to verify that the configuration remains available when starting a fresh shell session,which i did by typing printenv variables and drill after closing and opening the shell.

#What surprised me

I initially ran into an error while trying to use nano because the editor was not installed on my system. I also made a small mistake while creating the ll alias, which produced a command not found error; after correcting the alias syntax, ll worked as expected.

#Evidence

Terminal screenshots from the drill are stored in evidence/.

#Related

Previous day: ../day-16-environment-variables/

Next day: ../day-18-Vim-Fundamentals.../