Git 

Three main areas

    1. Working Directory
    2. Staging index
    3. Repository

Version Control System (VCS) or Source Code Manager (SCM)

        A VCS allows you to revert files back to a previous state, revert the entire project back to a previous state,
    review changes made over time, see who last modified something that might be causing
    a problem, who introduced an issue and when, and more. 

Commit (SnapShot)

        Git thinks of its data like a set of snapshots of a mini file system.
    Every time you commit, or save the state of your project in Git, it basically takes a
    picture of what all your files look like at that moment and stores a reference to that
    snapshot. 

Repository (Repo)

    A directory that contains your project work, as well as a few files which are used 
    to communicate with Git. Repositories can exist either locally on your computer or 
    as a remote copy on another computer.

Working Directory

        The files that you see in your computer's file system. When you
    open your project files up on a code editor, you're working with files in the Working
    Directory. This is in contrast to the files that have been saved (in commits!) in the repository.
    When working with Git, the Working Directory is also different from the command line's
    concept of the current working directory which is the directory that your shell is
    "looking at" right now.

Checkout

        When content in the repository has been copied to the Working Directory. It
    is possible to checkout many things from a repository; a file, a commit, a branch, etc. 

Staging Area or Staging Index or Index

        A file in the Git directory that stores
    information about what will go into your next commit. You can think of the staging area
    as a prep table where Git will take the next commit. Files on the Staging Index are
    poised to be added to the repository.

SHA

        A SHA is basically an ID number for each commit. It is a 40-character string
    composed of characters (0???9 and a???f) and calculated based on the contents of a file or
    directory structure in Git. "SHA" is shorthand for "SHA hash". A SHA might look like this: 
    moving updated/changed files

Branch

        A branch is when a new line of development is created that diverges from the
    main line of development. This alternative line of development can continue without
    altering the main line.
    Going back to the example of save point in a game, you can think of a branch as where
    you make a save point in your game and then decide to try out a risky move in the
    game. If the risky move doesn't pan out, then you can just go back to the save point. The
    key thing that makes branches incredibly powerful is that you can make save points on
    one branch, and then switch to a different branch and make save points there, too
    Working Directory -> Staging Index -> Repository (Saved area)

Git Id

    Git creates a seven digit ID(SHA) for every commit inorder to access previous versions

Configuring the terminal

    cd -> to go to home directory
    mv -> moving directory can be also used to change the directory or filename

GIT Bash Commands

    git init  (repo name)            - create a new repository in local computer
    git clone (url of the project)   - clone or copy a repository from web
    git status                       - to check the status of the repository

    ls                               - used to list all the files and directories
    mkdir                            - used to create a new directory
    cd                               - used to change directory
    git -rf                          - used to remove git files and repositories

    git log                          - to view the logs of all the commits made
    git log --oneline                - To view all the list of commits made  
    git log -p                       - To view where the changes were made in the commit (patch command)
    git log --decorate               - to view the hidden elements like tags in the command line 

    git push [variable name]         - sends the commited changes of master branch to the remote repository  
    git push --all                   - pushes all branches to the remote repository 

    git add  (fileName)              - adds file to staging area
    git add .                       - to add all the repos 
    git commit -m (message)          - to records or snapshots the file permanently for version history 
    git diff                         - shows the differences which are not yet staged 

    git tag -a (tagName) (SHA)       - to adds to specific commits (-a = this flag tells Git to create and annotated flag)
    git tag                         - displays all the tags available in the repository 
    git tag -d (name)               - to delete a tag
    git tag --delete (name)         - to delete a tag
    git tag -a beta (tagName)      - to add tag to the recent commit 

    git checkout (branch name)       - to change the branch 
    git checkout -b (branch name)    - creates a new branch while checking out (-b flag is used to create a new branch)
    git branch                       - shows the current working branch 
    git branch (name)                - Creates a branch with the name specified 
    git branch (name) (SHA)          - Creates a branch from the SHA (commit) spcified
    git branch -d (name)             - Deletes the branch with the name specified 

    git merge (branchName)           -   1. look at the branches that it's going to merge
                                            2. look back along the branch's history to find a single commit that both branches have in their commit history
                                            3. combine the lines of code that were changed on the separate branches together
                                            4. makes a commit to record the merge

                                            (The branch being merged in must be ahead of the checkout branch. The checked out branch's pointer will just be moved forward to point to the same commit as the other branch)
                                            (Inorder to merge two branches other than main. checkout to the other branch and run the merge command)

    
MERGE CONFLICT

        Remember that a merge conflict occurs when the exact same line(s) are changed in separate branches. 
    
    git commit --amend                  - To alter the most recent Commit 
    git revert (SHA)                    - to revert the previously made commit 
    git reset (commit)                  - to delete the commit in order 

Reset vs Revert

    At first glance, resetting might seem coincidentally close to reverting, 
    but they are actually quite different. Reverting creates a new commit that reverts or undos a previous commit. 
    Resetting, on the other hand, erases commits!

    git checkout -- .                    - to discard changes in the working directory 
    git reset (reference to commit)      - to erase commit
    git reset --hard HEAD^               - erase the commit last commit  
    git reset --soft                     - moves the commited changes to the staging index 
    git reset --mixed                    - unstages the commited changes 

Here's how we can refer to previous commits:

    The parent commit ??? The following indicate the parent commit of the current commit
    HEAD^ (or) HEAD~ (or) HEAD~1
    The grandparent commit ??? The following indicate the grandparent commit of the current commit
    HEAD^^ (or) HEAD~2
    The great-grandparent commit ??? The following indicate the great-grandparent commit of the current commit
    HEAD^^^ (or) HEAD~3


Stashing 

    Git provides an easy way fof stashing these uncommitted changes so that we can return to them later, without having to make unnecessary commits.
    Stashing can be done multiple times 

    git stash                           - Stashes the uncommited changes
    git stash pop                       - to bring back the uncommited changes stashed before 
    git stash apply                     - To apply whatever is stashed away, without removing it from the stash. This can be useful if you want to apply stashed changes to multiple branches 
    git stash -u                        - If there are untracked files(files that are never tracked with Git) They will not be included in the stash. 
                                        So we can use -u to tel git stash to include those untracked files 
    git stash list                      - To view all the stashes which was done multiple times
    git stash apply stash@{#}           - To apply the specific stash to the required place 
    git stash drop                      - To delete a particular stashes 
    git stash clear                     - To clear out all the stashes 