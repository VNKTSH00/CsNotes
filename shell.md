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
