#grep stands for global regular expression print.  
#grep -r searches recursively, it searches through a directory and its subdirectories for matching text. i.e grep -r "filename"
#sort arranges text in alphabetical order. sort filename
#sort -n sorts numbers according to their numerical value, i.e sort -n filename. 
#uniq removes adjacent duplicate lines, its removes only duplicates that are next to each other. i.e unique filename
#cut -d',' -f extracts specific fields/column from each line, cut -d',' -f1 filename
#awk '{print $1}' prints the first field/column of each line. i.e awk '{print $1}' teams.csv
#sed's/old/new/g stream editor, it is use for replacing words,deletinf lines and making bulk edits without opening a file in an editor 
#pipe chains(|) pipe connects commands together, it takes the output of one command and sends it as input to the next command.