# Git remote repo's

### What is Remote repository

Remote repositories are your project that hosted in internet or network somewhere.

We can connect remote repos with our local git via path \( http or ssh \) from hosted network.  We will see how to handle remote repos soon. 

### Check existing repos

First we need to check that any repos are already added. To check, you have to specify below comments in command line

```text
git remote -v
```

your will see list of remotes if git connected with repos like below

```text
> origin	https://github.com/schacon/ticgit (fetch)
> origin	https://github.com/schacon/ticgit (push)
```

`git remote -v` which shows you the URLs that Git has stored for the short name to be used when reading and writing to that remote.

`origin` is default short name for repo. which we can reference this later to pull or push code.

`https://github.com/schacon/ticgit` is the path or URL \( https or ssh \)where your repos hosted.

Here you have connected with one repo. But your are seeing two paths. What is this!.

* `fetch` - to pull code from remote repo.
* `push`  - push your commits to remote repo.

#### Tips

You will encounter below message if there is no repo available in current directory

```text
git remote -v
> fatal: not a git repository (or any of the parent directories): .git
```

### Add new repos

At first time, if we clone a repo from remote repository like below. Git will pull those code and store them in local. Now your new repo added implicitly into git remote.

```text
git clone https://github.com/schacon/ticgit
```

By default Git will assign a short name for that repo called `origin`

Now follow the section that we discussed above in **`Check existing repos`**_t_o verify that repo is added or not

#### How to add remote manually

Git has commands to handle the remote manually. Below are the commend to add a new remote repo.

```text
git remote add <shortname> <url>
```

`shortname` -  A short name for a repo. which we can reference this later to pull or push code.

`url` - Remote path \(https or ssh \) of repo

example

```text
git remote add testShortName https://github.com/paulboone/ticgit
```

_Using this command we can add as many as remote repos with git_

```text
git remote -v
> origin	https://github.com/schacon/ticgit (fetch)
> origin	https://github.com/schacon/ticgit (push)
> testShortName	https://github.com/paulboone/ticgit (fetch)
> testShortName	https://github.com/paulboone/ticgit (push)
```

#### Tips 

if you try to add a remote with a name that already exists in your local, You may encounter below message.

```text
git remote add origin https://github.com/octocat/Spoon-Knife
> fatal: remote origin already exists.
```

### Remove remote repos

If you want to remove a remote for some reason  that you’ve moved the server or are no longer using a particular mirror, or perhaps a contributor isn’t contributing anymore 

 you can use either of below command which expects one argument which is your remote name.

```text
git remote remove <shortName of your remote>
        (or)
git remote rm <shortName of your remote>
```

_**Note :** Above commend does not delete the remote repository from the server. It simply removes the remote and its references from your local repository._

**Tips** 

If you try to remove a remote which doesn't exist in remote server or network, You may encounter below message.

```text
 git remote rm nonExistantRepo
 > error: Could not remove config section 'remote.sofake'
```

### Update remote repos

#### Change remote url

To change an existing remote path with new one, we can use below commands.

```text
git remote set-url <existing remote name> <new remote url / path>
```

example

```text
git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
git remote set-url myrepo git@github.com:USERNAME/REPOSITORY.git
```

_**Note :** The next time you `git fetch`, `git pull`, or `git push` to the remote repository, you'll be asked for your GitHub username and password_

**Tips**

You may encounter these errors when trying to change a remote.

```text
git remote set-url sofake https://github.com/octocat/Spoon-Knife
> fatal: No such remote 'sofake'
```

#### Change remote name

To change or update an existing remote names, below commands are used

```text
git remote rename <existing remote name> <new name for the remote>
```

**Tips**

if you entered wrong name or made any typo's while entering , you will encounter below message

```text
git remote rename oldnam'ee newname
> Could not rename config section 'remote.[old name]' to 'remote.[new name]'
```

### Where can i these configuration in my system

If you go to your local repository folder in your system, 

There you have a hidden folder in the name of `.git`. This folder has all details of your repo. 

There you have a file named `config`. You can view and edit configuration available in config file. which will reflect to that particular repo only. Other repos will not get affected.

