#Day 04: Searching the Filesystem
#Phase 1 - File Navigation | Day 4 of 30
Commands covered today

#See commands.md for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

#Commands covered:

find -name
find -type
find -size
find -mtime
find -perm
locate
updatedb
du
du -sh
df -h
#What I practiced

Today I practiced searching the Linux filesystem and checking disk usage using Ubuntu through WSL. I searched /etc for .conf files using find -name, searched /var for files larger than 1 MB using find -size, and used du and df -h to understand how much storage was being used and how much space remained available.

During the /etc search, I found configuration files such as nsswitch.conf. When searching /var, the command returned a number of files larger than 1 MB, but I also encountered Permission denied messages for some protected directories. This showed me that filesystem searches are affected by permissions and that not every location can be accessed by a normal user.

#What surprised me

What surprised me was how much information a single find command can return when searching a system directory like /var. I also learned that Permission denied does not necessarily mean the command is wrong it can simply mean the current user does not have permission to inspect certain directories.

The df -h output also showed that the root filesystem was at approximately 89% usage, with about 27.9 GB of space remaining, which made the importance of monitoring disk space much more practical.

#Evidence

Terminal screenshots from my practice session are stored in evidence/.


#Related

Previous day: ../day-03-reading-inspecting-files/

Next day: ../day-05-links-checkpoint/