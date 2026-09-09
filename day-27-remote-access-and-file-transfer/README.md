Day 27: Remote Access & File Transfer
Phase 6 - NETWORKING, SCRIPTING & REMOTE ACCESS | Day 27 of 30
#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

I practiced generating an SSH key pair, adding my public key to a remote Amazon EC2 server, connecting to the server using the new SSH key, and securely transferring files between my local machine and the remote server.

I first displayed my public SSH key and worked with my existing EC2 key pair to access the server. On the remote server, I created the .ssh directory and added my new public key to ~/.ssh/authorized_keys.

I then set the appropriate permissions using chmod:

chmod 700 ~/.ssh
chmod 600 ~/.ssh/authorized_keys

After that, I tested the new SSH key:

ssh -i ~/.ssh/id_ed25519 ec2-user@44.220.193.98

I confirmed that I was connected to the remote server using:

hostname
whoami

Next, I created a local test file:

echo "This is the file i am creating" > test.txt

and checked its contents with:

cat test.txt

I used scp to securely copy the file from my local machine to the EC2 server:

scp -i ~/.ssh/id_ed25519 test.txt ec2-user@44.220.193.98:/home/ec2-user/

I then connected to the server and verified that the file was successfully transferred using ls -l and cat test.txt.

Finally, I copied the file back from the EC2 server to my local machine:

scp -i ~/.ssh/id_ed25519 ec2-user@44.220.193.98:/home/ec2-user/test.txt ./downloaded-test.txt

I verified the downloaded file with ls -l and cat downloaded-test.txt.

#What surprised me

One thing that surprised me was working with SSH keys and realizing that I could add a new public key to the server's authorized_keys file and then use the corresponding private key to connect. I also encountered problems when trying to use my Windows C:\Users\... path directly in the Linux/WSL terminal.

#Evidence

Screenshot or terminal transcript of the drill in evidence/.

#Related

Previous day: ../day-26-networking-basics/

Next day: ../day-28-Bash-Scripting-Foundations/