# Day 03: Reading & Inspecting Files

## Phase 1 - File Navigation | Day 3 of 30

## Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does and when I would reach for it.

Commands covered:

* cat
* less
* head
* head -n
* tail
* tail -f
* wc
* wc -l
* file
* stat

## What I practiced

I practiced reading and inspecting a real log file using Git Bash. I navigated to the Windows Temp directory and used the AdobeARM.log file as my practice file. I viewed the contents of the log with cat, inspected the most recent entries using tail -n -15, counted the file contents with wc, identified the file type with file, and examined detailed file metadata using stat.

The log file contained Adobe Acrobat update activity, including update checks, network connection errors, BITS download errors, and update status information. Working with an actual log file made the commands easier to understand because I could see how these tools can be used to investigate what is happening on a system.

## What surprised me

What surprised me was how much information could be extracted from one log file using simple Linux commands. The stat command was especially useful because it showed detailed metadata such as the file size, permissions, owner, inode, timestamps, and file type, while tail -n -15 made it easy to focus on the most recent activity instead of reading the entire log.

## Evidence

Terminal screenshots from my practice session are stored in evidence/.

The evidence shows:

* Navigating to AppData/Local/Temp using cd
* Opening and reading AdobeARM.log with cat
* Viewing the latest 15 lines with tail -n -15
* Counting information in the log with wc
* Identifying the file type with file
* Inspecting complete file metadata with stat
* Observing real Adobe Acrobat update and BITS related log messages
* Working with a real system log rather than an artificially created practice file


## Related

Previous day: ../day-02-creating-copying-moving/

Next day: ../day-04-searching-files/
