# Gym-Git-Exercise-Solutions
/* Bundle 1*/
//Exercise 1

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions       
$ git init
Initialized empty Git repository in C:/Users/hp/Desktop/Gym Git Exercise Solutions/.git/

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (master)
$ git branch -m master main

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git commit -m"renamed main branch to master"
[main (root-commit) de52689] renamed main branch to master
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
 create mode 100644 styles.css

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git remote add origin <https://github.com/tpambrose/Gym-Git-Exercise
-Solutions>
bash: syntax error near unexpected token `newline'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git remote add origin https://github.com/tpambrose/Gym-Git-Exercise-Solutions

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git remote -v
origin  https://github.com/tpambrose/Gym-Git-Exercise-Solutions (fetch)
origin  https://github.com/tpambrose/Gym-Git-Exercise-Solutions (push)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use        

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking     
upstream, see 'push.autoSetupRemote' in 'git help config'.


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$  git push --set-upstream origin main
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/tpambrose/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

$ git fetch --help

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git fetch --all
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 886 bytes | 80.00 KiB/s, done.
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * [new branch]      main       -> origin/main

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git push 
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git push --set-upstream origin main
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/tpambrose/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git pull origin main
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git push origin main
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/tpambrose/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
fatal: refusing to merge unrelated histories

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)

$ git pull origin main --allow-unrelated-histories
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.
 README.md | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)

$ git push origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 575 bytes | 575.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
   d514e9b..097f616  main -> main

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)

$ git checkout -b dev
Switched to a new branch 'dev'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git checkout -b test
Switched to a new branch 'test'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (test)
$ git checkout dev
Switched to branch 'dev'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git branch -d test
Deleted branch test (was 097f616).

//exercise 2

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash save "first changes"
Saved working directory and index state On dev: first changes

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash save "changes for about page"
Saved working directory and index state On dev: changes for about page

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash save "changes for team page"
Saved working directory and index state On dev: changes for team page

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git pop stash --help
git: 'pop' is not a git command. See 'git --help'.

The most similar command is
        log

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash --help

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash --help

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash list 
stash@{0}: On dev: changes for team page
stash@{1}: On dev: changes for about page
stash@{2}: On dev: first changes

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (a76b253d754a668f39d5403a195178c5d6505741)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash list 
stash@{0}: On dev: changes for team page
stash@{1}: On dev: first changes

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{1} (d4239602abccabeecd9d4e97c3213b4d445f8439)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git commit -m"stashed and committed the changes"
[dev d87cda8] stashed and committed the changes
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git push origin main
Everything up-to-date

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash list
stash@{0}: On dev: changes for team page

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{0} (a8348be4cd326c03af32bbf503cb52c5f1273dbf)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git reset team.html
Unstaged changes after reset:
M       README.md

/*bundle 2*/
//exercise 1

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/bundle-2)
$ git commit -m"created services page "
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)      
        services.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/bundle-2)
$ git add services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/bundle-2)
$ git commit -m"created services page "
[ft/bundle-2 92546e8] created services page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 501 bytes | 250.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting 
remote:      https://github.com/tpambrose/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * [new branch]      ft/bundle-2 -> ft/bundle-2

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/bundle-2)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git checkout dev 
Switched to branch 'dev'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git check out main
git: 'check' is not a git command. See 'git --help'.

The most similar command is
        checkout

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git checkout main 
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.  
Aborting

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git add  README.md

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git commit -m" added the stepsp to readme in dev branch "
[dev 459a3e9]  added the stepsp to readme in dev branch
 1 file changed, 3 insertions(+)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git push origin dev 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 346 bytes | 346.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects. 
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
   3ba6f6e..459a3e9  dev -> dev

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (dev) 
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git pull origin main 
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git branch 
  dev
  ft/bundle-2
* main

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git add services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git commit -m"made changes to the service page -added an new paragra
ph"
[ft/service-redesign e0f3b61] made changes to the service page -added an new paragraph
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 548 bytes | 274.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/tpambrose/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * [new branch]      ft/service-redesign -> ft/service-redesign       

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)      
        team.html

nothing added to commit but untracked files present (use "git add" to track)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git checkout main 
Already on 'main'
Your branch is up to date with 'origin/main'.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git add service.html
fatal: pathspec 'service.html' did not match any files

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ ls
index.html  README.md  services.html  styles.css  team.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git commit -m"added new changes to service.html on main branch"
[main 6a3f6d7] added new changes to service.html on main branch
 2 files changed, 24 insertions(+)
 create mode 100644 services.html
 create mode 100644 team.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git push origin main 
Enumerating objects: 5, done.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 629 bytes | 314.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
   097f616..6a3f6d7  main -> main

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git diff

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git diff

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git diff main 
diff --git a/services.html b/services.html
index f7f5a7e..46d16ff 100644
--- a/services.html
+++ b/services.html
@@ -7,6 +7,6 @@
 </head>
 <body>
     <p>hey this is my services page </p>
-    <p>hey i changed something</p>
+    <p>hey i am the second paragraph of the page </p>
 </body>
diff --git a/team.html b/team.html
deleted file mode 100644
diff --git a/team.html b/team.html
deleted file mode 100644
index 62d407e..0000000
--- a/team.html
+++ /dev/null
@@ -1,12 +0,0 @@
-<!DOCTYPE html>

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.     

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git merge main
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'  
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git commit -m"Merge main into ft/service-redesign branch"
[ft/service-redesign 1e045a9] Merge main into ft/service-redesign branch

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git add services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git commit -m"Resolve conflicts in services.html"
On branch ft/service-redesign
nothing to commit, working tree clean

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git add services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git commit -m "Resolve conflicts in services.html"
On branch ft/service-redesign
nothing to commit, working tree clean

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git add services.html

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git commit -m "Resolve conflicts in services.html"
[ft/service-redesign 1860dda] Resolve conflicts in services.html
 1 file changed, 12 deletions(-)

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git merge main
Already up to date.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git pull origin main
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git commit -m"merge main into ft/service-redesign branch"
On branch ft/service-redesign
nothing to commit, working tree clean

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 ! [rejected]        ft/service-redesign -> ft/service-redesign (fetch first)
error: failed to push some refs to 'https://github.com/tpambrose/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 896 bytes | 52.00 KiB/s, done.
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
   e0f3b61..89d6631  ft/service-redesign -> origin/ft/service-redesign
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> ft/service-redesign  


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 ! [rejected]        ft/service-redesign -> ft/service-redesign (non-fast-forward)
error: failed to push some refs to 'https://github.com/tpambrose/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.      
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> ft/service-redesign  


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git pull origin main
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 ! [rejected]        ft/service-redesign -> ft/service-redesign (non-fast-forward)
error: failed to push some refs to 'https://github.com/tpambrose/Gym-Git-Exercise-Solutions'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.      
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git pull origin main
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ FETCH_HEAD
bash: FETCH_HEAD: command not found

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git pull upstream main
fatal: 'upstream' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git pull origin ft/service-redesign
From https://github.com/tpambrose/Gym-Git-Exercise-Solutions
 * branch            ft/service-redesign -> FETCH_HEAD
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.     

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git add service.html
fatal: pathspec 'service.html' did not match any files

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git add .

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   services.html


hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign|MERGING)
$ git commit -m"resolved changes in service page"
[ft/service-redesign dd2f9d2] resolved changes in service page

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 748 bytes | 374.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects. 
To https://github.com/tpambrose/Gym-Git-Exercise-Solutions
   89d6631..dd2f9d2  ft/service-redesign -> ft/service-redesign       

hp@DESKTOP-VLJO66J MINGW64 ~/Desktop/Gym Git Exercise Solutions (ft/service-redesign)
$ git checkout dev
Switched to branch 'dev'

