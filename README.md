# Git Rebase and Squash Cheatsheet

This is quick reference for steps of git rebase and git squash. By reading through online material, I summarize this cheatsheet.

## 1. Starting point:

For now, git should be in your working feature branch and already committed and pushed.

## 2. Run git fetch:

Update local repo from removed repo.

> git fetch

## 3. Run Git Rebase:

Integrate changes from one branch into another.

> git rebase origin/master

## 3.1. Git squash before git rebase:

## 4. Resolve conflict:

During rebase, conflict may happen. After resolving conflict, updated change should add into branch.

> git add .

Then, continue rebase.

> git rebase --continue

If want to cancel rebase.

> git rebase --abort

## 5. Push to remove and update local repo:

Push to removed.

> git push

Force push to removed.

> git push origin <branchName> --force

## 6. Reset local repo:

If use force push, local repo/branch need to reset.

> git reset –hard origin/<branch name>
