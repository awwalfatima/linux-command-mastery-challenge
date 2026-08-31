#Day 20: Text Processing & Pipes

#Phase 4 - ENVIRONMENT, VIM & TEXT PROCESSING | Day 20 of 30

#Commands covered today

See commands.md for all 10 commands with my own explanation of what each one does.

#What I practiced

I created a raw log file called `drill.log` and used grep to filter for ERROR entries. I then used awk to extract the timestamp, sort to arrange the results, and uniq to remove duplicate timestamps. I combined everything into one pipeline: grep "ERROR" drill.log | awk '{print $1, $2}' | sort | uniq`. I also practiced sort and uniq separately using a names.txt file to understand how they work together in a pipeline.

#What surprised me

I initially used sort names.txt | uniq names.txt, but I realized that uniq should receive the output from sort through the pipe instead of using the filename again. Correcting it to sort names.txt | uniq helped me understand how output flows from one command to the next.

#Evidence

Screenshot or terminal transcript of the drill in evidence/.

#Related

Previous day: ../day-19-vim-navigation-search-replace/

Next day: ../day-21-viewing-process/