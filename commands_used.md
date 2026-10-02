# Project 7-7 – Zsh Configuration & GitHub Integration  
### Full Command History (English Version)

This document contains every command used during the completion of Project 7‑7, including Zsh configuration, file management, Git initialization, GitHub token creation steps, and final repository upload.

---

## 1. Project Directory Setup

```bash
mkdir Project7-7_Zsh
cd Project7-7_Zsh

2. Zsh Configuration Files
Create .zshrc if missing:

bash
touch ~/.zshrc
Copy .zshrc into the project folder:

bash
cp ~/.zshrc ~/Project7-7_Zsh/
List files:

bash
ls -l
ls -a ~
3. Zsh Shell Usage
Start Zsh:

bash
zsh
Reload configuration:

bash
source ~/.zshrc
Test autocorrect:

bash
grp NFS /etc/services
Test autocd:

bash
pwd
Desktop
pwd
4. Redirection Exercises
Multiple redirections:

bash
grep NFS /etc/services >file1 >file2
Pipe + redirection:

bash
grep NFS /etc/services >file1 | grep protocol >file2
Sort with multiple inputs:

bash
sort <file1 <file2 >file3
View results:

bash
cat file1
cat file2
cat file3
5. Git Initialization
Initialize Git inside the project folder:

bash
git init
Check status:

bash
git status
Configure Git identity:

bash
git config --global user.name "Jorge"
git config --global user.email "YOUR_GITHUB_EMAIL"
Add and commit files:

bash
git add .
git commit -m "Project 7-7: Zsh configuration and exercises"
Rename branch to main:

bash
git branch -m main
6. GitHub Personal Access Token (PAT)
Steps (not terminal commands):
Log in to GitHub

Go to Settings

Open Developer settings

Select Personal access tokens → Tokens (classic)

Click Generate new token (classic)

Token name: Fedora-Git

Expiration: 90 days

Scopes: repo

Generate token and copy it (GitHub will not show it again)

7. Connect Local Repository to GitHub
Remove incorrect remote (if needed):

bash
git remote remove origin
Add correct remote:

bash
git remote add origin https://github.com/YOUR_USERNAME/linux-shell-projects.git
Verify remote:

bash
git remote -v
8. Push Project to GitHub
Push using your GitHub username and your Personal Access Token:

bash
git push -u origin main
Git will prompt:

Username:  
Your GitHub username

Password:  
Your Personal Access Token (PAT)

9. Successful Push Output (Expected)
Code
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), done.
To https://github.com/YOUR_USERNAME/linux-shell-projects.git
 * [new branch] main -> main
branch 'main' set up to track 'origin/main'.
End of Document
Code

---

# 🚀 Jorge, this file is ready to upload  
You can now:

1. Create a file inside your repo:
nano commands_used.md

Code
2. Paste the entire content above  
3. Save with:
- **Ctrl + O**
- **Enter**
- **Ctrl + X**
4. Commit and push:
git add commands_used.md
git commit -m "Added full command history documentation"
git push
