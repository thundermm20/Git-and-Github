# Git
Version Control System is a tools that helps to track changes in code.

Git is a ${\color{blue}\text{Version Control System}}$. It is:
</br>
&bull; Popular</br>
&bull; Free and Open-Source</br>
&bull; Fast and Scalable</br>
&bull; Track History</br>
&bull; Collaborate</br>

# .gitignore
In this files names are saved of those files which we don't want to push to github

    # In .gitignore

    .env
    node_modules

# .gitkeep
This file is used to keep empty folders without content, which git & github generally ignores.

# Rebase
It is used to update code which is going on previous commit branch to new branch.

    git rebase <Branch Name>

Update code without commit.

    git rebase --continue

# Reflog
It is a commant that shows history of the commit. It allows to see the changes that have made to repository over time.

    git reflog

Find Specific Commit

    git reflog <Commit Hash>