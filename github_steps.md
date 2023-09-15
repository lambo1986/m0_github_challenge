# GitHub Steps

Describe in your own words how to establish a connection between a local repository and a remote repository on GitHub.
---
- create a new repo in github, then push the git up to the cloud using:

git remote add origin git@github.com:USERNAME/REPO_NAME.git
git branch -M main
git push -u origin main

- if you need to sever the github connection and renew, follow these steps:

1. Check your current git remote origin connection using git remote -v
2. If you are connected to a remote origin that you do not have access to, remove your connection using git remote remove origin
3. Check that the git remote origin was removed using git remote -v. If you don’t get anything in response, you know you aren’t connected to a remote repository!
4. Then you can create a new empty repository on your GitHub and connect it to that remote repository. Use the command git remote add origin [insert SSH code here] to establish that connection.
5. Check your remote origin is correct now using git remote -v.
6. Now that you’re connected to the correct remote repository, you can run those two commands to establish the main branch and push your work: git branch -M main and git push -u origin main.