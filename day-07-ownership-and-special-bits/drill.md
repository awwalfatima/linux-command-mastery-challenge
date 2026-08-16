#wsl
#whoami
#sudo groupadd project
#sudo usermod -aG project xahramas
#sudo usermod -aG project stude
#newgrp project
#groups
#mkdir home/sharedproject
#sudo chown xahramas:project home/sharedproject
#chmod 2775 home/sharedproject
#ls -ld home/sharedproject
touch home/sharedproject/-file2
ls -l home/sharedproject/file2
sudo find / -type f -perm -4000 -ls 2>/dev/null