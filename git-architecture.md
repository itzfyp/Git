# Git Workflow

### Git files structure

Git has three main sections which illustrated in below picture

![Git files lifecyle \(source by: https://git-scm.com/ \) ](.gitbook/assets/git-scm.png)

`git directory` git stores your codes \( metadata and object data \) in git directory while cloning from remote repository.

`working directory` when we are checking out a branch, git will pull out a copy of stored code from git directory and store in local system for you to use or modify.

`staging area` this is a simple file to store the information modified files which will go into your next commit.

### Git workflows on users actions

| Users Do | Git Does |
| :--- | :--- |
| clone / create repository | It stores the cloned / created repository in git directory in local disk. |
| checkout a branch | Git will pull a copy of that branch from git directory. Original code / branch will be prevented from being modified. |
| stage changes | If we stage modified / new files, Git will store those files in staging area. which will be used later in commit phase. |
| commit changes | Git takes the files as they are in the staging area and stores that snapshot permanently to your Git directory. |

## Reference

