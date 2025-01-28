# Getting on Board With Git

Git offers a variety of advantages to its users, including:

- Rolling back changes
- Rolling forward changes
- Mitigating competing versions of the same file.
- Tracking changes for multiple fiels.
- Recording only the changes made rather than saving entire separate versions of each file.
- And many more ...

# Installing Git

Follow directions provided on git-scm.com

```bash
git --version
```

# The Project at Hand

You were just hired to manage all of the blog content for a media company called Gorilla Army.

To start, create a directory on your desktop called GA-Blog.

To take advantage of Git superpowers, we have to add a hidden to add a hidden directory called .git/ to our project directory, which contains all of the data Git needs to operate. This is called "initializing".

Next, navigate to the GA-Blog directory you just created and run this command:

```bash
$ git init
```

# Status Update

Ask Git to give us an update on our project's status.

```bash
$ git status
```
Each save we make to our repository is called commit; this message is telling us that our project has no unsaved changes.

# Make a File

Let's use touch command

```bash
$ touch post.txt
```

Then, check the status again.

```bash
$ git status

On branch master

Initial commit
Untracked files:
  (use "git add <file>..." to include in what will be committed)
  post.txt
nothing added to commit but untracked files preset (use "git add" to track)
```

# Staging

To add this chnage to your next commit, you'll use the git add command.

```bash
$ git add post.txt
```

The command is add, but we describe the operation by saying that the file has been "staged". In other words, it has been added to the list of changes that will be officially saved with our next commit.

The files on this list aren't final, and any of these changes can be removed, or "unstaged".

```bash
$ git status
```

# For Efficiency's Sake

Instead of specifying each file, you can write git add ., which will add all of the files in the working directory to the next commit.

```bash
$ git add .
```

<img width="501" alt="image" src="https://github.com/user-attachments/assets/c66230af-8437-44ee-9593-9ef68a0e74e7" />


```bash
$ git log
```

This will yield a list of entried that looks like this:

```
commit 6d33f525a09b9918f75188db164ea2722039830b
Author: Sarah <sarah@gmail.com>
Date: Wed Jan 28 17:44:03 2015 -0500
added a new post
```

<img width="525" alt="image" src="https://github.com/user-attachments/assets/8a2d3f70-7834-4de9-9b5f-d0e82d0599c4" />
