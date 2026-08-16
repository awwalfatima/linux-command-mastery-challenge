Day 06: Shared Project Folder, SGID & SUID Audit
Phase 2 - Permissions, Ownership & Security | Day 6 of 30
#Commands covered today

Today's practice focused on Linux permissions, group ownership, SGID, and SUID auditing.


#What I practiced

I created a shared project environment and practiced using Linux groups and permissions to control access.

First, I created a project group and added users to it. I then created a shared project directory, changed its group ownership to project, and applied the SGID bit using:

chmod 2775 home/sharedproject

I verified the permission with:

ls -ld home/sharedproject

The s in the permission string confirmed that SGID was enabled:

drwxrwsr-x

I then created a file inside the shared directory and checked its ownership to confirm that the new file inherited the project group.

Finally, I performed a system wide SUID audit using:

sudo find / -type f -perm -4000 -ls 2>/dev/null


This was the most difficult Linux practice I have done so far.

The challenge was not just remembering a command. I had to understand how users, groups, ownership, permissions, SGID, and SUID all connect together.

I also had to troubleshoot several issues along the way. 

The most important moment was seeing the s appear in:

drwxrwsr-x

and then confirming that a newly created file inherited the project group. That made the purpose of SGID much clearer than simply reading about it.

#What surprised me

What surprised me most was that a single permission bit can change how group ownership behaves for every new file created inside a directory.

Before this exercise, I thought of permissions mostly as r, w, and x. This drill showed me that Linux permissions go much deeper, especially when multiple users need to work on the same project.

#Evidence

Screenshots and terminal output from the practice session are stored in:

evidence/


Related

Previous day: ../day-05-links-checkpoint/

Next day: ../day-07-ownership/