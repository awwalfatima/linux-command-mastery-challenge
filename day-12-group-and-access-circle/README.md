#Phase 2 - Permissions, Ownership & Security | Day 12 of 30

Commands covered today

See commands.md for all 10 commands with my own explanation of what each one does.

#What I practiced

I practiced managing Linux groups and controlling group membership. I created a group named devs, added users to the group, confirmed the group and user information with getent, removed a user from the group, and finally deleted the group.

The main drill was:

sudo groupadd devs
sudo gpasswd -a xahramas devs
sudo gpasswd -a testuser1 devs
getent group devs
sudo gpasswd -d xahramas devs
sudo groupdel devs
getent group devs

I also used getent group and getent passwd to inspect the groups and users configured on the system.

#What surprised me

I noticed that deleting a group with groupdel removes the group itself, so checking getent group devs afterward confirms that the group no longer exists.

#Evidence

Screenshot or terminal transcript of the drill in evidence.


#Related

Previous day: ../day-11-Creating-and-Managing-Users/

Next day: ../day-13-APT-Package-Management-(Debian/Ubuntu)/