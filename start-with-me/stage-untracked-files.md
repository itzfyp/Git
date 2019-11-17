# Stage Untracked / Modified files

As we see already in Git intro, staging area is an index file which will track the changes of staged files. Git tracks only staged files. So we need to stage all untrakced and modified files.

Here we are going to cover basic commands which mostly used by developers for staging

Git has below commands to move files to stage area.

```text
git add <options>
```

git add command has lots of options to add files. which are

* Add a file
* Add multiple  files
* Verbose
* Add specific set of files
* Add all files from a PATH
* Add all files from repo
* Add forced files

#### Add a file

We can commit a file with its name and format of that file

```text
git add firstFile.txt
```

Tips : if you omit or entered wrong file format, you could see below message

```text
➜ git add firstFile
fatal: pathspec 'firstFile' did not match any files
```

#### Add multiple files

We can add multiple files in single add command.

```text
git add firstFile.txt secondFile.txt home/index.js
```



