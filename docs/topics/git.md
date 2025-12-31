---
title: '- Git'
---

```bash
git branch --delete [local_branch_name]             # Remove local branch
git push origin --delete [remote_branch_name]       # Remove remote branch
git reset --hard                                    # Reset current Head to specified state
git clean -n                                        # Remove untracked files from work tree -- dry run
git clean -f                                        # Remove untracked files from work tree -- force
git clean -f -d -x                                  # Remove untracked files, directories, even ignored

git pull --recurse-submodules && git submodule update --init --recursive

git submodule foreach --recursive 'git checkout main && git submodule update --init --recursive'
git submodule foreach --recursive 'git checkout master && git submodule update --init --recursive'

git submodule foreach --recursive 'git checkout $(git remote show origin | sed -n 's/  HEAD branch: //p') && git submodule update --init --recursive'

git config --global alias.where '!git branch'
git where
```

```bash
git config --global user.name [username]
git config --global user.email [email]
git config --global credential.username [username]
git config --global init.defaultbranch "main"
git config --global --list
```

```bash
git config --local user.name [username]
git config --local user.email [email]
git config --local credential.username [username]
git config --local --list
```