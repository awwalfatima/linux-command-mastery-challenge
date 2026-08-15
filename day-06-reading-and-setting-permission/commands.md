# ls -l(permission string) shows detailed information about files
# chmod(relative +/-) changes permission from the current permission(rwx,meaning read,write and execute), the + is for adding permission while the - is for removing, for example chmod u+x file.sh(this will add users permission to execute in the file.sh )
# chmod(assignment=) this sets permission as specified, i.e chmod u=rw practice.txt, this will give the user read and write permission only.
# chmod 755(octal) following the r w x 4 2 1 respectively, the 7 permits the user to rwx, group can r and execute others too.
# chomd 644(octal) sets permission for owner to read and write, while group and others  can only read.
# chmod 600(octal) sets permission for owner to read and write, group and others have no permission.
# chmod -R the R stands for recursively, this changes permissions recursively, this will change the permissions directory and its files.
# umask Shows or sets the default permission mask. 
# umask -S displays the current umask in symbolic human readable form, for instance u=rwx,g=rx,o=rx
# stat -c %A %U %G displays a file's permissions, owner, and group in a customized format. %A = permissions, %U = owner, %G = group.
