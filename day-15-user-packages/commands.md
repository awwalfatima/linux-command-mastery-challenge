#id <user> checks if a user has been created successfully, syntax is id then user name 
#getent passwd <user> gets information,enteries from the system database. i.e getent passwd alex
#useradd -m -G this command creates a user in the home directory, and should be assign to a specified group. i.e useradd -m -G groupname username, useradd -m -G xahramas alex
#passwd <user> sets or changes a users password. i.e sudo passwd alex
#apt list --installed this shows list of installed packages
#apt list --upgradable this command shows packages that have new version, showing what should be upgraded.
#apt update && apt install -y this is two commands join together, apt install the package,the -y (yes) means it should do it automatically,and upgrade the package. i.e sudo apt upgrade && apt install -y tree
#dpkg -l | grep grep searches for text, dpkg -l lists installed debian packages, i.e dpkg -l | grep curl this command will list installed packages and will search for curl
#apt autoremove this command removes installed packages with their dependencies
#history displays command that you have previously typed