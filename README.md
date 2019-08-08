# Workshopgit2

Foobar is a Python library for dealing with word pluralization.

## Commands:

```bash
diff, gitk, reflog, reset
```

## Steps:

```python

01. Clone this repo: git clone https://github.com/eduardobohorquez/workshopgit2.git
02. cd workshopgit2
03. Create a new branch: git checkout -b new_branch
04. Create a new file: echo "any message" >> my_file.txt
05. Add your changes: git add *
06. Commit your changes: git commit -m "my message"
07. Verify your changes: git status
08. Upload your changes: git push origin new_branch
09. Verify the differences between master and new_branch: git diff master new_branch
10. Use the git GUI to see the history: gitk
11. Create a new branch from the branch created: git checkout -b new_branch2
12. Verify the files in branch: ls
13. Delete the file previously created: rm my_file.txt
14. Add your changes: git add my_file.txt
15. Verify your changes: git status
16. Commit your changes: git commit -m "delete the file"
17. Upload your changes: git push origin new_branch2
```

## Recovering the File:

```python

18. List the commits to recover the file: git reflog
19. Identify the commit id before the file was deleted
20. Make a "reset" to that commit id: git reset --hard {COMMIT_ID}
21. Update the references: git update-ref refs/heads/new_branch2 origin/new_branch2
22. Add the file: git add my_file.txt
23. Commit your changes: git commit -m "my recovery file message"
24. Upload your changes: git push origin new_branch2

```
