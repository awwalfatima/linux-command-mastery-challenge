Day 13: APT Package Management
Phase 3 - Package Management & System Utilities | Day 13 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

Today's practice focused on using APT to manage packages on Ubuntu. The drill was to refresh the package index, search for a small utility, install it, inspect its package information, and then remove it completely along with its configuration files.

I started by refreshing the package index:

sudo apt update

I then searched for a small utility and chose figlet:

apt search figlet

I attempted to install it with:

sudo apt install figlet

However, the installation did not complete because my Ubuntu system reported an unmet dependency involving systemd-sysv and systemd.

The error indicated that systemd-sysv required:

systemd (= 255.4-1ubuntu8.4)

while APT was trying to install:

systemd 255.4-1ubuntu8.17

I attempted to troubleshoot the issue by repairing the broken dependencies:

sudo apt --fix-broken install

I then refreshed the package lists again:

sudo apt update

and attempted to upgrade the packages:

sudo apt upgrade

After the troubleshooting steps, I tried installing figlet again:

sudo apt install figlet

Unfortunately, the same dependency problem remained, so I was unable to complete the installation and therefore could not proceed to the package inspection and removal stages of the drill.

#What I learned

This exercise helped me understand that APT package management is not just about installing individual applications. Packages can depend on specific versions of other packages, and a dependency conflict can prevent an otherwise simple installation from completing.

#What surprised me

What surprised me was that a small utility like figlet could not be installed because of a dependency conflict with systemd. I expected the installation to be straightforward, but troubleshooting the package manager became part of the exercise.

#Evidence

Screenshot or terminal transcript of the package management practice are in evidence/.

The dependency error is also included as evidence because it documents the troubleshooting process and the fact that the installation could not be completed.

Related

Previous day: ../day-12-group-and-access-circles/

Next day: ../day-14-NF/YUM-Alternative-Installs/