Day 28: Bash Scripting Foundations
Phase 6 - NETWORKING, SCRIPTING & REMOTE ACCESS | Day 28 of 30

#Commands covered today
See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

I practiced writing and executing a Bash script that reads the user's name, checks whether a configuration file exists, and loops through three server names to test their connectivity using ping.
I started by creating my script with:
nano drill.sh
The script used read -p to get the user's name and a variable to store the input. I then used an if statement to check whether config.conf exists.
I created the configuration file with:
touch config.conf
and used:
ls -l
to confirm that the file was created.
I also created an array containing three server names:
SERVERS=("google.com" "cloudflare.com" "github.com")
and used a for loop to go through each server and ping it.
After writing the script, I made it executable with:
chmod +x drill28.sh
and executed it with:
./drill28.sh
During the practice, I had to correct some Bash syntax and spelling mistakes in the script, including the shebang, the read -p syntax, the structure of the if statement, and the spelling of the SERVER variable. Fixing these errors helped me understand that Bash scripting requires careful attention to syntax and variable names.

#What surprised me

What surprised me was how small syntax mistakes could prevent the entire script from running correctly. I learned that the shebang must be written as #!/bin/bash, read -p needs the prompt in the correct position, and variables such as $SERVER must be spelled exactly the same way each time. This made me appreciate how important careful syntax is when writing automation scripts.

#Evidence

Screenshot or terminal transcript of the drill in evidence/.

#Related

Previous day: ../day-27-remote-access-file-transfer/

Next day: ../day-29-Functions-Arguments-&-Automation/