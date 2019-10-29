# Understanding level of Git Configuration

Git comes with many useful configuration variables. And it lets us to set and get configuration variables that controls how git looks and controls. We can set and get those configurations at three levels.

* System
* User / Global
* Repository

### System level \(--system\)

System-level covers an entire user, entire machine and all repos. While editing at this level, the changes can be seen all over the places, i.e., every repo level can be affected. _So, editing the configuration level in the system is often discouraged._

```text
git config --system <key> <value>
```

#### location of system configuration

for windows users `C:\ProgramData\Git\config` 

for mac / linux users `~/etc/gitconfig`

### User level \(--global\)

User level configuration is user-specific, meaning it is applied to an operating system user.

```text
git config --global <key> <value>
```

#### location of user configuration

for windows users  `C:\Users\<username>\.gitconfig` 

for mac / linux users `~/.gitconfig`

### Repository level \(--local\)

Repository level is the level which is specific to the repository. For example, if you have cloned any project from GitHub then by default git config will write on the local level when no configuration is passed.

```text
git config --local <key> <value>
```

#### location of local configuration

 It can be found in the repo's .git directory: `.git/config` 

_To know more about list of configuration available, Please go though_ [_git configuration list_](git-set-config.md)_._

