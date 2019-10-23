# git remote repo's

### What is Remote repository

Remote repositories are your project that hosted in internet or network somewhere.

We can connect remote repos with our local git via path \( http or ssh \) where your code hosted.  We will see how to handle remote repos soon. 

#### How to check if remote repo's already connected or not

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

#### what if there is no remote repo connected

~~nothing will be displayed~~

### Add new repo

At first time, if we clone a repo from remote repository like below. Git will pull those code and store them in local. Now your new repo added implicitly into git remote.

```text
git clone https://github.com/schacon/ticgit
```

By default Git will assign a short name for that repo path called `origin`

Now follow the section that we discussed above in _**How to check if remote repo's already connected or not** t_o verify that repo is added

#### How do we add remote manually

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

