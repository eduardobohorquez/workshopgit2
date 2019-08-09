# Workshopgit2

## Commands:

```bash
diff, gitk, reflog, update-ref, reset
```

## Steps:

```
1. Clone this repo: 

  git clone https://github.com/eduardobohorquez/workshopgit2.git
```
```
2. Go to Folder:

  cd workshopgit2
```
```
3. Create a new branch: 

  git checkout -b new_branch
```
```
4. Create a new file: 
  
  echo "any message" >> my_file.txt
```
```
5. Add your changes: 
  
  git add *
```
```
6. Commit your changes: 
  
  git commit -m "my message"
```
```
7. Verify your changes: 
  
  git status
```
```
8. Upload your changes: 
  
  git push origin new_branch
```
```
9. Verify the differences between master and new_branch: 
 
 git diff master new_branch
```
```
10. Use the git GUI to see the history: 
  
  gitk
```
```
11. Create a new branch from the branch created: 
  
  git checkout -b new_branch2
```
```
12. Verify the files in branch: 
  
  ls
```
```
13. Delete the file previously created: 
  
  rm my_file.txt
```
```
14. Add your changes: 

  git add .
```
```
15. Verify your changes: 

  git status
```
```
16. Commit your changes: 
 
  git commit -m "delete the file"
```  
```
17. Upload your changes: 
  
  git push origin new_branch2
```

## Recovering the File:

```
18. List the commits to recover the file: 
  
  git reflog
  
  And Identify the commit id before the file was deleted
```
```
19. Make a "reset" to that commit id: 

  git reset --hard COMMIT_ID
```
```
20. Update the references: 
  
  git update-ref refs/heads/new_branch2 origin/new_branch2
```
```
21. Add the file: 

  git add .
```
```
22. Commit your changes: 

  git commit -m "my recovery file message"
```
```
23. Upload your changes: 

  git push origin new_branch2
```
