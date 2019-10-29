# Git Setup

### Download Git

[Here](https://git-scm.com/downloads) you can find Git for your machine \(mac / windows\) 

### Update if Git installed already

if you have installed git already in your system, you can update git to latest version by using this commands in command line or terminal.

```text
git clone https://github.com/git/git
```

### Set Your Name and Mail in Git Config

After everything is set up and you have “git” in your PATH environment variable, then the first thing you have to do is to config git with your name and email. \(_Note : here you are going to set name and email at system level. Not user / repo specific. More details is_ [_here_](git-config.md)_\)._

#### Configure your name

```text
git config --global user.name "kyle symson"
```

#### Configure your email 

```text
git config --global user.email "getify@gmail.com"
```

#### What is the use of configuring name and mail ?

Whenever we commit a code , git will indicate that who are doing commit with name and email configured already. It will help us to know who has committed.

In future, at any time we can update the user details.

Want to know more about configuration, [click here](git-config.md) 

