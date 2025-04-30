

![image](https://github.com/user-attachments/assets/a9888803-10ed-4566-8db0-0726a26e5a9d)
![image](https://github.com/user-attachments/assets/02955a0c-4264-450b-b7cb-44cdb28c8768)
- git merge — combine branches
- git rebase — move commits
- git stash — temporarily save changes

# 🔀 1. Git Merge – Combine Another Branch into Main
## Create a new branch
  - git checkout -b feature-branch

## Make a change
   - echo "echo Feature added to script1" >> script1.sh

## Add and commit
   - git add script1.sh
   - git commit -m "Feature: Added line in script1"

## Go back to main
   - git checkout main

## Merge the feature branch
  - git merge feature-branch

# 🔁 2. Git Rebase – Replay Changes on Top of Another Branch
## Create another branch
  - git checkout -b rebase-branch

## Make a change in script2
  - echo "echo Rebase line added" >> script2.sh

## Add and commit
  - git add script2.sh
  - git commit -m "Rebase: Added line to script2"

## Rebase to main
  - git checkout main
  - git rebase rebase-branch

# 3. Git Stash – Temporarily Save Uncommitted Work
## Modify script3 without committing
  - echo "echo Temporary change" >> script3.sh

## Stash it
  - git stash

## Do other work or just check status
  - git status

## Bring back the stashed work
  - git stash apply
![image](https://github.com/user-attachments/assets/e66e0750-a654-40ba-bf48-84e70215e9a6)
![image](https://github.com/user-attachments/assets/d89beecc-8620-4711-9623-0aad455eb76d)

## 🚀 Finally, Push Everything to GitHub
- git add .
- git commit -m "Completed: Merge, Rebase, and Stash operations"
- git push origin main
![image](https://github.com/user-attachments/assets/f8955712-615f-4817-9163-e3eafc8e3494)

