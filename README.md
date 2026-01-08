## Undoing Wrong Commits in Git 

# What happened?

I intentionally made a wrong commit named:

"wrong commit added by mistake" :  What I did to fix it

# Revert
I used:  git revert <commit-id>


This command created a new commit that safely undid the changes from the wrong commit.

1 git revert — SAFE (for already pushed commits)

2 Use when the commit is already pushed to GitHub

3 Does NOT delete history

4 Creates a new commit reversing the mistake


# Example

git log          
git revert <"commit id"> 
git push origin main



# soft reset
--soft reset (keeps changes in staging)
git reset --soft HEAD~1
Meaning:
Commit removed
Changes still staged

# --hard reset (deletes everything)
git reset --hard HEAD~1


