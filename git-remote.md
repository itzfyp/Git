# git remote repo's

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
origin	https://github.com/schacon/ticgit (fetch)
origin	https://github.com/schacon/ticgit (push)
```

`git remote -v` which shows you the URLs that Git has stored for the short name to be used when reading and writing to that remote.

`origin` is default short name for repo. which we can reference this later to pull or push code.

`https://github.com/schacon/ticgit` is the path or URL \( https or ssh \)where your repos hosted.

Here you have connected with one repo. But your are seeing two paths. What is this!.

* `fetch` - to pull code from remote repo.
* `push`  - push your commits to remote repo.

#### Tips

~~If there is no repos connected, you may encounter below message~~

### Add new repos

At first time, if we clone a repo from remote repository like below. Git will pull those code and store them in local. Now your new repo added implicitly into git remote.

```text
git clone https://github.com/schacon/ticgit
```

By default Git will assign a short name for that repo called `origin`

Now follow the section that we discussed above in **`Check existing repos`** _**``**t_o verify that repo is added or not

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
origin	https://github.com/schacon/ticgit (fetch)
origin	https://github.com/schacon/ticgit (push)
testShortName	https://github.com/paulboone/ticgit (fetch)
testShortName	https://github.com/paulboone/ticgit (push)
```

#### Tips 

if you try to add a remote with a name that already exists in your local, You may encounter below message.

```text
git remote add origin https://github.com/octocat/Spoon-Knife
fatal: remote origin already exists.
```

### Remove remote repos

If you want to remove a remote for some reason — you’ve moved the server or are no longer using a particular mirror, or perhaps a contributor isn’t contributing anymore — you can either use  below command which expects one argument which is your remote name.

```text
git remote remove <shortName of your remote>
        (or)
git remote rm <shortName of your remote>
```

_**Note**: Above commend does not delete the remote repository from the server. It simply removes the remote and its references from your local repository._

**Tips** 

If you try to remove a remote which doesn't exist in remote server or network, You may encounter below message.

```text
 git remote rm nonExistantRepo
 error: Could not remove config section 'remote.sofake'
```

### Update remote repos

To change or update an existing remote names, below commands are used

```text
git remote rename <existing remote name> <new name for the remote>
```

if you entered wrong name or made any typo's while entering , you will encounter below message

```text
git remote rename oldnam'ee newname
# Could not rename config section 'remote.[old name]' to 'remote.[new name]'
```

