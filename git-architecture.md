# Git Workflow

### Git files structure

Git has three main sections which illustrated in below picture

![Git files lifecyle \(source by: https://git-scm.com/ \) ](.gitbook/assets/git-scm.png)

`git directory` git stores your codes \( metadata and object data \) in git directory while cloning from remote repository.

`working directory` when we are checking out a branch, git will pull out a copy of stored code from git directory and store in local system for you to use or modify.

`staging area` this is a simple file to store the information modified files which will go into your next commit.

### Steps followed by Git

| Users Do | Git Does |
| :--- | :--- |
| Clone / Create repository | It stores the cloned / created repository in git directory which available on local disk  |
| checkout a branch | Git will pull a copy of that branch from git directory available. Original code / branch will be prevented from being modified |
|  |  |

## Reference

