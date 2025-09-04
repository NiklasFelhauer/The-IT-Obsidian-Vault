
## Update
1. Update a Branch from Main:
   ```shell
   git rebase origin/main
   ```

   ```shell
   git pull origin main
   ```
## Create
1. Create and switch to the new branch in one step:
   ```shell
	git checkout -b my-new-branch
   ```
2. Push the new branch to remote (e.g., GitHub, GitLab):
   ```shell
   git push -u origin my-new-branch
   ```
   
## Switch
2. Switch to an existing branch:
   ```shell
   git checkout <branchName>
   ```
3. Switch branches (modern syntax):
   ```shell
   git switch <branchName>
   ```
## Delete
2. Delete a branch locally:
   ```shell
   git branch -d <branchName>
   ```

3. Remove Merged Local Branches
   ```shell
 git branch --merged main | ForEach-Object {
    if ($_ -ne "* main" -and $_ -ne "main") {
        git branch -d $_.Trim()
    }
}

   ```

4. Prune deleted branches:
   ```shell
   git fetch --prune
   ```
## Get
4. Fetch all new branches:
   ```shell
   git fetch --all
   ```

6. View all branches (local and remote):
   ```shell
   git branch -a
   ```

7. Pull the latest changes from a branch:
   ```shell
   git pull <branchName>
   ```

## Add
12. Add a specific file to the staging area:
   ```shell
   git add <fileName>
   ```

13. Add all changes in the current directory to staging:
   ```shell
   git add .
   ```

## Commit
14. Commit with a message:
   ```shell
   git commit -m "Your commit message"
   ```
## Push
16. Push changes to the remote repository:
   ```shell
   git push origin <branchName>
   ```

## Merge
18. Merge another branch into the current branch:
   ```shell
   git merge <branchName>
   ```

## Rebase
19. Rebase the current branch onto another branch:
   ```shell
   git rebase <branchName>
   ```

20. Abort a rebase:
   ```shell
   git rebase --abort
   ```

## Status
21. View the current status of the working directory:
   ```shell
   git status
   ```

## Log
22. View commit history:
   ```shell
   git log
   ```

23. View a one-line summary of the commit history:
   ```shell
   git log --oneline
   ```

## Stash
24. Save changes to the stash:
   ```shell
   git stash
   ```

25. Apply the most recent stash:
   ```shell
   git stash apply
   ```

26. List all stashes:
   ```shell
   git stash list
   ```

## Remote
27. Add a new remote repository:
   ```shell
   git remote add origin <repositoryURL>
   ```

28. View remote repositories:
   ```shell
   git remote -v
   ```

29. Remove a remote repository:
   ```shell
   git remote remove <name>
   ```

## Tag
30. Create a new tag:
   ```shell
   git tag <tagName>
   ```

31. Push a tag to the remote repository:
   ```shell
   git push origin <tagName>
   ```

32. Delete a tag locally:
   ```shell
   git tag -d <tagName>
   ```

33. Delete a tag remotely:
   ```shell
   git push origin --delete <tagName>
   ```

## Reset
34. Reset the staging area but keep changes:
   ```shell
   git reset <fileName>
   ```

35. Reset the working directory to the last commit:
   ```shell
   git reset --hard
   ```

36. Undo the last commit but keep changes:
   ```shell
   git reset --soft HEAD~1
   ```

## Miscellaneous
37. View the Git configuration:
   ```shell
   git config --list
   ```

38. Set a global username:
   ```shell
   git config --global user.name "Your Name"
   ```

39. Set a global email:
   ```shell
   git config --global user.email "youremail@example.com"
   ```
