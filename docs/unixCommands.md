# Helpful Unix Commands

| command | description | example |
:----------|:-------------|:----------|
| ```awk```|print field (organized by $1,$2,$3,etc.) in a file - here we print the third one |```awk '{print $3}' file1``` |
| |print by regular expression - here we print where field 2 is more than field 3 |```awk '$2>$3' file1``` |
| |print by regular expression - here we print where field 1 is equal to "a" |```awk '$1 == "a" file1``` |
| ```cal``` | shows the calendar for this month | ```cal``` |
| | calendar for year | ```cal 2020```|
| | calendar for a month in specific year | ```cal 2 2020``` |
| ```cat``` | view contents of a file | ```cat myfile```
| | to append file | ```cat file1 >> file2``` |
| ```cd``` | to change into a subdirectory | ```cd subdir``` |
| | to change into any directory | ```cd home/folder1/subfolder1/``` |
| | to change into parent directory | ```cd ../``` |
| | to change to root directory | ```cd /``` |
| | to change into home directory | ```cd``` |
| ```chmod``` | allow yourself to execute one of your own files | ```chmod u+x file``` |
| | allow anyone with access to the directory to read/execute a file | ```chmod o+rx file``` |
| ```cp``` | copy file (use the -i option to ensure original is kept) | ```cp -i file1 copyfile1``` |
| | place file in another directory to yours | ```cp -i /home/folder1/subfolder1/file1 ./``` |
| | place file in your directory into another | ```cp -i file1 /home/folder1/subfolder1/``` |
| | copy an entire folder to your directory | ```cp -ir /home/folder1/ ./``` |
| ```date``` | get the today's date | ```date``` |
| ```du```|get the disk usage for for contents in a directory |```du```|
|```echo```|echo a word to the output|```echo "hello world"```|
| |echo a variable like your PATH| ```echo $PATH```|
| |echo possible combinations|```echo {A,G,C,T}{A,G,C,T}```|
| ```find```|finds files matching pattern (in this case all .txt files) in directory | ```find ./ -name "*.txt" print``` |
| | find all .txt files in home directory |```find "$HOME/" -name "*.txt" print```|
|```grep```| find occurences of a pattern in a file|```grep 'a' file1```|
| |find occurences of a pattern regardles of case|```grep -i 'a' file1```|
| |find number of occurences|```grep -c 'a' file1```|
| ```jobs```|lists jobs waiting or running in the background (numbered like "%1,%2,%3,etc.") |```jobs``` |
| |start job 4 again |```%4``` |
|```kill```| kill a specific job|```kill %4``` |
|```less/more```|these commands allow you to preview a file (NOT A BINARY FILE!!!) and go through it by hitting enter or space. leave the preview by pressing ```q``` |```less``` |
| | |```more``` |
|```ls```|see files in directory |```ls``` |
| |see invisible files in directory (those starting with "." like a ".bashrc" file) | ```ls -a``` |
| |see permissions and invisible files|```ls -la``` |
|```man```|get the documentation for a command, for example ```ls``` |```man ls``` |
|```mkdir```|make a directory |```mkdir newdir``` |
| |make a directory in another folder|```mkdir /home/folder1/newdir``` |
| ```mv```|rename a file, does not save the original|```mv -i oldname newname``` |
|```ps```|what files are running? |```ps``` |
| ```pwd```|print the working directory |```pwd``` |
|```rm```|to **PERMANENTLY** remove a file |```rm file1``` |
| | to **PERMANENTLY** remove a directory |```rm -r /home/folder1/``` |
| ```rmdir```| also **PERMANENTLY** removes a directory| ```rmdir /home/folder1/```|
|```sed```|replace pattern with another pattern in a file - here we replace "no" with "FALSE" |```sed 's/no/FALSE/g' file1``` |
| | replace pattern with nothing |```sed 's/no//g' file1```|
| ```sort```| sort by first column| ```sort file1```|
| ```vi```|open a text editor. hit ```i``` to start writing, ```Esc``` then ```:wq``` then ```Enter``` to leave and save | ```vi filetocreate```|


> This cheatsheet was adapted from the [University of Indiana Unix Command Introduction](https://kb.iu.edu/d/afsk)

> To dive in deeper I reccommend taking a look at these [bioinformatics oneliners](https://github.com/stephenturner/oneliners)

[Return To Main Page](../index.md)
