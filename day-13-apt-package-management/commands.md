#apt advanced package tool, the apt file manager allows you to install software,remove software and update your system.
#apt update this command updates your source list, this is the syntax sudo apt update name of the software/package you want to update. i.e sudo apt htop
#apt upgrade this will update all the packages on your system that has update available,its updates to the latest version, sudo apt upgrade followed by name of the package you want to upgrade, i.e sudo apt upgrade htop.
#apt full-upgrade upgrades the package but can install or remove packages to complete the upgrade. sudo apt full-upgrade
#apt remove removes software but leaves it configuration files behind. sudo apt remove softwares name.
#apt install is the command that allows you to install software. you sudo apt install softwares/package name.i.e sudo apt install tree.
#apt purge this command removes everything, including configuration files, unlike apt remove, which removes the package, but leaves configuration files, so when next you install the packege that old configuration file exits, sudo apt purge name of the package removes everything completely.
#apt autoremoove removes packages that are no longer needed, packages that are dependencies of other programs that has been removed.syntax: sudo apt autoremove.
#apt search searches for a packege, apt search package name, for search no sudo privildge is needed.
#apt show shows information about the package you want to see, it will show you the source, maintainer, install size, dependencies, download size etc.syntax: apt show
#dpkg -l / dpkg -L dpkg -l lists the debian packages installed, syntax dpkg -l /dpkg -L lists all files installed by specific packages, syntax : dpkg -L name of package 
  