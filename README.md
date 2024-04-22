# Git exercise

## Bundle 1

### Exercise 1

```bash

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (master)
$ git branch -m master main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        hello.txt

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        hello.txt
        index.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add index.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        hello.txt


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        hello.txt


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   hello.txt
        new file:   index.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git commit -m "First commit of the files"
[main (root-commit) 1a42f05] First commit of the files
 3 files changed, 14 insertions(+)
 create mode 100644 README.md
 create mode 100644 hello.txt
 create mode 100644 index.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
nothing to commit, working tree clean

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git remote add origin https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch -M main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 473 bytes | 473.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch dev

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
* main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout dev
Switched to branch 'dev'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (dev)
$ git branch test

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (dev)
$ git branch
* dev
  main
  test

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (dev)
$ git checkout test
Switched to branch 'test'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (test)
$ git checkout dev
Switched to branch 'dev'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (dev)
$ git branch -d test
Deleted branch test (was 1a42f05).

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (dev)
$

```