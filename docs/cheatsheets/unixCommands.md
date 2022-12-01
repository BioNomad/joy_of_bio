# Helpful Unix Commands

### awk

| command | description | example |
:----------|:-------------|:----------|
| ```awk```|print field (organized by \$1,\$2,$3,etc.) in a file - here we print the third one |```awk '{print $3}' file1``` |
| |print by regular expression - here we print where field 2 is more than field 3 |```awk '$2>$3' file1``` |
| |print by regular expression - here we print where field 1 is equal to "a" |```awk '$1 == "a" file1``` |

### cal 

| command | description | example |
:----------|:-------------|:----------|
| ```cal``` | shows the calendar for this month | ```cal``` |
| | calendar for year | ```cal 2020```|
| | calendar for a month in specific year | ```cal 2 2020``` |

### cat 

| command | description | example |
:----------|:-------------|:----------|
| ```cat``` | view contents of a file | ```cat myfile```
| | to append file | ```cat file1 >> file2``` |

### cd 

| command | description | example |
:----------|:-------------|:----------|
| ```cd``` | to change into a subdirectory | ```cd subdir``` |
| | to change into any directory | ```cd home/folder1/subfolder1/``` |
| | to change into parent directory | ```cd ../``` |
| | to change to root directory | ```cd /``` |
| | to change into home directory | ```cd``` |

### chmod 

| command | description | example |
:----------|:-------------|:----------|
| ```chmod``` | allow yourself to execute one of your own files | ```chmod u+x file``` |
| | allow anyone with access to the directory to read/execute a file | ```chmod o+rx file``` |

### cp 

| command | description | example |
:----------|:-------------|:----------|

| ```cp``` | copy file (use the -i option to ensure original is kept) | ```cp -i file1 copyfile1``` |
| | place file in another directory to yours | ```cp -i /home/folder1/subfolder1/file1 ./``` |
| | place file in your directory into another | ```cp -i file1 /home/folder1/subfolder1/``` |
| | copy an entire folder to your directory | ```cp -ir /home/folder1/ ./``` |

### date 

| command | description | example |
:----------|:-------------|:----------|
| ```date``` | get the today's date | ```date``` |

### du 

| command | description | example |
:----------|:-------------|:----------|
| ```du```|get the disk usage for for contents in a directory |```du```|

### echo 

| command | description | example |
:----------|:-------------|:----------|

|```echo```|echo a word to the output|```echo "hello world"```|
| |echo a variable like your PATH| ```echo $PATH```|
| |echo possible combinations|```echo {A,G,C,T}{A,G,C,T}```|

### find 

| command | description | example |
:----------|:-------------|:----------|

| ```find```|finds files matching pattern (in this case all .txt files) in directory | ```find ./ -name "*.txt" print``` |
| | find all .txt files in home directory |```find "$HOME/" -name "*.txt" print```|

### grep 

| command | description | example |
:----------|:-------------|:----------|
|```grep```| find occurences of a pattern in a file|```grep 'a' file1```|
| |find occurences of a pattern regardles of case|```grep -i 'a' file1```|
| |find number of occurences|```grep -c 'a' file1```|

### jobs 

| command | description | example |
:----------|:-------------|:----------|
| ```jobs```|lists jobs waiting or running in the background (numbered like "%1,%2,%3,etc.") |```jobs``` |
| |start job 4 again |```%4``` |

### kill 

| command | description | example |
:----------|:-------------|:----------|
|```kill```| kill a specific job|```kill %4``` |

### less/more 

| command | description | example |
:----------|:-------------|:----------|
|```less/more```|these commands allow you to preview a file (NOT A BINARY FILE!!!) and go through it by hitting enter or space. leave the preview by pressing ```q``` |```less``` |
| | |```more``` |

### ls 

| command | description | example |
:----------|:-------------|:----------|
|```ls```|see files in directory |```ls``` |
| |see invisible files in directory (those starting with "." like a ".bashrc" file) | ```ls -a``` |
| |see permissions and invisible files|```ls -la``` |

### man 

| command | description | example |
:----------|:-------------|:----------|
|```man```|get the documentation for a command, for example ```ls``` |```man ls``` |

### mkdir 

| command | description | example |
:----------|:-------------|:----------|
|```mkdir```|make a directory |```mkdir newdir``` |
| |make a directory in another folder|```mkdir /home/folder1/newdir``` |

### mv 

| command | description | example |
:----------|:-------------|:----------|
| ```mv```|rename a file, does not save the original|```mv -i oldname newname``` |

### ps 

| command | description | example |
:----------|:-------------|:----------|
|```ps```|what files are running? |```ps``` |

### pwd 

| command | description | example |
:----------|:-------------|:----------|
| ```pwd```|print the working directory |```pwd``` |

### rm 

| command | description | example |
:----------|:-------------|:----------|
|```rm```|to **PERMANENTLY** remove a file |```rm file1``` |
| | to **PERMANENTLY** remove a directory |```rm -r /home/folder1/``` |

### rmdir 

| command | description | example |
:----------|:-------------|:----------|
| ```rmdir```| also **PERMANENTLY** removes a directory| ```rmdir /home/folder1/```|

### sed 

| command | description | example |
:----------|:-------------|:----------|
|```sed```|replace pattern with another pattern in a file - here we replace "no" with "FALSE" |```sed 's/no/FALSE/g' file1``` |
| | replace pattern with nothing |```sed 's/no//g' file1```|

### sort 

| command | description | example |
:----------|:-------------|:----------|
| ```sort```| sort by first column| ```sort file1```|

### vi 

| command | description | example |
:----------|:-------------|:----------|
| ```vi```|open a text editor. hit ```i``` to start writing, ```Esc``` then ```:wq``` then ```Enter``` to leave and save | ```vi filetocreate```|


!!! abstract "References"

    1. [University of Indiana Unix Command Introduction](https://kb.iu.edu/d/afsk)
    2. [bioinformatics oneliners](https://github.com/stephenturner/oneliners)
    
