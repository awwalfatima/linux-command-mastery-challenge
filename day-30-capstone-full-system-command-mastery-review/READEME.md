Day 30: Capstone — Full System Command Mastery Review
Phase 6 - NETWORKING, SCRIPTING & AUTOMATION | Day 30 of 30
#Commands covered today

See commands.md for all the commands.
#What I practiced

For today's capstone, I brought together commands and skills from across the 30 Day Linux Command Mastery Challenge and used them in a practical system administration workflow.

I started by building a system health check script, day30_healthcheck.sh, to display information such as system uptime, memory usage, disk usage, running processes, and system status. I also created a second version that combined ps, systemctl, and journalctl to produce a simple system report.

I then connected to my remote Amazon EC2 server using SSH and practiced running commands on the remote host. I used hostname and whoami to confirm that I was connected to the correct machine and user.

As part of the deployment practice, I used scp to transfer my health check script from my local machine to the EC2 server. After deploying the file, I checked its permissions and applied chmod and chown to make sure the file had the appropriate permissions and ownership.

I also practiced scheduling the health check script with cron. I used a cron entry to run the script every hour and redirected the output to health_check.log.

For log analysis, I practiced using journalctl together with grep, awk, and sed. This helped me filter errors, select specific fields from log output, and modify text in the results.

I also practiced using find to locate stale .log files that had not been modified for more than seven days. I used -print first so that I could review the files before considering deletion.

Finally, I performed a basic security audit using last, who, and history to review recent login activity, currently logged in users, and recent commands recorded in my shell.

The capstone brought together many of the commands I learned throughout the challenge, especially Linux system administration, permissions, networking, remote access, process management, services, logs, and automation.

I also practiced the commands needed for the final capstone deployment workflow: SSH, SCP, permissions, ownership, service management, journal logs, and output logging.

#What surprised me

What surprised me was how many of the commands from the earlier days of the challenge could be combined into one practical workflow. Commands that I originally learned separately, such as ssh, scp, chmod, chown, systemctl, journalctl, grep, awk, sed, find, last, and who, started to make more sense when I used them together on a real EC2 server.

One mistake I made was initially treating each command as a separate task, but the capstone helped me see how these commands can work together to automate and manage a real Linux system.

#Evidence

Screenshot or terminal transcript are found in evidence/.

300-Command Journal

This day also serves as the final review of my 30-Day Linux Command Mastery Challenge.

#Related

Previous day: ../day-29-functions-arguments-automation/

Challenge complete: Day 30 of 30