# Steps followed before adding any code
Created a branch by the name of git_assignment_HeroVired in github
Used the code tab in the repository to fetch the SSH url of the repository
Logged in to VS Code and used the git clone command to clone the repository in vs code 
git clone git@github.com:Gaurav-Idnani/git_assignment_HeroVired.git
The folder used in Local Machine was D:/Assignments

# Steps Followed for first phase in dev branch
Created a new file in vs code
Added the code as provided in the assignment
Corrected the code for indentation
Saved and committed the code in dev branch
Used the git add . command to stage changes
used the git commit -m "Version 1" to commit changes to dev branch
used the git push to push the code to dev remote and updated the Readme till here.
git push --set-upstream origin dev

# Steps followed for second phase in feature/sqrt branch
Ceated the feature branch using the command git checkout -b feature/sqrt
Uncommented the feature code in python file.
Committed the change to branch
Now saving the comments here and committing it to branch before switching back to dev.

# Steps followed after switching back from feature/sqrt branch to dev
# Note : One step was missed earlier, which involved merging the changes in dev to main. That step is being taken care before starting phase 3.(bugfix in dev)

# Note : The changes from feature/sqrt have not been yet fetched in the dev branch
First step was to close the pull request raised from dev to main to account for merge completion missed(as mentioned below)

Then, the divide method was updated in the python file, followed by the commit.
Lastly, since we need to keep the feature/sqrt branch up to date, these changes need to be merged there as well.


