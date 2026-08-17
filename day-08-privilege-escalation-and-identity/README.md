Day 08: Privilege Escalation & Identity
Phase 3 - Users, Groups & Privilege Management | Day 8 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

#What I practiced

Today I practiced moving between normal user and privileged contexts and checking what different users are allowed to do.

I started by checking my current identity with whoami and my permissions with sudo -l, which showed that my account could run commands with sudo privileges. I then used sudo -i to open a root shell and confirmed the change with pwd and whoami.

I also practiced sudo -u by running:

sudo -u stude whoami

and:

sudo -u nobody whoami

Both commands demonstrated how sudo -u can execute a command as a specified user.

I checked the sudoers configuration with:

sudo visudo -c

which returned:

/etc/sudoers: parsed OK
/etc/sudoers.d/README: parsed OK

I also practiced su and su -. My attempts to switch to the stude account using su resulted in authentication failures, which became part of the troubleshooting process.

Finally, I used id to inspect user and group information:

id
id stude

This showed the user IDs, group IDs, and group memberships for both accounts.

#What surprised me

What surprised me was that having sudo privileges does not mean that every method of switching users will automatically work. I was able to use sudo -u stude whoami successfully, but trying su - stude resulted in Authentication failure, which helped me understand that sudo and su use different authentication and privilege mechanisms.

I also made an error while trying sudo !!, which resulted in:

sudo: sudosudo-u: command not found

This reminded me that command shortcuts need to be used carefully and that understanding what the shell expands is just as important as knowing the command itself.

#Evidence

Screenshots from the practice session are stored in:

evidence/


Related

Previous day: ../day-07-ownership/

Next day: ../day-09-Integrity-Encryption-Firewalling/