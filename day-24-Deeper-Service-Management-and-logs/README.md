Day 24: Deeper Service Management & Logs
#Phase 5 - PROCESS & SERVICE MANAGEMENT | Day 24 of 30

#Commands covered today
See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced
I practiced going deeper into service management and Linux logging using systemctl and journalctl. I listed the services on my WSL system and checked for failed services, which returned 0 loaded units, then reviewed the system journal and pulled logs specifically for the nginx service to see its start, stop, reload, and restart activity. I also filtered the journal for error level messages and saw several WSL/kernel related errors, which helped me understand how logs can reveal problems beyond just the service I am currently managing.

#What surprised me
What surprised me was seeing that systemctl list-units --state=failed reported no failed services, while journalctl -p err still showed several error messages. This helped me understand that an error in the system journal does not automatically mean that a systemd service is currently in a failed state.

#Evidence
Screenshots of the service list, failed-service check, journalctl, Nginx service logs, and error level logs are stored in evidence/.

#Related
Previous day: ../day-23-init-systems-systemctl-basics/
Next day: ../day-25-process-and-service-checkpoint/