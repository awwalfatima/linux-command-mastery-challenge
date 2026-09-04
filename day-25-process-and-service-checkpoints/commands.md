#ps aux | grep displays runnining processess on the system then searches the output for a particular process.i.e ps aux | grep sleep
#systemctl status <svc> shows the current status of a systemd service
#journalctl -u <svc> --since today shows the journal logs for a specific service from today.
#kill -0 (liveness check) checks whether a process exists and whether you have permission to send it a signal.
#uptime shows how long the system has been running, along with information about system load.
#free -h shows RAM and swap memory usage in human readble values.
#vmstat virtual memory statistics provide memory about processes, memory, swap, cpu, system activity.
#iostat displays statistics about CPU and disk, input/output activity.
#watch repeatedly runs a command and displays its output
#crontab -e / crontab -1 cron allows linux to automatically execute commands at scheduled time, crontab -e opens your users cron schedule for editing while crontab -l lists your existing jobs