# Day 02: Creating, Copying, Moving & Deleting

## Phase 1 - File Navigation | Day 2 of 30

### Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

Commands covered:

- mkdir
- mkdir -p
- touch
- cp
- cp -r
- mv
- rm
- rm -r
- rm -rf
- rmdir

### What I practiced

I practiced creating, copying, moving, renaming, and deleting files and directories using Git Bash. I created nested directory structures using mkdir -p, created multiple files with touch, and used cp -r to copy a directory and its contents to a backup location. I also practiced navigating into the directories to verify their contents, renaming a file with mv, and removing files with rm.

### What surprised me

What surprised me was that Linux does not treat files and directories the same way when deleting them. For example, when I tried rm practice2, the command failed because practice2 was a directory, which helped me understand why commands such as rm -r and rm -rf exist. I also made a few navigation and command structure mistakes during the practice, then corrected them and continued the exercise.

### Evidence

Terminal screenshots from my practice session are stored in evidence/.

The evidence shows:

- Creating nested directories with mkdir -p
- Creating empty files with touch
- Inspecting directory contents with ls
- Copying directories recursively with cp -r
- Creating a backup copy of the practice directory
- Moving and renaming a file with mv
- Removing files with rm
- Removing directories recursively with rm -r and rm -rf
- Navigating between directories with cd and cd ..
- Encountering and correcting command errors

### Practice Drill

The main drill was to create a nested folder structure, create files inside it, make a backup copy, rename a file, and clean up the practice directories.

The exercise helped me understand the difference between working with individual files and working with directories, especially when copying and deleting.

### Related

Previous day: ../day-01-file-navigation/

Next day: ../day-03-links/