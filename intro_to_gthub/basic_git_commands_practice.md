# Learning Objectives

By the end of this lesson, you' be able to:

- Practice using basic Git commands.

# Git Review

To save the changes that we've made to our work to the GitHub platform, we must:

- Stage all of the files using *git add . *
- Commit our changes using *git commit - m "message"*
- Push the committed changes up to GitHub using *git push*

When you work with GitHub, you may be asked to "add, commit, push" your files. What this means is that you must run these three commands in succession to upload your code to the corresponding repo on GitHub.

# Knowlesde Check

When you have files that you want to stage using Git, which of the following commands must you run so that Git will track all of the files in the current directory?

Select the best answer.

[x] git add .
Correct: We use "git" to specify that we are running a Git command, "add" to stage files, and a period (".") to tell Git to stage all of the files in the repo.

[ ] git track --all
[ ] git stage --all_files
[ ] git commit -m "all files"

# Knowledge Check

Once you have stages files, in order to get them ready for upload, you must __ the changes:

Select the best answer.

[x] commit
Correct: Once files are staged, we must commit the changes before we are able to push the code up to GitHub.

[ ] add
[ ] push

# Forking

Most of your course materials are distributed using Git repos hosted on GitHub and they're shared with your classmates. But because they're shared, they can also be overwritten.

How can you push your changes directly to the original repo to prevent someone else from overwriting them?

You can tackle this with forks.

A fork is a private copy of a repo that is saved to your own account. That way, you can make changes to this copy without fear of losing your progress!

<img width="797" alt="image" src="https://github.com/user-attachments/assets/c93b64d6-eeec-40a1-a62a-d778b2b234f7" />

# Cloning

Cloning is the process of downloading a repo from a remote location (most often GitHub) to our machine.

We can clone repos from our own account or even public repos from other developers and data scientists.

You may hear the phrase "fork and clone", which is your cue to:

- Navigating to the appropriate repo on your cohort's GitHub organization.
- Fork the repo using the "Fork" button on the repo's page
- Run the *git clone* command in your terminal to download the repo to your machine.

<img width="806" alt="image" src="https://github.com/user-attachments/assets/9c7e0426-2eb4-4106-aa03-a05c9d7daa80" />

# Knowledge Check

How do you download a repo to your computer?

Select the best answer.

[x] Clone
Correct: To download a repo, we use the *git clone* command. While this will be commonly used with a forked repo, forking isn't necessary for the download process.

[ ] Fork
[ ] Add commit push

# Knowledge Check

When working with a repository, what must you do before you can clone the repo and make changes?

Select the best answer.

[x] Fork the original repo on GitHub so that you have a personal copy for editing.
Correct: The repo must be forked to your own account before you can safely make changes

[ ]  Clone the original repo and make your changes, then create a pull request.
[ ] Create a new repo in your account so that you can copy and paster the files.

