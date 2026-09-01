Day 21: Viewing Processes
Phase 5 - PROCESS & SERVICE MANAGEMENT | Day 21 of 30

#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

I practiced finding and inspecting running processes in my WSL environment. I used pgrep bash to find the PIDs of running Bash processes, then used top to view active processes and system resource usage. I also used pstree -p to see how processes are connected, and pstree -p 23201 to focus on a specific Bash process and its child sleep processes. Finally, I attempted to identify the process using port 80 with sudo lsof -i :80.

#What surprised me

What surprised me was seeing the relationship between the Bash process and the sleep processes in pstree, it made the parent child relationship between processes much easier to understand. I also learned that commands requiring sudo will fail if the password is entered incorrectly, so I need to make sure I use the correct password when checking protected system information.

#Evidence

Screenshots of pgrep, top, pstree, and the lsof -i :80 attempt are saved in evidence/.

#Related

Previous day: ../day-20-text-processing-pipes/

Next day: ../day-22-controlling-processes-with-signals.../