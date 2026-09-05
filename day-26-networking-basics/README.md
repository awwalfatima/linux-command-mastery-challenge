Day 26: Networking Basics

Phase 6 - NETWORKING, SCRIPTING & SSH MASTERY | Day 26 of 30

#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

I practiced the basic Linux networking commands by identifying my machine's network configuration and default gateway with ip a and ip route. I tested connectivity to Google using ping -c 3, checked Google's HTTP response headers with curl -I, and used ss -tulnp to see the ports currently listening on my system. I also practiced curl, wget, netstat -tulnp, hostname, and hostnamectl to understand how I can inspect and troubleshoot a Linux machine's network connectivity and identity.

#What surprised me

What surprised me was that my first ping -c 3 google.com failed with "Temporary failure in name resolution", but running the same command again succeeded. It helped me see the difference between having network connectivity and successfully resolving a hostname through DNS.

#Evidence

Screenshot or terminal transcript of the networking drill in evidence/.


#Related

Previous day: ../day-25-process-service-checkpoint/

Next day: ../day-27-Remote Access-&-File-Transfer/