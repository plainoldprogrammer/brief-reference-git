# Brief Reference Git
Brief reference of the Git control version system.

---

#### Create a git new repository
```
$ git init
```

#### Show the current status of the repository
```
$ git status
```

#### Add all the modified files to the stage
```
$ git add --all
```

#### Commit with a message the files on the stage
```
$ git commmit -m "message of the commit"
```

#### Show the log
```
$ git log
```

#### Show the latest 2 commits
```
$ git log -n2
```

#### Modify the comment of the last commit
```
$ git commit --amend
```

#### Show the commits message in oneline
```
> git log --oneline
```

#### Remove the last commit from git and github
```
> git push -f origin HEAD^:master
```

#### Show the global configuration
```
> git config --global --list
```

#### Show the local configuration
```
> git config --local --list
```

#### Unset a specific configuration
```
> git config [<file-option>] --unset-all name [value_regex]

Example:
> git config --global --unset-all core.pager
```

#### Create a git tag
```
> git tag -a v1.0 -m "Version v1.0 (Stable)"
```

#### Push a git tag
```
> git push origin <tagname>
```

#### View the diff of the just added files
```
> git diff --staged

or

> git diff --cached
```

#### Correct the last commit message local and in github
```
> git commit --amend

> git push --force origin
```

#### Show the changes of a specific file
```
> git diff mainwindow.h
```

#### Get the sha1 of an object
```
> echo "Apple Pie\n" | git hash-object --stdin

or (is different)

> echo Apple Pie\n | git hash-object --stdin
```

#### Create a hash object in the current git directory
```
> echo "Apple Pie 2" | git hash-object --stdin -w
```
