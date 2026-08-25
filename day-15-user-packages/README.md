Day 15: Users & Packages Checkpoint
Phase 4 - Users, Groups & Package Management | Day 15 of 30
Commands covered today

#See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

For today's checkpoint, I provisioned a new team member account called user5. I created a team-cloud group and added user5 to the group using useradd -m -G. I then set a password for the new user with passwd and verified the account and group membership using id user5.

After creating the account, I installed the three role related tools:

sudo apt install -y curl tree git

The installation confirmed that tree was already installed and upgraded curl and git along with their required dependencies. This gave me practical experience combining user provisioning and package installation into one workflow.

I also tested switching to the newly created user with:

su user5

When I attempted to install a package from the user5 account using sudo, I received:

user5 is not in the sudoers file.

This helped me understand that creating a user and adding them to a normal role group does not automatically give them administrative privileges.

#What surprised me

What surprised me was that the packages installed with apt are system-wide, not assigned specifically to user5. Even though I installed curl, tree, and git while logged in as another user, the tools are available to users across the system. The user's permissions and group membership determine what they are allowed to do with the system and its resources.

I also encountered the sudoers error when user5 attempted to use sudo, which reinforced the difference between being a normal user, belonging to a group, and having administrative privileges.

#Evidence

Screenshot/terminal transcript of the user creation, group assignment, password setup, verification, and package installation is stored in evidence/.


#Related

Previous day: ../day-14-dnf-rpm/
Next day: ../day-16-Environment-Variables/