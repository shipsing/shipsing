# shipsing

What is the use of git push origin main?
git push origin will push the current branch to the branch of the matching name in the remote repository (aka, “branch configured upstream”), if it exists, otherwise, it will not push and notify that the current branch has no remote counterpart (error message: “<branchname> has no upstream branch”).


In Git, "origin" is a shorthand name for the remote repository that a project was originally cloned from. More precisely, it is used instead of that original repository's URL - and thereby makes referencing much easier. Note that origin is by no means a "magical" name, but just a standard convention.

If you already have a local branch and want to set it to a remote branch you just pulled down, or want to change the upstream branch you're tracking, you can use the -u or --set-upstream-to option to git branch to explicitly set it at any time.

git push origin HEAD:master: This will push your local main branch to the existing remote master branch.
git push origin HEAD: This will push your local main branch to the branch of the same name on the remote, in other words, this will create a new branch on the remote called main. This is what we want!
