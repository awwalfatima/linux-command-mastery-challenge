# Day 11: User,Groups & Package Management

# Phase 3 - Creating and Managing Users | Day 11 of 30

## Commands covered today

See commands.md for all 10 commands with my own explanation of what each one does.

## What I practiced

I practiced creating, managing, modifying, and deleting Linux user accounts. I created users with `useradd`, checked their account information with `getent passwd`, removed a user with `userdel`, worked with passwords using `passwd`, checked my group membership with `groups`, and practiced adding a user to a supplementary group with `usermod -aG`.

## What surprised me

I initially ran useradd -m testuser2 without sudo and received a permission error, which reminded me that creating and modifying system users normally requires administrative privileges. I also learned that usermod -aG must be used with sudo when modifying another user's group membership.

## Evidence

Screenshots or terminal transcripts of the user management drills are stored in evidence.

## Related

Previous day: ../day-10/Security-Checkpoint-and-Audit

Next day: ../day-12/Groups-Access-Circles
