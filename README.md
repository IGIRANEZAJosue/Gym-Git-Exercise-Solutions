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


### Exercise 2

```bash
Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash list

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash
Saved working directory and index state WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash
Saved working directory and index state WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 65ec762 delete files
stash@{1}: WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash
Saved working directory and index state WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 65ec762 delete files
stash@{1}: WIP on main: 65ec762 delete files
stash@{2}: WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (9a8ab6bd81287758125550eeb4b2876e29d6c9e8)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 65ec762 delete files
stash@{1}: WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (0f05a1cf34930f065b9e7ec8f2d23f748a4f3ddf)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git commit -a -m "Stashed the changes"
[main 85602d5] Stashed the changes
 2 files changed, 26 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 527 bytes | 527.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   65ec762..85602d5  main -> main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash list
stash@{0}: WIP on main: 65ec762 delete files

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (e0b1326087a821d48ccd23ca120746af115b5e32)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git reset --hard
HEAD is now at 85602d5 Stashed the changes

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$

```
