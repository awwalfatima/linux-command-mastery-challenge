Day 29: Functions, Arguments & Automation
Phase 6 - NETWORKING, SCRIPTING & AUTOMATION | Day 29 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#Today I practiced:

Function definitions: function_name() { }
Positional arguments: $1 / $2
Argument count and arguments: $# / $* / $@
Script name: $0
Exit codes: $?
crontab syntax
Cron scheduling: 0 * * * *
Running scripts with nohup script.sh &
trap
logger
#What I practiced

For today's drill, I turned yesterday's service checking script into a more reusable script that accepts a service name as an argument.

I used a Bash function to check whether the service is running. If the service is stopped, the script attempts to restart it.

I tested the script by passing nginx as the service name:

./drill28.sh nginx

I also practiced scheduling the script with cron so that it can run automatically every hour:

0 * * * * /home/xahramas/drill28.sh nginx

Before relying on the scheduled task, I checked the cron service status:

systemctl status cron

This helped me understand how Bash functions, command line arguments, exit codes, and cron can work together to automate a simple system administration task.

#What surprised me

What surprised me was how a small script can become much more useful when it accepts a service name as an argument, because I can reuse the same script for different services instead of creating a separate script for each one.

#Evidence

Screenshot or terminal transcript of the drill in evidence/.


#Related

Previous day: ../day-28-bash-scripting-foundations/

Next day: ../day-30-Capstone: Full-System-Command-Mastery-Review/