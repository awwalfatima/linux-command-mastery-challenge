Day 06: Reading & Setting Permissions
Phase 2 - Permissions, Ownership & Security | Day 6 of 30
#Commands covered today

#See commands.md for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.


#What I practiced

I created a scripts.sh file in my WSL Linux environment and practiced setting its permissions to rwxr-xr-x using three different chmod methods.

First, I used relative notation:

chmod u+rwx,g+rx,o+rx scripts.sh

Then I used assignment notation:

chmod u=rwx,g=rx,o=rx scripts.sh

Finally, I used octal notation:

chmod 755 scripts.sh

After each change, I used ls -l to verify the result.

The final output confirmed:

-rwxr-xr-x 1 xahramas xahramas 0 Aug 16 00:08 scripts.sh

This confirmed that all three methods produced the same permission result.

#What I learned

The three permission methods can achieve the same result, but they work differently.

Relative +/- adds or removes permissions from the existing permissions.
Assignment = sets the exact permissions specified.
Octal notation provides a shorter numerical way to define the complete permission set.

For 755:

7 = rwx  → owner
5 = r-x  → group
5 = r-x  → others

Therefore:

755 = rwxr-xr-x
#What surprised me

My first attempts did not work because I was using Git Bash on the Windows filesystem and also made some chmod syntax mistakes by leaving out the filename. Moving into the native WSL Linux filesystem and paying attention to the complete chmod [permissions] [file] structure fixed the problem.

That troubleshooting helped me understand that the environment matters when practicing Linux permissions.

#Evidence

Screenshots from the practice session are stored in:

evidence/


#Related

Previous day: ../day-05-links-checkpoint/

Next day: ../day-07-ownership/