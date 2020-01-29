# git-notes

## Install and Configure
- Install using Homebrew
```
$ brew install git
```

- Verify
```
$ git --version
git version 2.9.2
```

- Configure
```
$ git config --global user.name "Jose Dalino"
$ git config --global user.email "hello@example.com"
```

- Add .gitgnore file

## Repositories
- Turn an existing directory into a git repositoru
```
$ git init
```

- Clone (download) a repository
```
$ git clone https://[URL].git
```

## Branching
- Create a new branch
```
$ git branch [branch-name]
```

- Switch to a specified branch
```
$ git checkout [branch-name]
```

-  Combines the specified branch’s history into the
current branch. This is usually done in pull requests,
but is an important Git operation.
```
$ git merge [branch]
```

- Deletes the specified branch
```
$ git branch -d [branch-name]
```

## Synchronize changes
- Downloads all history from the remote tracking branches
```
$ git fetch
```

- Combines remote tracking branch into current local branch
```
$ git merge
```

- Uploads all local branch commits to GitHub
```
$ git push
```

- Updates your current local working branch with all new commits from the corresponding remote branch on the remote repo. git pull is a combination of git fetch and git merge
```
$ git pull
```

## Making Changes
- Lists version history for the current branch
```
$ git log
```

- Lists version history for a file, including renames
```
$ git log --follow [file]
```

- Shows content differences between two branches
```
$ git diff [first-branch]...[second-branch]
```

- Outputs metadata and content changes of the specified commit
```
$ git show [commit]
```

- Snapshots the file in preparation for versioning
```
$ git add [file]
```

- Records file snapshots permanently in version history
```
$ git commit -m "[descriptive message]"
```

## Redo Commits
- Undoes all commits after [commit], preserving changes locally
```
$ git reset [commit]
```

- Discards all history and changes back to the specified commit
```
$ git reset --hard [commit]
```
