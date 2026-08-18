Day 09: Integrity, Encryption & Firewalling
Phase 3  Security, Networking & System Protection | Day 9 of 30
#Commands covered today

See commands.md for all 10 commands with my own explanation of what each one does.

#What I practiced

I practiced checking file integrity using md5sum and sha256sum. I created day.txt, generated its checksum, changed the file, and generated the checksum again to see how the hash changed. I also practiced GPG encryption and decryption, and tried using chattr and UFW for file protection and firewall rules though they didnt work in my environment.

#What surprised me

I expected chattr and UFW to work normally, but my WSL environment did not support them properly. chattr returned an operation-not-supported error because my filesystem uses wslfs, while UFW could not initialize iptables.

#Evidence

Screenshot or terminal transcript of the drill in evidence/.

Related

Previous day: ../day-08-Privilege-Escalation-Identity/

Next day: ../day-10-security-checkpoint-and-audit/