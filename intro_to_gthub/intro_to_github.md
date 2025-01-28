# Local Versus Remote

So far, we've been making changes locally by editing files and repostories on our computers. That's all well and good, but what if we want to collaborate with others or back up our files just in case our companies dies?

For that, we need to connect our local repository to a remote one.

Enter GitHub.

<img width="407" alt="image" src="https://github.com/user-attachments/assets/49a91f2c-d5ce-44b0-93f4-586691001dae" />

# Learning Objectives

By the end of this lesson, you'll be able to:

- Define GitHub and its benefits.
- Describe each step of the GitHub flow.

What is GitHub?

GitHub is a company that's famous for the platform it built to manage Git repositories in the cloud.

On GitHub, developers can share their code, comment on it, and reiew changes. It's an implementation of the ame Git software you installed on your computer, but it also comes with some additional features.

In a lot of ways, GitHub is like Dropbox.

You have a folder in the cloud - your remote repository - that syncs with your computer. You can share this remote repository with others, grant them special permissions, and view different versions of your files.

<img width="269" alt="image" src="https://github.com/user-attachments/assets/d5fc077a-4bca-45cb-8fb4-345a08259693" />

# Creating a GitHub Account

To start , let's head over to Github.com. The first think we'll do is create a username by clicking on the field in the upper right-hand corner of the screen.

<img width="781" alt="image" src="https://github.com/user-attachments/assets/13f52697-6aef-4773-b67f-fb894a9ab672" />

# Basic Navigation: Repo Owner

This is what the GitHub interface looks like for a repository

<img width="704" alt="image" src="https://github.com/user-attachments/assets/18d61cfd-966b-4584-a1fb-cfdc3eb3358c" />

Repo Name and Owner describe who owns the repository, the name of the repository, and whether or not it is public or private.

Recall that we referred to Git-enabled directories as repositories or repos. That name applies to projects on GitHub as well.

# Basic Navigation: Overview

Overview dislays the number of commits, branches, releases, and contributors to a particular repository. Selecting any of these options will open a detailed view of your selection.

<img width="703" alt="image" src="https://github.com/user-attachments/assets/e824bbbd-1970-4d2a-83a0-3cee73758119" />

# Basic Navigation: Repository File Structure

Repository File Structure displays the contents of the repository. Selecting any file or directory will open a detailed view of that file and allow you to edit its content directly.

<img width="703" alt="image" src="https://github.com/user-attachments/assets/1557b284-dc73-4210-8d2e-11754c5cfa8f" />

# So, How Do Developers Do This?

Consider a project like Node.js, a JavaScript framework. Node.js is completely open source, which means that anyone can read (and even copy) the code that makes it work.

The source code is publicly available on GitHub.  If you visit the mai repository, you'll see that there are more than 2,000 contributors who have committed changes to Node.js.

Although it's open source and anyone can read or contribute to its code, Node.js is maintained by a company called Joyent. These contributors don't have the ability to edit te original Joyent repository - that wouldn't b very efficient or safe. Someone could accidentally make a change that conflicts with someone else's contributions, causing the code to break. Changes need to be inspected and approved by Joyent before they can officially be added to the project.

# The GitHub Flow

The workflow for contributing to an open-source product or your dev team's project comprises the following steps:

1. Forking
2. Cloning
3. Editing
4. Adding/committing
5. Pushing
6. Submitting a pull request

<img width="506" alt="image" src="https://github.com/user-attachments/assets/ebc1d09d-9958-40b7-a241-20957b15996e" />

# Step 1: Froking

To add a copy of someone else's GitHub repository to your GitHub account, fork it by clicking the Fork button in the upper right-hand corner.

This forked repository is not perfectly identical, but it includes all of the same source files, issues, and commit history. 

By forking Joyent's repository, for example, you now have a full working copy of the Node.js source code to play with. This way, when you break something (which you will), the main repository won't be affected.

# Step 2: Cloning

To make a local copy of a fork, you'll clone the repository. This will save the code on your machine so you can edit it.

To do so, open your terminal, navigate to where you'd like to store the repository, then type:

```bash
$ git clone https://url-to-clone
```

You can find the URL to clone by clicking the green button that says "Clone or download".

<img width="784" alt="image" src="https://github.com/user-attachments/assets/20175b02-c7df-4cb9-abf6-a1e39645ddb6" />

# Step 3: Editing

This is when you make your revolutionary edits to the code and reimagine how Node.js works.

You could do this using a text editor of your choice. Atom and Sublime are some of the some of the most popular.

# Step 4: Adding and Committing

Remember, you're editing the code on you local copy of the repository. We know that any time we do this, we need to use some very important Git commands so that our local copy is protected if we goof up.

Recall these commands:

```bash
$ git add <your-file-name>
$ git commit - m "message"
```

# Step 5: Pushing

Once you've committed these changes, your local repository will differ from your remote repository.

To update your remote repository on GitHub, you have to push those changes using the *git push origin master* command.

If you're curious, here's a brief overview:

- *origin* is a shortcut for the URL of your default remote repository (in this case, the repository on GitHub). You can have many remotes if you want, but we're only going to work with one for now.
- *master* refers to the branch on your remote repository where you are currently adding your changes. We're going to be working on the master branch.

<img width="423" alt="image" src="https://github.com/user-attachments/assets/db1e76c3-ae9f-4ab6-9cfc-bbb858b01d97" />

# Step 6: Submitting a Pull Request

At this point, your local and remote repositories contain the changes you've made. If you want to share these changes with the original repository owner, Joyent, you can submit a pull request.

A pull request effectively says, "Hello, maintainer of Project X. I made some changes here in my forked copy, and I think they're good ones. You should add them to your repository".

Pull requests are a GitHub featre, so you'll need to head back to the browser to submit them.

<img width="782" alt="image" src="https://github.com/user-attachments/assets/4f690fda-1a8c-481d-aec2-1610a6a3206f" />

# Go Try It!

Perform the workflow:
    - Fork
    - Clone
    - Edit (It's OK if you feel like you can't make any substantial edits. The purpose of this exercise is to get a feel for the workflow, not majorly edit a project.)
    - Commit
    - Push
    - Submit a pull request
  
