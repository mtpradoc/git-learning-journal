# Git Basic Commands

## Install VSCode and Set Up 'code' Command in Terminal
I think VSCode is one of the main tools one have to have installed while trying to work with Git. VSCode comes with git if you are using Mac, if using Windows install git and gitbash.

- Open Visual Studio Code
- Open the Command Palette by pressing **cmd + shift + P**
- Install 'code' command in PATH by typing **Shell Command: Install 'code' command in PATH**
- Select the option and press Enter
- Restart the terminal

## Let's create our working folder
Let's create a folder and in order to be able initialize git

Create a folder
```bash
$ mkdir git-project
$ cd git-project
```

Open a new instance of Visual Studio Code
```bash
$ code ./
```

## Initial Git Configuration
Let's add our information to track our authoring

```bash
$ git config --global user.name "username"
$ git config --global user.email mymail@mail.com
```

## Let's Initialize Git
We can initialize a new repository just by being local.

```bash
$ git init
```

## Understand HOW Git Track File Status
Git tracks the lifecycle of files in three primary stages: modified, staged and commited. Understanding these stages will help you better manage your code and work effectively in version control.

1. Mofified (Unstaged)
When a file is modified (shown as M in Git), it means you've made changes to the file, but those changes have not yet been staged or commited. The file is stil in your working directory, and Git is aware of the changes but has not done anything with them yet.

```bash
$ git status
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
    M  example.py
```

Let's see this part. Tracked modified file:
```bash
M  example.txt (staged for commit)
```

When we have add a new U (untracked) file
```bash
U  newfile.txt
```

2. Staged (Ready to be Commited)
When you stage a file, it means you are telling Git that you're ready to include the changes in the next commit. This is done with the git add command.
Staging prepares the file changes, but they are not yet committed. Think of this as a "pre-commit" stage where Git is ready to track the changes.

```bash
$ git add index.html
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
    modified:   index.html
```

Staged the modified file:
```bash
M  example.txt (staged for commit)
```

Staged new file
```bash
A  newfile.txt
```

3. Commited (Confirmed - Saved to Local Repository)
Once the changes are committed, they are stored in Git's local repository, and the file is now officially part of the project's version history. Committing a file is akin to taking a snapshot of the current state of your project.

```bash
$ git commit -m "feat: initial file"
```
Let's review git tracking status
```bash
$ git status
On branch main
nothing to commit, working tree clean
```