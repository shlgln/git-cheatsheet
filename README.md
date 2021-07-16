# git-cheatsheet
Title: Working with Git
1- Why do we use version control tools like Git?
We use it for source maintenance and project versioning
2- What is a repository? What important files does a good repository have?
It is a repository that holds all commits, releases, branches, tags, etc. Important files of a good repository are: LINCENCET , README.md and .gitignore
3- What are the parts of a good document?
It has three parts:
- Explanation about the type of project operation
- Explain how to work with the project
- How to help others in the process of project progress
4- What does the git clone command do?
Clones a repository into a newly created directory, and creates and checks out an initial branch that is forked from the cloned repository’s currently active branch.
5- What command should be executed if we want to update the local repository with the remote repository?
using git clone 
6- What is the difference between reset, revert, checkout?
git reset: It actually does a couple of different things depending on how it is invoked. The command modifies the index (the so-called “staging area”). It can also change which commit a branch head is currently pointing at. This command may alter existing history 
git revert: This command can be considered an ‘undo’ type command. However, it is not a traditional undo operation. Instead of removing the commit from the project history, it figures out how to invert the changes introduced by the commit and appends a new commit with the resulting inverse content. This prevents Git from losing history, which is important for the integrity of your revision history and for reliable collaboration.
git checkout: This command operates on three distinct entities: files, commits, and branches. In addition to the definition of “checkout,” the phrase “checking out” is commonly used to imply the act of executing the git checkout command. The git checkout command allows you to navigate between the branches that are created by git branch.
7- What is the difference between merge and rebase?
git Merge: it takes the contents of a source branch and combines them with a target branch Only the target branch is updated in this process. The history of the source branch remains similar.
git Rebase - Another way to integrate modifications from one branch to another is by Rebase. Rebase compresses all the modifications into a single patch. The patch is then inserted into the target branch.
8- What command is used to view the history of comets?
using git log
9- What command do we use if we want to see changes to a file?
using git diff
10-1- What is the use of tag?
Typically, people use this functionality to mark release points (v1.0, v2.0 and so on)
 10-2- How to create a tag?
using git tag <tag_name>	
11- What is the process for participating in a gate-managed project?
a- git clone <remote>
b- git checkout –b <new branch>
c- Make the desired changes
d- git commit –m “message”
e- git merge
f- git pull <remote>
g- git push
12-1- What are the branches used for? 
Branching means you diverge from the main line of development and continue to do work without messing with that main line
12-2- how can they be integrated?
git merge <branch name>
