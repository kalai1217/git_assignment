
# GIT ASSIGNMENT
_This repo contains Git Assignments_
# Question 1

### Step 1: Create a new Git repository.

Create a new Git repository either locally or on a Git hosting service like GitHub.

### Step 2: Create a file and commit changes.

Create a file within your Git repository directory. Add content to the file and save it. Then, stage the changes and commit them using Git.

### Step 3: View the commit history of your repository.

To view the commit history of your repository, use the command `git log`.

### Step 4: Open the file you created earlier and make some changes to it.

Open the file in a text editor, make some changes, and save the file.

### Step 5: Check the file you modified is now marked as "modified" and unstaged.

To check the status of your files, including the modified file, use the command `git status`. This will show you which files have been modified and are unstaged.

### Step 6: Stage the changes you made to the file and commit the changes to the repository.

Stage the changes to the modified file using the command `git add <file_name>`. Then, commit the changes with a descriptive message using the command `git commit -m "Your commit message"`.

### Step 7: Clone the repository you have created on GitHub.

On GitHub, navigate to your repository's page and copy the clone URL. Then, in your terminal, use the command `git clone <repository_url>` to clone the repository to your local machine.

### Step 8: Fetch the changes.

Navigate into the cloned repository directory using the command line. Then, use the command `git fetch` to fetch any changes that have been made to the original repository since you cloned it.

### Step 9: Pull changes.

To merge the changes you fetched into your local copy of the repository, use the command `git pull`. This will update your local repository with the latest changes from the remote repository on GitHub.

## Question 2
### Step 1: Clone the repository you have created on GitHub.

On GitHub, navigate to your repository's page and copy the clone URL. Then, in your terminal, use the command `git clone <repository_url>` to clone the repository to your local machine.

### Step 2: Create a new branch using the command.

Create a new branch locally using the command `git branch <branch_name>`.

### Step 3: Switch to the new branch.

Switch to the newly created branch using the command `git checkout <branch_name>`.

### Step 4: Make some changes to the code in your local copy of the repository.

Open the necessary files in your preferred text editor, make changes, and save the files.

### Step 5: Commit changes to the new branch.

Stage the changes using the command `git add <file_name>` and then commit them with a descriptive message using the command `git commit -m "Your commit message"`.

### Step 6: Switch back to the original branch.

Switch back to the original branch using the command `git checkout <original_branch_name>`.

### Step 7: Merge the new branch.

Merge the changes from the new branch into the original branch using the command `git merge <new_branch_name>`.

### Step 8: Push changes to the original branch.

Push the changes made in the original branch to the remote repository on GitHub using the command `git push origin <original_branch_name>`.


## Question 3
## Step 1: Create a feature branch.

Create a new feature branch locally using the command `git checkout -b <feature_branch_name>`.

## Step 2: Switch to the new branch.

Switch to the newly created feature branch using the command `git checkout <feature_branch_name>`.

## Step 3: Open the file and make some changes to it.

Open the file in a text editor, make the necessary changes, and save the file.

## Step 4: Add and commit the changes to the new branch.

Stage the changes using the command `git add <file_name>` and then commit them with a descriptive message using the command `git commit -m "Your commit message"`.

## Step 5: Push the changes to the new feature branch.

Push the changes made in the feature branch to the remote repository on GitHub using the command `git push origin <feature_branch_name>`.

## Step 6: Create a pull request.

Create a pull request on GitHub by navigating to the repository's page and clicking on the "New pull request" button.

## Step 7: As another user in the master branch make some changes to the same file.

As another user, checkout the master branch locally using the command `git checkout master`. Then, open the file, make changes, and save it.

## Step 8: Add and commit the changes to the master branch.

Stage the changes using the command `git add <file_name>` and then commit them with a descriptive message using the command `git commit -m "Your commit message"`.

## Step 9: Push the changes to the master branch.

Push the changes made in the master branch to the remote repository on GitHub using the command `git push origin master`.

## Step 10: Resolve the conflict.

After the pull request is created, if there's a conflict, you need to resolve it. To resolve conflicts, use the command `git rebase master <feature_branch_name>` while you are on the feature branch. This will apply your changes on top of the changes from the master branch, allowing you to resolve any conflicts that arise.

Once conflicts are resolved, stage the changes (`git add <conflicted_file_name>`) and continue the rebase process (`git rebase --continue`). Repeat this process until all conflicts are resolved.

## Step 11: Push the resolved changes.

After resolving conflicts, push the changes to the feature branch using `git push origin <feature_branch_name>`.

## Question 4
## Step 1: Create a feature branch.

Create a new feature branch locally using the command `git checkout -b <feature_branch_name>`.

## Step 2: Switch to the new branch.

Switch to the newly created feature branch using the command `git checkout <feature_branch_name>`.

- Open the file and make some changes to it.
- Add and commit the changes to the new branch.
- Open the same file and make some changes to it.
- Add and commit the changes to the new branch.
- Open the same file and make some changes to it.
- Add and commit the changes to the new branch.

## Step 3: Identify the commit or commits that you want to "cherry-pick"

Note the hash of the commit or commits that you want to "cherry-pick".

## Step 4: Use the "git checkout" command to switch to the branch where you want to apply the changes.

Switch to the branch where you want to apply the changes using the command `git checkout <branch_name>`.

## Step 5: Use the "git cherry-pick" command followed by the commit hash(es) that you want to apply.

Apply the changes from the specified commit(s) to the current branch using the command `git cherry-pick <commit_hash>`.
## Question 5
## Step 1: Create a feature branch.

Create a new feature branch locally using the command `git checkout -b <feature_branch_name>`.

## Step 2: Switch to the new branch.

Switch to the newly created feature branch using the command `git checkout <feature_branch_name>`.

- Open the file and make some changes to it.
- Add and commit the changes to the new branch.
- Open the same file and make some changes to it.
- Add and commit the changes to the new branch.
- Open the same file and make some changes to it.
- Add and commit the changes to the new branch.

## Step 3: Use the "git log" command to view the commit history and identify the commit to which you want to reset.

View the commit history using `git log` and note the commit hash to which you want to reset.

## Step 4: Use the "git reset" command followed by the desired reset type and the commit hash.

Perform a reset using `git reset --<reset_type> <commit_hash>`.

## Step 5: Verify that the reset was successful by using the "git log" command again.

Check the commit history with `git log` to ensure that the reset was successful.

## Step 6: Use the "git log" command to view the commit history and identify the commit that you want to reverse.

View the commit history using `git log` and note the commit hash that you want to revert.

## Step 7: Use the "git revert" command followed by the commit hash or reference to which you want to revert.

Revert a commit using `git revert <commit_hash>`.

## Step 8: Verify that the revert was successful by using the "git log" command again.

Check the commit history with `git log` to verify that the revert was successful.

