Shell commands 

    #!/bin/bash                                                         -   shebang 

    which bash                                                          -   to know the path of the bash executer

    sh file_name                                                        -   to the run the script file 
    bash file_name                                                      -   to run the file with bash interpreter // bash -> bourne_again shell
    ls -l                                                               -   to list the long list of the file with its permissions

        -r          -> Read permission 
        -w          -> Write permission
        -x          -> Execute Permission 

    chmod +x file_name                                                  -   to give executable permissions to everywone 

    variable="string"                                                   -   to store string value in the variable
    echo $variable                                                      -   to print the value in the variable 

        -e to use \n                                                    -   to add new line while printing output // use man (comamnd) for more details

    read variable                                                       -   to get input from the user and store it in the varaible
    sleep (time)                                                        -   to pause the terminal for the next action. usually in secs
    declear -p                                                          -   to view the declared statements in the terminal 

IF ELSE statement (syntax)

    if [[ ## == ## ]]                                                   // spaces are mandatory 
    then 
        statement
    else    
        statement 
    fi

    Conditions in IF statement 

    -eq     -       equal 
    -ne     -       not equal
    -lt     -       less than   
    -le     -       less than or equal
    -gt     -       greater than 
    -ge     -       greater than or equal 

    ==      -       equal 
    =~      -       pattern matching

ELSE IF statement 

    if (( ## >= ##))
    then 
        statement 
    elif [[ $## -le ##]]
    then 
        statement
    fi

FOR loop  (syntax)

    for (( initialisation; condition; increment/decrement ))
    do  
        stement
    done

WHILE loop (syntax)

    while [[ condition ]]
    do 
        statement                           // for increment or decrement use double parantheses like (( I-- ))
    done

UNTIL look (Syntax)

    until [[ CONDITION ]]
    do 
        STATEMENTS 
    done

EXIT status

    1 -> false
    0 -> true     // inverse in shell output than normal 

    To view the exit status of the last command -> echo $?

combining commands with ";" 

    [[4 -ge 5]]; echo $? // prints the result after executing the condition

Commenting in shell script 

    // Single Line comment 

    # enter the text here ( starts with a # sign )

    // Multi line comment

    : '  //// single quote

    code or comment 

    '    //// single quote

Arithmetic operations

Declaration

    let c=a+b
    let c=a-b
    let c=a*b
    let c=a/b



ARRAYS

CREATING ARRAYS

ARR=("a" "b" "c")                                           -   creates a array of three elements and stores it in ARR
echo ${ARR[1]}                                              -   prints the first element in array ARR 
echo ${ARR[*]}                                              -   prints the all the elements in array ARR 

