# EXP6GIT
EXPERIMENT – 6

Cloning a GitHub Repository and Updating the Local Repository

Objective

To clone an existing GitHub repository, verify the remote connection, modify a file and commit the changes locally, then update the local repository with the latest changes available on the remote repository.

Git Workflow

GitHub Repository → Clone → Local Repository → Modify File → Commit Changes → Update Remote Repository → Pull Latest Changes

---

Git Commands

Step 1: Navigate to the parent folder

cd my-project

Note: "my-project" is the parent folder where you want to clone the repository. If you are already in the desired location, skip this command.

Step 2: Clone the existing GitHub repository

git clone <GitHub-repository-URL>

Example:

git clone https://github.com/USERNAME/experiments.git

Step 3: View the cloned repository folder

ls

Step 4: Navigate into the cloned repository

cd experiments

Step 5: Verify the remote connection

git remote -v

This displays the remote repository URL for fetch and push operations.

Step 6: View the files inside the repository

ls

You should see the existing files, such as:

- app.txt
- Other files present in the repository

Step 7: View the existing file contents

cat app.txt

Step 8: Modify the existing file

vi app.txt

Make the required changes.

To save and exit:

Esc
:wq

Step 9: Check the repository status

git status

Step 10: Stage the modified file

git add app.txt

Step 11: Commit the changes locally

git commit -m "Updated app file"

This saves the changes in the local Git repository.

Step 12: View the commit history

git log --oneline

---

Updating the Remote Repository

Step 13: Make changes on GitHub

1. Open the same repository on GitHub.
2. Open "app.txt".
3. Click the pencil (Edit) option.
4. Add some new content.
5. Click Commit changes to save the changes on GitHub.

Step 14: Pull the latest changes into the local repository

Return to Git Bash and execute:

git pull origin main

Note: Use "main" only if the remote branch is named main. If it is named master, use "git pull origin master".

This fetches and integrates the latest remote changes into your local branch.

Step 15: Verify the updated file

cat app.txt

Step 16: Check the repository status

git status

If everything is synchronized, you should see:

nothing to commit, working tree clean

---

Result

The existing GitHub repository was successfully cloned into the local system. The remote connection was verified, the file was modified and committed locally, and the latest changes from the remote repository were pulled into the local repository.
