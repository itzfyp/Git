# Create a file and check status of it

### Create New file

Now create any file you want in your local. Here we are creating a text file for demo

```text
➜ firstFile.txt

Hello, Here we are creating a new text file for demo.
```

Now you have a file with some text. Check the status of your changes that git tracks.

```text
➜ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	firstFile.txt

nothing added to commit but untracked files present (use "git add" to track)
```

Here you can see your files `firstFile.txt`  under Untracked files section. Which means untracked files are not yet able to get converted to a Git commit. Only Staged files will be available for next or future commit.

Only new files will come under Untracked files section. Modified files will come under `Changes not staged for commit` section with modified flag on before each files. like below

```text
➜ git status
On branch master

No commits yet

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
  
  modified: firstFile.txt
  
nothing added to commit but untracked files present (use "git add" to track)
```

In next section we will see how to move new files or modified files into staging area.

