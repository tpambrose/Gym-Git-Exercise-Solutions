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
