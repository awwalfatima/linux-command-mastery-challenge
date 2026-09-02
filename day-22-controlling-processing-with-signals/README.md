Day 22: Controlling Processes with Signals

Phase 5 - PROCESS & SERVICE MANAGEMENT | Day 22 of 30

#Commands covered today

See commands.md for all 10 commands with my own explanation of what each one does.

#What I practiced

I practiced controlling background and foreground processes using sleep, jobs, fg, bg, Ctrl+Z, and nohup. I started a long running sleep process in the background, brought it to the foreground with fg, suspended it using Ctrl+Z, and then resumed it in the background with bg. I then started another sleep process using nohup so it could continue running independently of the terminal session.

#What surprised me

I initially tried to use bg on a job that was already running in the background and received the message bg: job 2 already in background. This helped me understand that bg is specifically used to resume a stopped or suspended job, not a job that is already running in the background. I then corrected the workflow by bringing the process to the foreground, suspending it with Ctrl+Z, and using bg to resume it.

#Evidence

Screenshots of the process control practice, including jobs, fg, Ctrl+Z, bg, and nohup, are saved in evidence/.

#Related

Previous day: ../day-21-viewing-processes/

Next day: ../day-23-Init-Systems-and-systemctl-Basics.../