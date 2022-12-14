
Youtube - https://youtu.be/ZtqBQ68cfJc

Linux Commands

    whoami              -  username of the currently logged in user
    man                 -  manuals for commands (man <command>)
    clear               -  clears the terminal screen
    clear -x            -  clears the terminal screen without clearing the history
    ctrl^l              -  same operation as "clear -x"
    pwd                 -  print name of the current/working directory
    ls                  -  list the contents of the directory
        ls -l           -  use a long listing format
        ls -a           -  does not ignore entires starting with .
    cd                  -  change directory (created by shell)
        cd ..           -  go to the parent directory (one level)
        cd ~            -  go to the home directory
        cd /            -  go to the root directory
    find                -  list all the directories with their paths
    mkdir               -  create a new directory
    mkdir /path         -  creates a directory in the specified path
    mkdir -p            -  create any necessary parent directory
    touch               -  to create empty files / change file timestamps
    rmdir               -  to remove only empty directories
    rm                  -  to permanently remove files
        rm -v (verbose) -  shows the list of the removed files
        rm -r (recurse) -  to remove directories and their child directories
        rm -ri (decide) -  to verify every file 

    mv (oldname) (newName)                 -    to rename files
    mv (file) (destination)                -    to move files 
    cp (parentFile) (Destination)          -    to save a copy of a file in the destination
    more                                   -    to view the contents of the file
    head (filename)                        -    to view the head part of the file 
    tail (filename)                        -    to view the tail part of the file
    date                                   -    to view the date
        date > (filename)                  -    to save the date in the directory (overwrites the file)
        date >> (filename)                 -    to save without overwriting 
    cat                                    -    prints the entire contents of the file / contcatenate files
        cat (file1) (file2) > (file3)      -    concatenate two files and save it in the third file
                                                can also be used to send the concantenated files to other commands
        cat -n                             -    prints the output with the number of lines    
    less (filename)                        -    opens the file in a viewable format with a search dialog box
                                                (space) - to go down a page
                                                (b)     - to go up a page
                                                (G)     - to go to the end of the file
                                                (g)     - to go the start of the file
                                                (q)     - to quit and go to the terminal 
    echo                                   -    outputs the given text
        echo >> (output file)              -    saves the conent and redirect to a new file 
    wc                                     -    no of lines / no of words / no of bytes / name of the file
        wc -c                              -    prints the number of bytes
        wc -m                              -    prints the number of characters
        wc -l                              -    prints the number of lines

Piping "|"

    Taking the output of one command and passing it as the input of another command

syntax

    cat (file1) (file2) | wc -l > numbers.txt // saves the number of lines from the concatenation of file1 and file2 and saves it in number.txt

sort                                    -    sorts the items in alphabetical order and case sensitve 

    sort -f  (filename)                 -    ignores the uppercase while sorting; for numbers with first character 
    sort -n      ""                     -    sorts numerically
    sort -n      ""                     -    sorts the numbers in descending order
    sort -un (filename)                 -    sorts the unique numbers / filenames

uniq                                    -    report or omit adjacent repeated lines (usually used with sort) 
    
    sort (filename) | uniq              -    best practice to remove all the duplicates
    sort (filename) | uniq -d           -    to print only the one with duplicates    
    sort (filename) | uniq -u           -    to print only the one without duplicates    
    sort (filename) | uniq -c           -    to print the duplicates with the count 

    sort (filename) | uniq -c | sort -nr > (newfile)    - sorts the items in the file; counts the unique elements; sorts them with the count; and save them in the file 

path name expansion

        echo *.txt                          -     shows all the files in the format txt (matching path names)
        echo *.??                           -     shows all the files that end with two charcter extensions
        rm *.???                            -     to remove all the files that end with three character expansion

touch {a,b,c,d}.txt                     -     creates a.txt b.txt c.txt d.txt files 

ls (filename).*                         -     lists all the files with the same filename without the extension
     
echo {1..99}                            -     expands from 1 -> 99

mkdir {1..99}.txt                       -     creates (1.txt -> 99.txt) 99 directories
     
diff (firstFile) (secondFile)           -     to find the difference between two different files 

diff -u (fileName1) (fileName2)         -     to get the detailed view of the changes 

                                           
time 2:21:20 

find   // big concept  

    to find files and directories 

        find . -name '*.js'             -   To find all the files under the current tree that have the .js extension and print the
                                            relative path of each file 

        find . -type d -name '*E*'      -   to find all directories which has uppercase E in it  // d for directory 
        find . -type f                  -   to find all files                                    // f for files 

    can be used with -or and -not operators and so on 

grep    // big concept 

    helps to find text inside the file 

        grep TEXT filename              -   shows the TEXT located in the file 
        grep -r TEXT .                  -   lists and shows all the location of TEXT in all directories
        grep -ri TEXT .                 -   lists and shows all the location of TEXT in all directories without case sensitive

sizes of files and folders

    du                                  -   to find the sizes of the directories
        du filename                     -   to find size for a particular directories
        du -m                           -   to find the size on megagbytes
        du -mh                          -   to find the size on megagbytes in a human readable format 
        du -h | sort -h                 -   to sort all the file in the . sorted by size from small to big

    df  
        df -h                           -   to list long record of the sizes of files and directories
                    

















   

 