#systemctl list-units --type=service lists the currently loaded service units managed by systemd,it is useful when you want to see which services are currently loaded and their status.
#systemctl list-units --state=failed shows services that have failed.
#systemctl daemon-reload tells systemd to reload its service configuration files.
#journalctl displays logs collected by the systemd journal.
#journalctl -f displays journal logs in real time. the -f means follow.
#journalctl -u shows logs for a specific systemd service, the u stands fpr unit.
#journalctl --since shows logs starting from a specific time. i.e journalctl --since today
#journalctl -p err shows journal messages at the error priority level. the p is for priority and the err means error
#tail -f/var/log/syslog Displays the last few lines of syslog file and continues showing new entries as they are written.
#tail -f/var/log/auth.log follow authentication logs live.