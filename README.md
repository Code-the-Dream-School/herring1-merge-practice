# herring1-merge-practice

This repository is temporary, to be used to practice merge conflict resolution.  When submitting to
a shared project, the basic steps are as follows:
1. Clone the project.  Check out the default branch.  In our case that's dev.  From that branch, create a branch for your changes, say feature27
2. Within that branch, create and test your changes.
3. Check out the default branch.
4. Do a `git pull origin dev`.
5. Check out the feature branch, in this case feature27.
6. Do a git merge dev.
7. If all is well, push your branch and create the PR.
8. If several team members have been making changes to the same file, you may get merge conflicts.  If git tells you that you have one or several merge conflicts, open each file with a conflict, and resolve the conflict.  Be sure you find all of them.  VSCode will flag each of them.  Sometimes you will take your change and discard the conflicting change, sometimes you will do the converse, sometimes you will accept both changes, and sometimes you'll have to combine them with manual editing.
9. Test your revised branch.
10. If the tests pass, add and commit your changes.
11. If this takes a while, other team members may have made more changes. You may need to check out the dev branch again, pull it again, and merge it again, resolving merge conflicts as needed.
12. Once all of that is complete, push your branch and submit the PR.
13. The PR may identify still more merge conflicts.  If so, repeat step 11 and push your branch again.
14. Time for a new feature branch!

We will experiment with concurrent changes so that you can practice these steps.  During the practice session, each student will make 3 changes to this README.md, all at the same time.  In a feature branch, make 3 changes to this README.md.  Each change should be 2-3 lines.  **First change here.**  Everyone is going to change the same lines.  Once you have made your changes, add and commit your changes and push your feature branch.  Then open a PR.

This is another paragraph where you make a change: **Second change here.** The actual words you write don't matter.

This is another paragraph where you make a change. In this case, just delete a randomly chosen word from the paragraph.

We'll merge changes as the PRs arrive, if there aren't merge conflicts.  When a merge conflict occurs your PR, follow the steps above to resolve it.  If you didn't get a merge conflict in your PR, create another feature branch and repeat the steps until you have practiced resolving merge conflicts.  Please note: Even if there is no merge conflict identified for your PR when you create it, a merge of somebody else's PR may create one you'll have to fix before it can be merged.
