# SDV502 - Lab Three - Version Control System (Git)

## Git Commands:

1. cherry-pick:

    - Using cherry-pick, Git allows you to add individuals commits from any branch to your current head branch. This functions differently to merging/rebasing, as only the selected commit is integrated, rather than all commits from the a branch.

    - Command syntax -> git cherry-pick COMMIT-HASH

    - Commit Hash can be found via GitHub or via the Git command 'git log'.

    ![commit-hash-method-1](images/CommitHash1.png)

    ![commit-hash-method-2](images/CommitHash2.png)

2. unstaging:

    - 'git add' adds files to Git's staging index, from which they will be included in the next commit. 'git add .' can be used to stage all changes since the last commit. Specific files can also be staged using 'git add FILE-PATH'.

    - 'git reset' unstages all files currently in Git's staging index and resets your current head branch to the prior commit. 'git reset HEAD FILE-PATH' can also be used to unstage specific files. 'git reset MODE COMMIT-HASH' can also be used to reset to a given commit. Modes include:

        > '--soft' does not reset staging index or working tree but resets head to given commit.
        > '--mixed' resets the staging index but not the working tree.
        > '--hard' resets the staging index and the working tree.

3. unmodifying:



4. undoing:



5. rebasing:

    - 'git rebase' changes the base of your branch from one commit to another, making it seem as if your branch was created from a different commit by creating new commits and applying them to the new specified base.

    - i.e. 'git checkout FEATUR'E then 'git rebase master' moves the entire feature branch on top of the master branch.

    - Is a way to integrate changes from one branch to another, similar to 'git merge'. 'git rebase' compresses all changes and integrates them to the target branch.

6. stashing:



7. cleaning:



8. branching workflow:



