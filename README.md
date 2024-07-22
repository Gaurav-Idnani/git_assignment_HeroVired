# Git LFS (Large File Storage)

In order to enable the lfs system for git we use the command when we have checked out to this branch.
git lfs install

Secondly we have to specify which type of files, git would track as part of LFS enablement.
In this example we have used a .MP4 video file. Use this command
git lfs track "*.mp4"

As per the documentation provided on Git LFS we used this one more command as part of SOP
git add .gitattributes
The .gitattributes file looks somewhat like the .gitignore file to store the configurational parameters for files which we need to track.

Lastly, we follow the normal procedure to commit this file to the git repository like we would for any other file.
git add .
git commit -m "Added a large video file"
git push --set-upstream origin lfs


