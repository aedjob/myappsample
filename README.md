#MyApp
This is my App

details for online youtube tutorial https://www.youtube.com/watch?v=SWYqp7iY_Tc

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   app.js
        new file:   index.html


Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git commit
Aborting commit due to empty commit message.

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git commit
[master (root-commit) 83dd2cf]  Initial commit
 2 files changed, 8 insertions(+)
 create mode 100644 app.js
 create mode 100644 index.html

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git status
On branch master
nothing to commit, working tree clean

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   app.js

no changes added to commit (use "git add" and/or "git commit -a")

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git add .

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git commit -m 'Changed app.js'
[master eedb4a1] Changed app.js
 1 file changed, 1 insertion(+)

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ touch .gitignore

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ touch log.txt

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git add .

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   log.txt


Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git add .

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   dir1/app1.js
        new file:   log.txt


Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git branch login

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ get status
bash: get: command not found

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   dir1/app1.js
        new file:   log.txt


Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git commit -m 'another change'
[master b7073a8] another change
 3 files changed, 3 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 dir1/app1.js
 create mode 100644 log.txt

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git checkout login
Switched to branch 'login'

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (login)
$ touch login.html

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (login)
$ git add .

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (login)
$ git commit -m 'login form'
[login 0084a62] login form
 3 files changed, 3 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 login.html

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (login)
$ git checkout master
Switched to branch 'master'

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git checkout login
Switched to branch 'login'

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (login)
$ git checkout master
Switched to branch 'master'

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git merge login
Merge made by the 'recursive' strategy.
 dir2/app2.js | 1 +
 index.html   | 1 +
 login.html   | 1 +
 3 files changed, 3 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 login.html

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git remote add origin https://github.com/aedjob/myappsample.git

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git remote
origin

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git push -u origin master
Enumerating objects: 20, done.
Counting objects: 100% (20/20), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (20/20), 1.52 KiB | 222.00 KiB/s, done.
Total 20 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/aedjob/myappsample.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ touch README.md

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git add .

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git commit -m 'Added readme'
[master 0c3daf9] Added readme
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 278 bytes | 139.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/aedjob/myappsample.git
   027d294..0c3daf9  master -> master

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ git pull
Already up to date.

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$ ^C

Alfredo@DESKTOP-2GCQEGE MINGW64 ~/Desktop/myapp (master)
$
