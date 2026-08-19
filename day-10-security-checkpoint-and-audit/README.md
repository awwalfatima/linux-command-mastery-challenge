Day 10 CHECKPOINT Security Checkpoint & Audit
Phase 2 - Permissions, Ownership & Security | Day 10 of 30
#Commands covered today

See commands.md for the full list of commands.

#What I practiced

Today was a checkpoint where I brought together several of the security and account management commands I had practiced during this phase.

I started by checking login history with last and last -n 5, then used lastlog to inspect the last login information for system accounts. I also tested filtering the results for my own account and by time period.

I checked active sessions with w, who, and who -q. The results showed no active login sessions being reported by those commands at the time of the check.

Next, I audited my account identity and group memberships using groups and id. The output confirmed that my xahramas account has UID/GID 1000 and is a member of several groups, including adm, sudo, audio, video, plugdev, users, netdev, and project.

Finally, I searched my shell history with history | grep sudo. This gave me a quick audit trail of previous administrative actions, including package installation, directory creation, ownership and permission changes, and group management commands.

Overall, this checkpoint helped me practice looking at a Linux system from a security audit perspective who has access, who is logged in, what groups users belong to, and what administrative actions have previously been performed.

#What surprised me

What surprised me was seeing "Never logged in" for accounts in the lastlog output, including my own account, even though I was actively working in the terminal. I also made a small typo with lastlo instead of lastlog, which resulted in a command not found message and reminded me to verify command names carefully.

#Evidence

Screenshots and terminal transcripts from this checkpoint are stored in evidence/.

#Related

Previous day: ../day-09-Integrity-encryption-and-Firewalling/

Next day: ../day-11-Creating-and-Managing Users/