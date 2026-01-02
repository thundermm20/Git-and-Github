# Clone
${\color{blue}\text{Clone}}$ - Cloning a repository on a local machine.

    git clone <-some link->

</b>Example</b>:

    Step-1: Open project in Github

    Step-2: Click on <br>Code
    
    Step-3: Select clone link type(HTTP) and copy link

    Step-4: Enter "git clone https://github.com/account/project.git" and press Enter

Some Terminal Commands:

    cd                      -->   Change/Enter Directory
    cd                      -->   Exit Directory
    mkdir <Folder Name>     -->   Make New Folder
    ls                      -->   List files
    clear                   -->   Clear Terminal
    ls -a                   -->   List all files including hidden

# Status
${\color{blue}\text{Status}}$ - Displays the state of the code.

    git status
<b>Working</b>:
    </br></br>
&bull; When ${\color{blue}\text{Git and Github}}$ have same code

    nothing to commit, working tree clean
&bull; When ${\color{blue}\text{Git and Github}}$ have different code it shows ${\color{red}\text{modified: <-File Name->}}$ with details and Shows ${\color{red}\text{M}}$ mark on explorer.

    Changes not staged for commit:
        (use "git add <file>..." to update what will be commited)
        (use "git restore <file>..." to discard changes in working directory)
            modified: <File Name>

        no changes added to commit (use "git add" and/or "git commit -a")

&bull; When ${\color{blue}\text{Git}}$ has more file than ${\color{blue}\text{Github}}$ then ${\color{red}\text{Untracted Files}}$ status is shown with ${\color{red}\text{U}}$ mark on explorer.

    Untracked Files:
        (use "git add <file>..." to include in what will be commited)
            <File Name>

        no changes added to commit (use "git add" and/or "git commit -a")

${\color{blue}\text{Status Types}}$ </br></br>
${\color{blue}\text{1:- Untracked}}$</br>
New Files that Git  does not yet track</br></br>
${\color{blue}\text{2:- Modified}}$ </br>
Changed</br></br>
${\color{blue}\text{3:- Staged}}$ </br>
File is ready to be commited</br></br>
${\color{blue}\text{4:- Unmodified}}$ </br>
Unchanged</br></br>

# Add
${\color{blue}\text{Add}}$ - Adds new or changed files in your work directory to the Git staging area and show ${\color{red}\text{A}}$ mark in explorer as ready to be commited.

    git add <File Name>      -->     Add specific file

    git add .                -->     Add all files
<b>After adding "git status"</b></br>
After adding the files are ready to be commited and shows as ${\color{red}\text{modified: <-File Name>}}$ and ${\color{red}\text{new file: <-File Name>}}$

    Changes to be commited:
        (use "git restore --staged <file>..." to unstage)
            modified: <File Name>
            new file: <File Name>
# Commit
${\color{blue}\text{Commit}}$ - It is the record of change

    git commit -m "some message"

Then it is saved with screenshot on ${\color{red}\text{Local Machine (PC/Laptop)}}$ and needed to be initialized on Github.

# Push Command

${\color{blue}\text{Push}}$ - Upload Local repo(Git) content to remote repo(Github)

    git push origin main

# Init
${\color{blue}\text{Init}}$ - Init is used to create Git repository.

    git init

Add

    git add .

Commit

    git commit -m "message"
    
${\color{blue}\text{Remote}}$ - It is used to link git to github

    git remote add origin <Link>

${\color{blue}\text{Remote -v}}$ - To verify link.

    git remote -v
    
    Example:- https://github.com/name/repo.git/

# -u  in Push
${\color{blue}\text{-u}}$ - In git push it is used to set stream which means we work on that project for long time.

    git push -v origin main

# Branch
${\color{blue}\text{Branch}}$ - This is used to work on different features of same project separately.

# Git Branch
${\color{blue}\text{Git Branch}}$ - This is used to check branch.

    git branch

# Branch -M
${\color{blue}\text{Branch -M}}$ - To rename branch.

    git branch -M <Name>

# Branch Checkout
${\color{blue}\text{Branch Checkout}}$ - This is used to move from one branch to another (to navigate).

    git checkout <Branch Name>

# Branch Checkout -b
${\color{blue}\text{Branch Checkout -b}}$ - This is used to create new branch.

    git checkout -b <New Branch Name>

# Branch Checkout -d
${\color{blue}\text{Branch Checkout -d}}$ - This is used to delete branch.

    git checkout -d <Branch Name>

# Pull Command
It is used to fetch and download content from a remote repo and immediately update the local repo to match that content.

    git pull origin main

# Branch Merge
It refers to merging of two branches.

${\color{blue}\text{MERGE WITH PULL REQUEST}}$</br>
It lets you tell others about changes you have pushed to a branch  in a repository on Github. It also helps to check whether changes are applicable after reviewing by senior developer.

    Step-1: Open branch which you want to merge.

    Step-2: Click on Compare or pull request.
    
    Step-3: It opens view if branches are mergeable or not & which branch is going to merge whom.
    
    Step-4: Write pull request name(write comment).
    
    Step-5: Click on Create pull request.
    
    Step-6: Then Github check if it is automatic mergeable
    
    Step-7: Click on Merge pull request.
    
    Step-8: Click on Confirm merge and new commit is added with name and description.
    
    Step-9: Then it show message of succession.
    
    Step-10: Then same changes will be shown in both branches

# Merge Conflicts
It is an event that takes place when Git is unable to automatically resolve differences in code between two commits.

${\color{blue}\text{MERGE WITH GIT}}$</br>
It is used to merge branches in local repository and solve merge conflicts.

${\color{blue}\text{Diff}}$ - It is used to differentiate one branch from another. In simple words, it is used to compare commits, branches, files & more.

    git diff <Branch Name>

${\color{blue}\text{Merge}}$ - It is used to merge one branch to another locally.

    git merge <Branch Name>

It shows conflicts occuring during merging branches. And provide overview to solve it with options.

    <<<<<<< HEAD (Current Change)
    <p>(dropdown)</p>
    =======
    <p>(button)</p>
    >>>>>>> main (Incoming Change)

    Options:
        Accept Current Change
        Accept Incoming Change
        Accept Both Changes
        Compare Changes

Now we can simply add, commits and merge changes

# Log
It is used to view commit logs

    git log

# Undoing Change
${\color{blue}\text{Case 1}}$ - Staged Changes<br>
These are the changes which are added but not commited. Reset is used to undo add.

    git reset <File Name>

    git reset

${\color{blue}\text{Case 2}}$ - Commit Changes (For One Commit)<br>
These are the changes which are added and commited both. Reset HEAD~1 is used to undo one commit.

    git reset HEAD~1

${\color{blue}\text{Case 3}}$ - Commit Changes (For Multiple Commits)<br>
These are the changes which are added and commited both. These are is used to undo multiple commits.

    git reset <Commit Hash>      Hash example: 32h2h23jk34jj324bh3h

Reset --hard is used to also make changes in the VS Code.

    git reset --hard <Commit Hash>

# Fork
A fork is a new repository that shares code and visibility settings with the original "upstream" repository. Fork is a rough copy.

    Step-1: Open project code which is going to fork.
    Step-2: Click on Fork.
    Step-3: When Create a new fork shows, do changes if needed.
    Step-4: Click on Create fork.
    Step-5: Now all project code will be fork.