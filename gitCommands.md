git init (initialize repo)

git status (check if there are new or modified files in your workspace)

git add <some file> (add to staging area)

git commit -m "some message" (commit your changes before you push them to the remote repo)

git push origin master (upload your local changes to the remote repo [from master branch])

git pull origin master (get the latest changes from remote repo)

git pull --rebase [[[[[[CAN SOMEONE PLEASE EXPLAIN THE BENEFITS OF THIS COMMAND TO A NORMAL PULL OR MERGE???]]]]

git log (see commit history)

git checkout -b someName (create a new branch and directly switch to it)

git branch -d someName (delete a branch)

git merge someBranch (merge a branch into the branch you are currently in)

git reset --hard HEAD~1 (discard your last commit)
git reset --hard HEAD~2 (discard your 2 last commits)
