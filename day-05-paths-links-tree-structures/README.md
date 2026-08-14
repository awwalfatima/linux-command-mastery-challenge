Day 05: Paths, Links & Tree Structures
Phase 1 - File Navigation | Day 5 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

tree
tree -L
ln (hard link)
ln -s (symbolic link)
readlink
realpath
basename
dirname
pushd / popd
ls -lt
#What I practiced
Practice Drill — Checkpoint

I practiced working with paths, symbolic links, and directory structures by finding a configuration file under /etc, creating a symbolic link to it, resolving its real path, and displaying the /etc directory structure to a depth of two levels.

I used:

find /etc/ -name "*.conf"
ln -s /etc/nsswitch.conf $config
realpath /etc/nsswitch.conf
cd /etc/
tree -L 2

I also practiced installing and checking tree. At first, tree was not available, and running sudo apt install tree returned E: Unable to locate package tree. I fixed this by updating the package lists with sudo apt update and then installing tree successfully.

After installation, I verified it with:

tree --version

and then used:

tree -L 2

to display the /etc directory structure two levels deep.

Hard link vs symbolic link

A hard link points directly to the same underlying file data as the original file, while a symbolic link works more like a shortcut because it points to the original file's path.

#What surprised me

What surprised me was that tree was not immediately available and sudo apt install tree could not find the package until I first ran sudo apt update, this helped me understand that Linux needs an up-to-date package list before apt can locate and install some packages.

#Evidence

Screenshots and terminal transcripts from the practice drill are stored in:

evidence/

The evidence shows:

Searching /etc for .conf files
Creating a symbolic link
Resolving the path with realpath
Updating the Ubuntu package lists
Installing tree
Checking the installed tree version
Running tree -L 2 on /etc
Related

Previous day: ../day-04-searching-filesystem/

Next day: ../day-06-permissions/