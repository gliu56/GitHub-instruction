# GitHub-instruction
record Git command

refer http://docs.duckietown.org/DT18/opmanual_duckiebot/out/preliminaries_git.html

Clone a repository:
$ git clone git@github.com:USERNAME/REPOSITORY.git

Create a new branch:
git checkout -b branch-name
To see which branch you are working on you can either use both of these commands
$ git branch
$ git status

Commit and Push changes:
After you edited some files, you want to push your changes from the local to the remote location. In order to do so, first do a double-check on which files you have changed and if things look legitimate. Invoke
$ git status

and check the output. There will be several files, that show up in red. These are files you have changed, but not yet added for a future commit. Most of the time you want to push all your changes so you add them to your commit by executing
$ git add --all

If you do not want to add all files, single files can be added. Then you need to specify each single file
$ git add file-path

After you solved this, add a commit message to let collaborators know, what you have changed:
$ git commit -m "commit-message"

If everything went smooth without any issues you are ready to push your changes to your branch:
$ git push origin branch-name

Fetch new branches:
If new branches have been pushed recently to the repository and you don’t have them you can invoke a

$ git fetch --all
to see all new branches and checkout to those.

Open a pull request:
If you are working on another branch than the master or if you forked a repository and want to propose changes you made into the master, you can open a so-called pull-request. In order to do so, press the corresponding tab in the dashboard of a repository and then press the green button New pull request. You will be asked which branch from which fork you want to merge.

