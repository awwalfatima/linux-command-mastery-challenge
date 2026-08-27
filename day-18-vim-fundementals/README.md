Day 18: Vim Fundamentals
Phase 4 - ENVIRONMENT, VIM & TEXT PROCESSING | Day 18 of 30

#Commands covered today

See commands.md for all 10 commands with syntax and my own explanation of what each one does.

#What I practiced

Today’s practical drill was focused on getting comfortable with the Vim text editor and its different modes.

I opened a new file in Vim and typed three lines of text:

first line of text: Thank you IOTBTECH and TekTariq
second line of text: i love linux
third line of text: this is the last one, i promise :)

I practiced entering Insert mode with i, returning to Command/Normal mode with Esc, and saving the file with :wq.

I then reopened the file, moved to the middle line, and used dd to delete it. I used u to undo the deletion and restore the line, then saved and exited using :wq.

This drill helped me understand that Vim works differently from a normal text editor because actions such as typing, deleting, saving, and quitting depend on the mode I am currently in.

#What surprised me

The biggest thing that surprised me was how easy it is to get stuck in Vim if I forget which mode I am in. Learning that Esc takes me back to Normal mode made the editor much easier to control, especially when I needed to use commands like dd, u, and :wq.

#Evidence

Screenshots from the practical drill are stored in evidence/.


#Related

Previous day: ../day-17-persisting-configuration/

Next day: ../day-19-Vim-Navigation-and-Search/Replace.../