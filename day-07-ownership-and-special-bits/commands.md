#chown changes the owner of a file or directory.
#chown user:group changes both the owner and group ownership of a file or directory.
#chown -R recursively changes ownership for a directory and everything inside it
#chgrp this command changes the group ownership of a file or directory.
#chmod u+s(SUID) sets the SUID bit so an executable runs with the privileges of its owner.
#chmod g+s(SGID) sets the SGID bit so that files created in a directory inherit the directory's group.
#chmod +t(sticky bit) the sticky bit so users can generally delete only files they own within a shared directory.
#find -perm/4000 finds files with the SUID permission bit set.
#getfacl displays the detailed Access Control List (ACL) permissions for a file or directory.
#setfacl -m  adds specific ACL permissions for a user or group.