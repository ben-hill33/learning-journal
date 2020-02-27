# Reading Assignment notes

Git is a distributed version control system (DVCS)  for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files.
What git does is it stores data in a file system made up of snapshots. Each time you save a changed version of your project - called a commit - Git creates a snapsho tof the file and stores a reference to it. If the file has not changed, git only sotres a reference to the already sotred identical version of it.
Git mostly relies on local operations because necessary info can be found in local resources. This allows process expediency because a projects history resides on the local disk, not having to get info from a server, and allows me to work on a prject offline.
Git tracks changes like file corruption or loss of info in transit
Git minimizes the possibility of damage to files

Files in git can reside in 3 main states: 
- Commited Data is securely stored in a local database
- Modified File has been changed but not committed to the database
- Staged Flagged a file’s changed version to be committed in the next snapshot

To check settings use the "git config --list" command

Command $ git help; will give you a list of commands
Also git command --help
And, man git-command
	

Local Repository Structure
The local Git repository has three components:
1. Working Directory: The actual files reside here.
1. Index: The area used for staging 
1. Head: Points to the most recent commit


Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.
Tracked
Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
Untracked
Untracked files were not in the last snapshot and do not currently reside in the staging area.
Commit Mistakes
You can use the –amend command when you need to alter a commit message or forgot to add some files.

``` $ git commit --amend```

In the example above, you can use this command to easily change your commit message, if no changes were made since the newest commit.

$ git commit -m “my first commit"

$ git add example_file

$ git commit --amend
