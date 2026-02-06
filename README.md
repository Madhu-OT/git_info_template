# git_info_template
Git commands listed for different project development processes

Git Workflow for Built Application Updates
1. Initial Setup (First Time)
bash
# Clone remote repository
git clone <remote-repo-url>
cd uirecipemanagement
 
# Create and switch to feature branch
git checkout -b feature/trail-test

2. Development Cycle
bash
# Make code changes...
# Stage changes for commit
git add .
 
# Commit changes locally
git commit -m "feat: Add Trail-Test functionality"
 
# Continue development as needed
git add .
git commit -m "fix: Resolve routing issues"

3. Sync with Remote
bash
# Fetch latest changes from remote
git fetch origin
 
# Rebase your branch on top of main/master
git rebase origin/main
 
# Resolve any conflicts if they exist
# (edit files, then git add ., git rebase --continue)

4. Push Changes
bash
# Push feature branch to remote
git push origin feature/trail-test
 
# Create Pull Request/Merge Request through Git UI
# Or merge directly if you have permissions

5. Update Main Branch
bash
# Switch to main branch
git checkout main
 
# Pull latest changes
git pull origin main
 
# Merge feature branch
git merge feature/trail-test
 
# Push updated main to remote
git push origin main

6. Cleanup
bash
# Delete local feature branch
git branch -d feature/trail-test
 
# Delete remote feature branch (optional)
git push origin --delete feature/trail-test
Alternative Workflow (Simplified)
bash
# For quick updates to existing branch
git checkout testing
git add .
git commit -m "Update Trail-Test component"
git push origin testing
Key Commands Summary
•	git clone - Get repository
•	git checkout -b - Create feature branch
•	git add + git commit - Save changes locally
•	git fetch + git rebase - Sync with remote
•	git push - Send changes to remote
•	git pull + git merge - Update main branch

