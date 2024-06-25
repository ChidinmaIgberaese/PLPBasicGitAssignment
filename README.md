# PLPBasicGitAssignment

This repository documents the basic workflow of creating a GitHub repository, connecting it to a local folder, and handling common Git operations.

## Steps and Commands Used

### 1. Create GitHub Repository

- Created a new repository named `PLPBasicGitAssignment` on GitHub. I checked the README.md box to help create the README.md file.

### 2. Initialize Local Repository

- Opened Git Bash and navigated to the desktop directory.

  On Gitbash, i did the following commnds;
  cd desktop
  mkdir PLPBasicGitAssignment
  cd PLPBasicGitAssignment
  git init

### 3. Set the default branch name to main for all new repositories globally:

I changed my branch globally from "master" to "main" to avoid confusion. This made my hello.txt file repository to show on github main branch automatically without having to switch default settings in order to see my text file as instructed in step7 of the assignment.
git config --global init.defaultBranch main

### 4. Create and Commit Files

Opened VSCode and created a file named hello.txt with this command:
code .

### 5. Staged and committed the file to the local repository:

git add hello.txt
git commit -m "Add hello.txt with a greeting"

### 6. Connect to Remote Repository

Added the remote repository URL and pushed changes to the main branch:
git remote add origin https://github.com/ChidinmaIgberaese/PLPBasicGitAssignment.git
git push -u origin main

### 7. Handling Remote Repository Conflicts (Rebasing)

Fetched remote changes:
git fetch origin

Rebased local commits on top of remote changes:
git rebase origin/main

### 8. Pushed the rebased changes to the remote main branch:

git push -u origin main

### 9. Adding and Editing Documentation:

Made changes to the README.md file directly in VSCode.Stage, Commit, and Push the Changes:
git add README.md
git commit -m "Update README.md with additional documentation"
git push origin main
