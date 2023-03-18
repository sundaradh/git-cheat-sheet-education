GIT CHEAT SHEET![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.001.png)![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.002.png)

Git is the free and open source distributed version control system that’s responsible for everything GitHub related that happens locally on your computer. This cheat sheet features the most important and commonly used Git commands for easy reference.

**INSTALLATION & GUIS STAGE & SNAPSHOT**

With platform speci c installers for Git, GitHub also provides the ease of staying up-to-date with the latest releases of the command line tool while providing a graphical user interface for day-to-day interaction, review, and repository synchronization.

**GitHub for Windows**

h ps://windows.github.com

**GitHub for Mac**

h ps://mac.github.com

For Linux and Solaris platforms, the latest release is available on the official Git web site.

**Git for All Platforms** h p://git-scm.com

**SETUP**

Con guring user information used across all local repositories

**git config --global user.name “[firstname lastname]” ![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.003.png)**set a name that is identi able for credit when review version history **git config --global user.email “[valid-email]”**

set an email address that will be associated with each history marker **git config --global color.ui auto**

set automatic command line coloring for Git for easy reviewing

**SETUP & INIT**

Con guring user information, initializing and cloning repositories

**git init**

initialize an existing directory as a Git repository

**git clone [url]** retrieve an entire repository from a hosted location via URL

Working with snapshots and the Git staging area

**git status![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.004.png)**

show modi ed  les in working directory, staged for your next commit **git add [file]**

add a  le as it looks now to your next commit (stage)

**git reset [file]**

unstage a  le while retaining the changes in working directory

**git diff**

diff of what is changed but not staged

**git diff --staged**

diff of what is staged but not yet commi ed

**git commit -m “[descriptive message]”**

commit your staged content as a new commit snapshot

**BRANCH & MERGE**

Isolating work in branches, changing context, and integrating changes

**git branch**

list your branches. a \* will appear next to the currently active branch **git branch [branch-name]**

create a new branch at the current commit

**git checkout**

switch to another branch and check it out into your working directory **git merge [branch] ![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.005.png)**

merge the speci ed branch s history into the current one **git log** 

show all commits in the current branch s history 

**INSPECT & COMPARE SHARE & UPDATE![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.006.png)**

Examining logs, diffs and object information



|**git log**|
| - |
|show the commit history for the currently active branch|
|**git log branchB..branchA**|
|show the commits on branchA that are not on branchB|
|**git log --follow [file]**|
|show the commits that changed  le, even across renames|
|**git diff branchB...branchA**|
|show the diff of what is in branchA that is not in branchB|
|**git show [SHA]**|
|show any object in Git in human-readable format|
**TRACKING PATH CHANGES**

Versioning  le removes and path changes

**git rm [file] ![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.007.png)**delete the  le from project and stage the removal for commit **git mv [existing-path] [new-path]**

change an existing  le path and stage the move

**git log --stat -M** show all commit logs with indication of any paths that moved

**IGNORING PATTERNS**

Preventing unintentional staging or commiting of  les

**logs/ \*.notes pattern\*/![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.008.png)**

Save a  le with desired pa erns as .gitignore with either direct string matches or wildcard globs.

**git config --global core.excludesfile [file]** system wide ignore pa ern for all local repositories

Retrieving updates from another repository and updating local repos

**git remote add [alias] [url]![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.009.png)**

add a git URL as an alias

**git fetch [alias]**

fetch down all the branches from that Git remote

**git merge [alias]/[branch]**

merge a remote branch into your current branch to bring it up to date **git push [alias] [branch]**

Transmit local branch commits to the remote repository branch

**git pull**

fetch and merge any commits from the tracking remote branch

**REWRITE HISTORY**

Rewriting branches, updating commits and clearing history

**git rebase [branch]![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.010.png)**

apply any commits of current branch ahead of speci ed one **git reset --hard [commit]**

clear staging area, rewrite working tree from speci ed commit

**TEMPORARY COMMITS**

Temporarily store modi ed, tracked  les  in order to change branches

**git stash![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.011.png)**

Save modi ed and staged changes

**git stash list**

list stack-order of stashed  le changes

**git stash pop**

write working from top of stash stack

**git stash drop**

discard  the changes from top of stash stack

Education![](Aspose.Words.66b69b2d-7eb5-4192-9820-a45e415e11e5.012.png)

Teach and learn be er, together. GitHub is free for students and teach- **education@github.com** ers. Discounts available for other educational uses. **education.github.com**
