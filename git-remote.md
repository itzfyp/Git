# git remote repo's

### What is Remote repository

Remote repositories are your project that hosted in internet or network somewhere.

### How to get remote repo's

We can connect remote repos with our local git via path \( http or ssh \) where your code hosted. 

First we need to check that any repos are already added. To check, you have to specify below comments in command line

```text
git remote -v
origin	https://github.com/schacon/ticgit (fetch)
origin	https://github.com/schacon/ticgit (push)
```

`git remote -v` which shows you the URLs that Git has stored for the short name to be used when reading and writing to that remote.

`origin` is the short name which will discuss later in this chapter

`https://github.com/schacon/ticgit` is the path or URL \( https or ssh \)where your repos hosted.



