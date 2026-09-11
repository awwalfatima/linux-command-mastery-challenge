#nano day30_healthcheck.sh
##!/bin/bash
#echo "uptime is: "&uptime
#echo "memory usage: " &free -h
#echo "disk usage: "&df -h
#echo "running process: " &ps aux
#echo "system status: "&systemctl status
#chmod +x day30_healthcheck.sh
#./day30_healthcheck.sh
#nano day30_healthcheck2.sh
#echo "process: "&ps aux
#echo "services: "&systemctl status
#echo "system logs: "&journalctl -n 20
#chmod +x day30_healthcheck2.sh
#./day30_healthcheck2.sh
#ssh -i C:\Users\pc\Downloads\my-linux-challenge-keypair.pem ec2-user@44.220.193.98
#hostname
#whoami
#ls -l ~/my-linux-challenge-keypair.pem
#ls -l day30_healthcheck.sh
#scp -i ~/my-linux-challenge-keypair.pem day30_healthcheck.sh ec2-user@44.220.193.98:/home/ec2-user/
#ssh -i ~/my-linux-challenge-keypair.pem ec2-user@44.220.193.98
#ls -l /home/ec2-user/day30_healthcheck.sh
#chmod +x /home/ec2-user/day30_healthcheck.sh
#./day30_healthcheck.sh
#chmod 744 day30_healthcheck.sh
#ls -l day30_healthcheck.sh
#whoami
#chown ec2-user:ec2-user day30_healthcheck.sh
#sudo dnf cronie -y 
#crontab -e
#0 * * * * /home/ec2-user/day30_healthcheck.sh >> /home/ec2-user/health_check.log 2>&1
#journalctl -n 20
#journalctl --no-pager | grep -i "error"
#journalctl -n 10 --no-pager | awk '{print $1, $2, $3, $5}'
#journalctl -n 10 --no-pager | sed 's/systemd/SYSTEMD/g'
#journalctl --no-pager | grep -i "error" | awk '{print $1, $2, $3, $5}' | sed 's/systemd/SYSTEMD/g'
#find /home/ec2-user -type f -name "*.log" -mtime +7 -print
#last -n 10
#who
#history | tail -n 20
