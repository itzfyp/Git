# Create a file and check status of it

### Create New file

Now create any file you want in your local. Here we are creating a text file with some text.

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



