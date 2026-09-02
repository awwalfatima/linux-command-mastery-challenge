#Day 23: Init Systems & systemctl Basics
#Phase 5 - PROCESS & SERVICE MANAGEMENT | Day 23 of 30

#Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does.

#What I practiced
I practiced managing the nginx service with systemctl. I stopped nginx,
confirmed that it was inactive, restarted it, and then used enable --now
to enable it to start automatically at boot and start it immediately.
I confirmed that nginx was both active and enabled.

#What surprised me
I accidentally typed reloads instead of reload, which gave me an
Unknown command error, and I fixed it by using the correct command.

#Evidence
Screenshot or terminal transcript of the drill in evidence/.

#Related
Previous day: ../day-22-Controlling-Processes-with-Signals/
Next day: ../day-24-Deeper-Service-Management-and-Logs/
