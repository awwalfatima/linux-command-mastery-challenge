#ssh stands for secure shell, it allows you to securly connect to another computer over a network and work on it from your terminal.syntax: ssh username@server_ip, i.e ssh ubuntu@192.168.6.8
#ssh -p allows you to specify the SSH port. the defualt port is 22. syntax: ssh -p port username@server_ip, i.e: ssh -p 80 ubuntu@192.168.4.5
#ssh -i tells ssh which private key file to use for authentication. syntax; ssh -i /path/ username@server_ip. i.e ssh -i C:\Users\pc\Desktop\my-linux-challenge-keypair.pem ubuntu@54.132.43.23
#ssh-keygen creates an ssh key pair, which consists of private and pblic keys.
#ssh-copy-id copies your public ssh key to a remote server,this allows you to log in using ssh key instead of passowrd.syntax: ssh-copy-id username@server_ip
#scp stands for secure copy protocol, this allows you to securely copy files between your local machine and a remote machine over ssh.syntax: scp file username@server:/remote/path i.e scp report.txt ubuntu@192.168.2.3:/home/ubuntu
#sftp ssh file transfer protocol provides an interactive way to transfer and manages files on a remote machine securely. syntax: sftp username@server. i.e sftp ubuntu@192.168.1.20
#rsync synchronizes files and directories between locations.its can transfer only changes,rather than copying everything,therefore making it useful for backups,deployment and synchronizing directories.syntax: rsync source destination.
#~/.ssh/config configuration file
#sshd_config hardening this is the configuration file for ssh server daemon