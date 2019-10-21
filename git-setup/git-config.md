# git config

Git comes with many useful configuration variables. And it lets us to set and get configuration variables that controls how git looks and controls. We can set and get those configurations at three levels.

* System
* User
* Repository

### System level

System-level covers an entire user, entire machine and all repos. While editing at this level, the changes can be seen all over the places, i.e., every repo level can be affected. _So, editing the configuration level in the system is often discouraged._

```text
git config --system <options>
```

#### location of system configuration

for windows users `C:\ProgramData\Git\config` 

for mac / linux users `~/etc/gitconfig`

### User level



