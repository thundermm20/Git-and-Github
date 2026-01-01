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

# Branch
${\color{blue}\text{Branch}}$ - This is used check branch.

    git branch

# Branch -M
${\color{blue}\text{Branch -M}}$ - To rename branch.

    git branch -M <Name>

# -u  in Push
${\color{blue}\text{-u}}$ - In git push it is used to set stream which means we work on that project for long time.

    git push -v origin main

