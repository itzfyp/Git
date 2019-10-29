# git config lists

Git has lots of options which we can configure. Some of  configurations explained below.

#### **user**

this option has two properties to configure commit details of git user.

* `user.name`  : it is used to set up Git with your name.
* `user.email` : it is used to set up Git with your email

example

```text
git config --global user.name "<Your-Full-Name>"
```

```text
git config --global user.email "<your-email-address>"
```

#### color

Git fully supports coloured terminal output.It allows to change the theme of terminal.

* `color.ui` : It turns on and off all Git’s coloured terminal output
* `color.*`   : it  will list out all available options, where we can turn on /off specific options coloured settings

```text
git config --global color.ui auto
```

```text
git config --global color.*
> color.branch
> color.diff
> color.interactive
> color.status

git config --global color.branch false
```

#### core

Core has some of features which will be used in tracking, commiting time

* `core.excludesfile` ****: It allows to add `.gitignore` files at any level
* `core.editor`       : it tells git to choose which editor can be used to edit or add commit message

```text
git config --global core.excludesfile ~/.gitignore_global
```

```text
git config --global core.editor emacs
```

[Click](https://git-scm.com/docs/git-config) here to learn more about list of options available in git configuration Official site. 

