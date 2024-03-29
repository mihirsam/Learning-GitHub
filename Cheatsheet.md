﻿# CheatSheet
This cheat sheet summarizes commonly used Git command line instructions for quick reference.


**Install**

GitHub for Windows https://windows.github.com 
GitHub for Mac https://mac.github.com 
Git for All Platforms http://git-scm.com 
Git distributions for Linux and POSIX systems are available on the official Git SCM web site.

**Create repositories**

 - $ git init
	 - Turn an existing directory into a git repository
 - $ git clone [url]
	 - Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits
	
**Branches**
 - $ git branch [branch-name]
	 - Creates a new branch
 -  $ git checkout [branch-name]
	 - Switches to the specified branch and updates the working directory

 - $ git merge [branch]

	 - Combines the specified branch’s history into the current branch. This is usually done in pull requests, but is an important Git operation.

 - $ git branch -d [branch-name]
	 - Deletes the specified branch

**Synchronize changes**

 - $ git fetch

	 - Downloads all history from the remote tracking branches

 - $ git merge

	 - Combines remote tracking branch into current local branch

 - $ git push

	 - Uploads all local branch commits to GitHub

 - $ git pull

	 - Updates your current local working branch with all new commits from
	   the corresponding remote branch on GitHub. git pull is a combination
	   of git fetch and git merge

**Make changes**

 - $ git log

	 - Lists version history for the current branch
 - $ git diff [first-branch]...[second-branch]

	 - Shows content differences between two branches

 - $ git add [file]

	 - Snapshots the file in preparation for versioning

 - $ git commit -m "[descriptive message]"

	 - Records file snapshots permanently in version history

**Redo commits**

 - $ git reset [commit]

	 - Undoes all commits after [commit], preserving changes locally

 - $ git reset --hard [commit]

	 - Discards all history and changes back to the specified commit


**Rewriting branches, updating commits and clearing history**

 - $ git rebase <branch>

	 - apply any commits of current branch ahead of specified one

 - $ git reset --hard <commit>

	 - clear staging area, rewrite working tree from specified commit
	

**Glossary**

 - git: an open source, distributed version-control system
 - GitHub: a platform for hosting and collaborating on Git repositories
 - commit: a Git object, a snapshot of your entire repository compressed
   into a SHA
 - branch: a lightweight movable pointer to a commit
 - clone: a local version of a repository, including all commits and
   branches
 - remote: a common repository on GitHub that all team member use to
   exchange their changes
 - fork: a copy of a repository on GitHub owned by a different user
 - pull request: a place to compare and discuss the differences
   introduced on a branch with reviews, comments, integrated tests, and
   more
 - HEAD: representing your current working directory, the HEAD pointer
   can be moved to different branches, tags, or commits when using git
   checkout

