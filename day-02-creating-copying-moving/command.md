mkdir  stands for make directory,is a command you use to create folder,which is called directory in linux. You create directory by typing mkdir followed by the name of the directory. i.e mkdir practice (this will create a folder named practice)
mkdir -p is used when creating nested folders or directories, the -p stands for parent. You create it by mkdir -p then the names of the folder in hierarchy order, or how they should be nested rather. example : mkdir -p practice/day1/day2/day3
touch is for creating files. touch then the name of the file, for instance touch final, this will create a file called final.
cp stands for copy, it use to copy files while keeping the original file, it duplicates the file. you write cp then the source followed by the destination. i.e cp file1 file2 file3 file (this will copy files 1,2,3 into folder file )
cp -r is copy recursive, this means it copies directories and their files.i.e cp -r day2/day3 day1, everything here, the files and the directory in day2 and 3 will be copied to day1
mv is for moving and renaming folder or file. i.e mv complete completed (renames complete to completed)
rm stands for remove, it a command that removes files. rm then the name of the file. i.e rm final
rm -r removes recursively, deletes folder with it files. i.e rm -r complete
rm -rf removes recursively with force without confimation prompt. i.e rm -rf practice2
rmdir removes empty directory. rmdir then the name of the directory, i.e rmdir completed
