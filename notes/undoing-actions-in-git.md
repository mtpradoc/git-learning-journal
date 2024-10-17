# Git History and Undoing Changes

## 1. git log --oneline

The git log command is useful for viewing the history of commits. The --oneline option condenses the output to one line per commit, showing a shortened commit hash and the commit message.

Command:
```bash
$ git log --oneline
```
Example Output:
```bash
a1b2c3d Update README
e4f5g6h Add new feature to homepage
i7j8k9l Initial commit
```
Explanation:
The commit hash (like a1b2c3d) is a short unique identifier for each commit.
The commit message provides a brief description of the change.
This command is particularly useful for getting a quick overview of your repository's history.

## 2. Undoing git add (Unstaging Changes)

If you staged changes using git add but realized you need to unstage them, you can undo the staging without affecting the changes themselves.

Command to Unstage a File:
```bash
$ git restore --staged <filename>
```
Example:
```bash
$ git restore --staged example.txt
```
Explanation:
This command moves the file from the staged area back to the working directory, meaning it's no longer staged for commit but your changes remain in the file.

## 3. Undoing git commit (Amend or Reset)

Sometimes you may want to undo or modify a commit. Here are a few ways to handle this:

### 3.1. Amending the Last Commit
If you need to change the last commit (e.g., update the commit message or add more changes), use the --amend option.

Command:
```bash
$ git commit --amend
```
Explanation:
This command allows you to modify the last commit. You can update the message or include additional staged changes.
Be cautious when using this after pushing to a remote, as it changes commit history.

### 3.2. Undoing the Last Commit but Keeping Changes
If you want to undo the last commit but keep your changes staged, use:

Command:
```bash
$ git reset --soft HEAD^
```
Explanation:
This command moves the last commit's changes back to the staging area. The commit is undone, but the changes remain ready to be committed again.

### 3.3. Undoing the Last Commit and Unstaging Changes
If you want to undo the last commit and also unstage the changes:

Command:
```bash
$ git reset HEAD^
```
Explanation:
This resets the last commit and moves the changes back to the working directory, meaning they are no longer staged.

## 4. git checkout for Reverting Changes

You can use git checkout to revert a file to a previous commit or discard changes in the working directory.

Command to Revert a File to a Previous Version:
```bash
$ git checkout <commit-hash> -- <filename>
```
Example:
```bash
$ git checkout a1b2c3d -- example.txt
```
Explanation:
This command restores example.txt to the state it was in at the specified commit (a1b2c3d).
It will overwrite local changes, so use it carefully.

## 5. git tag (Optional: Combine with git checkout)

Tags in Git are used to mark specific points in your commit history, such as version releases. You can use tags in combination with git checkout to switch to specific versions.

### 5.1. Creating a Tag:
Command:
```bash
$ git tag v1.0.0
```
### 5.2. Pushing Tags to Remote:
```bash
$ git push origin --tags
```
### 5.3. Checking Out a Tag:
Command:
```bash
$ git checkout v1.0.0
```
Explanation:
Tags are often used for marking releases or specific milestones in a project.
Using git checkout with a tag allows you to switch to a specific version of your project.