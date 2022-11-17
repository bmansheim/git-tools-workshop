# Git tools workshope

Get your git on!

## What's inside

We're going to go through some

**great tips** for using git, GitHub, VS Code so you can

**leverage the tools** to

**get things done**!

## Agenda

- Quick review of git concepts
- Tips and tricks in git, GitHub, and Visual Studio Code
- More fun with Docs-as-code

## Git concepts

- **git** : an open source, distributed version-control system
- **repository** : a container for your project's files and their revision history
- **remote** : a common repository on GitHub that all team member use to exchange their changes
- **fork** : a copy of a repository on GitHub owned by a different user
- **clone** : a local version of a repository, including all commits and branches
- **commit** : a snapshot of your repository with incremental changes
- **branch** : a collection of commits
- **pull request (pr)**: a comparison between branches with reviews and comments
- **GitHub** : a platform for hosting and collaborating on Git repositories
- **CLI** : Command-line interface such as terminal and cmd
- **IDE** : Integrated development environment such as Visual Studio Code and Atom

Definition of terms

## Git concepts

The workflow

## Git concepts

Git branches

## Git concepts

Show me please?

## Tricks

VScode: Command palette

VScode: Use palette to transform to Title case

GitHub: GitHub CLI

Git: Git aliases

Git: Amend to fix last commit

Git: Prune remote branches

GitHub: Go to file \> press . (period) to open VS code

## VScode palette

Ctrl + Shift + P or F1

For example: **Transform case**

## GitHub CLI

https://cli.github.com/

Extend your commands to PRs

```dos
> gh pr create

? Title Fix links to API docs

? Body \<Received\>

? What's next? Submit

branch 'fix-404-enable-storage' set up to track 'origin/fix-404-enable-storage'.

To https://github.com/bmansheim/azure-docs-pr.git

[new branch] HEAD -\> fix-404-enable-storage
https://github.com/MicrosoftDocs/azure-docs-pr/pull/218416
```

## Git aliases

https://githowto.com/aliases

Streamline your cli commands

```dos
git config --global alias.co checkout
git config --global alias.br branch
```

Instead of typing git checkout master, you only need to type: git co master

You could also edit these commands or add more by modifying the ~/.gitconfig file directly:

```dos
[alias]

co = checkout
pr = !gh pr create
com = !git add . && git commit -m
up = push -u origin HEAD
fresh = !git fetch origin && git cm && git pull upstream main && git push origin main
```

## Git Amend

https://github.com/git-tips/tips

Cleanup last commit

Modify previous commit without modifying the commit message

`git commit --amend --no-edit`

Reword the previous commit message

`git commit --amend -m "New commit message"`

## Git remote prune

https://git-scm.com/docs/git-prune

Delete old branches

Modify previous commit without modifying the commit message

```dos
git remote prune origin

URL: https://github.com/bmansheim/azure-docs-pr.git

[pruned] origin/add-ama-aws-onboard
[pruned] origin/d4storage-mgr-review
[pruned] origin/enable-d4storage-cli-ps
[pruned] origin/fix-404-enable-storage
[pruned] origin/patch-1
[pruned] origin/patch-2
[pruned] origin/web
```

Delete local branches

`git br –D add-ama-aws-onboard`

## Online VScode

At your Mom's house?

http://github.com + . (period)

## Continuous Integration/ Continuous Deployment (CI/CD)

GitHub pages

GitHub actions
