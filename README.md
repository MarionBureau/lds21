Exercice Git GitHub
Detail des requettes Git Bash
mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB
$ touch index.html

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB
$ git init
Initialized empty Git repository in C:/Users/mbure/Documents/Digital School B1/G

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git config --global user.name 'MarionBureau'

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git config --global user.email 'm.bureau04@gmail.com'

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git add index.html

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html


mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ touch style.css

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        style.css


mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git add *.html *.css

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
        new file:   style.css


mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git commit
[master (root-commit) 6776f0d] 1ère sauvegarde
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
 create mode 100644 style.css

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git status
On branch master
nothing to commit, working tree clean

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html
        modified:   style.css

no changes added to commit (use "git add" and/or "git commit -a")

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git add *.html *.css

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git commit-m 'changement fichier html et css'
git: 'commit-m' is not a git command. See 'git --help'.

The most similar command is
        commit-tree
mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git branch --list
* master

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git branch master
fatal: A branch named 'master' already exists.

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git branch file

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (maste
$ git checkout file
Switched to branch 'file'
M       index.html
M       style.css

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$ git branch --list
* file
  master
mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$ git remote add origin https://github.com/MarionBureau/lds21.git

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 236 bytes | 3.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/MarionBureau/lds21.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$ touch README.md
mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$ git add .

mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$ git commit -m 'Ajout du fichier READ.ME'
[file 1f8a512] Ajout du fichier READ.ME
 3 files changed, 150 insertions(+)
 create mode 100644 README.mdmbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$  git push --set-upstream origin file
Enumerating objects: 11, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (8/8), 1.89 KiB | 969.00 KiB/s, done.
Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'file' on GitHub by visiting:
remote:      https://github.com/MarionBureau/lds21/pull/new/file
remote:
To https://github.com/MarionBureau/lds21.git
 * [new branch]      file -> file
Branch 'file' set up to track remote branch 'file' from 'origin'.

 mbure@LAPTOP-5NCBR2S9 MINGW64 ~/Documents/Digital School B1/Git/TP GITHUB (file)
$  git push --set-upstream origin file
Enumerating objects: 11, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (8/8), 1.89 KiB | 969.00 KiB/s, done.
Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'file' on GitHub by visiting:
remote:      https://github.com/MarionBureau/lds21/pull/new/file
remote:
To https://github.com/MarionBureau/lds21.git
 * [new branch]      file -> file
Branch 'file' set up to track remote branch 'file' from 'origin'.


Code HTML 
Ajout titre H1

Ajout titre H2
