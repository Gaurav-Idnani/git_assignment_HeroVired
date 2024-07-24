switched to main branch
(as in the end we have to finally merge changes to main)
git checkout main

# created a new branch geometry-calculator
git checkout -b geometry-calculator

# create new file areaCalculator.py and add the code provided

# proceed to commit the change and push to remote
git add.
git commit -m "Area calculator file added to branch"
git push --set-upstream origin geometry-calculator

# a. Create a New Branch:
git checkout -b feature/circle-area
- Create a new branch named "feature/circle-area" to work on the circle area feature
uncomment line 10,11 and save the file

# b. Stash Changes for Circle Area Feature:
git stash
Saved working directory and index state WIP on feature/circle-area: db39f70 Area calculator file added to branch

- Before committing the changes, stash them using git stash to save the incomplete feature implementation.
git status
On branch feature/circle-area
nothing to commit, working tree clean

# c. Create a New Branch for Rectangle Area Feature:
git checkout geometry-calculator.
git checkout -b feature/rectangle-area
- Create a new branch named "feature/rectangle-area" to work on the rectangle area
uncomment line 14,15,16 to add the rectangle area feature

Stash Changes for Rectangle Area Feature:

- Before committing the changes, stash them using git stash to save the incomplete feature implementation.
git stash
Saved working directory and index state WIP on feature/rectangle-area: db39f70 Area calculator file added to branch
- Verify that the working directory is clean
git status
On branch feature/rectangle-area
nothing to commit, working tree clean

# e. Switch Back to Circle Area Branch:
git checkout feature/circle-area
- Switch back to the "feature/circle-area" branch to continue working on the circle area feature.

- Retrieve the stashed changes
git stash apply 1
On branch feature/circle-area
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   areaCalculator.py

no changes added to commit (use "git add" and/or "git commit -a")
- Complete the circle area feature implementation and save the changes.

# f. Commit and Push Circle Area Feature:
git add areaCalculator.py
git commit -m "Completing circle area feature"
git push --set-upstream origin feature/circle-area

# g. Switch Back to Rectangle Area Branch:
git checkout feature/rectangle-area
- Switch back to the "feature/rectangle-area" branch to continue working on the rectangle area feature.

- Retrieve the stashed changes
git stash apply 0
- Complete the rectangle area feature implementation and save the changes. h. Commit and Push Rectangle Area Feature
git add areaCalculator.py
git commit -m "Completing the rectangle area feature"
git push --set-upstream origin feature/rectangle-area

# h. Commit and Push Rectangle Area Feature

# i. Create Pull Requests:
Since, both branches have been worked on independently they will have their seperate PRs
Additional step, though it is not mentioned we will add another layer of adding PRs to geometry-calculator branch
That would allow us to push both features together forward
- Create a pull request to the ‘dev’ branch.

- Have another team member or reviewer review your pull requests. 
- After receiving approval, merge both pull requests into the main branch.
Since both PRs have been merged to dev we will now create PR from dev to main effectively having both features in dev and main
