#sudo this command is use for running commands with elevated privildges.
#sudo -i when you need to run a sequence of admin tasks,this command allows you to use root privildege.
#sudo -u runs command as a specific user
#sudo !! this command re runs the previous command
#visudo edits the /etc/sudoers file while checking its syntax to prevent errors that could break sudo access.
#su this command is use when you want to switch user from the one you are in, i.e su stude, this will switch to stude user.
#su - u runs command as specific user
#whoami prints the name of the current user,the username that you are in, i.e whoami will print xahramas(if i am in xahramas)
#sudo -l lists all the tools and permissions that you can run as sudo.(ALL:ALL)ALL thismeans as any user and as any group we can run all commands.
#id this command prints detailed information about your identity, i.e id (this will print out the userid,groupid, gid,sudo etc),if you want it for specific user, then you id username.