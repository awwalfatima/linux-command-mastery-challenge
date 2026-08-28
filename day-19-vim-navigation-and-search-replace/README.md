# Day 19: Vim Navigation & Search/Replace

# Phase 4 - ENVIRONMENT, VIM & TEXT PROCESSING | Day 19 of 30

# Commands covered today

See commands.md for all 10 commands with my own explanation of what each one does and when I would reach for it.

# What I practiced

Today’s practical drill focused on navigating through a configuration file, searching for specific keywords, moving between search results, and replacing text across the entire file using Vim.

I opened my configuration file in Vim and used :10 to jump directly to line 10. I then practiced searching for keywords using / for forward searches and used n and N to move between matching occurrences.

After navigating through the file, I practiced Vim's search and replace feature using :%s/old/new/g to replace every occurrence of a word across the file. The replacement was successful,changed backward to backdown, and Vim displayed 3 substitutions on 2 lines, confirming that the changes had been made.

I also practiced the other navigation and editing commands covered today, including gg, G, dw, x, o, O, and ZZ.

# What surprised me

What surprised me was how quickly Vim can make changes across multiple lines with a single command. Seeing 3 substitutions on 2 lines after using the search and replace command helped me understand how powerful Vim can be for editing configuration files.

# Evidence

Screenshots from the practical drill are stored in evidence/.


# Related

Previous day: ../day-18-vim-fundamentals/

Next day: ../day-20-text-processing-and-pipes/