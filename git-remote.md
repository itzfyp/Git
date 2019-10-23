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

`origin` is the short name which will discuss later in this chapter

`https://github.com/schacon/ticgit` is the path or URL \( https or ssh \)where your repos hosted.

Here you have connected with one repo. But your are seeing two paths. What is this!.

* `fetch` - to pull code from remote repo.
* `push`  - push your commits to remote repo.

#### what if there is no remote repo connected

~~nothing will be displayed~~



