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

## Bundle 2

### Exercise 2

```bash

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git pull
Already up to date.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git commit -m "Added changes to the services page"
[main 550d6e5] Added changes to the services page
 1 file changed, 2 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 363.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   cbb2bdd..550d6e5  main -> main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git reset --hard
HEAD is now at 550d6e5 Added changes to the services page

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout ft/service-redesign
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
* ft/bundle-2
  ft/service-redesign
  main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/bundle-2)
$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git commit -m "Added changes to services"
[ft/service-redesign b87594a] Added changes to services
 1 file changed, 2 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ ^C

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 359 bytes | 359.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git commit -m "Made changes to services"
[main 3ee9133] Made changes to services
 1 file changed, 1 insertion(+), 1 deletion(-)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 345 bytes | 345.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   550d6e5..3ee9133  main -> main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
Merge made by the 'ort' strategy.
 services.html | 2 ++
 1 file changed, 2 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git merge main
Already up to date.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git checkout main
Already on 'main'
M       services.html
Your branch is up to date with 'origin/main'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout ft/service-redesign
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout ft/service-redesign
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git commit -a -m "Change to services"
[ft/service-redesign c6f8119] Change to services
 1 file changed, 1 insertion(+), 3 deletions(-)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 638 bytes | 638.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   b87594a..c6f8119  ft/service-redesign -> ft/service-redesign

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git commit -m "Change in the service page"
[main e3fcf1c] Change in the service page
 1 file changed, 1 insertion(+), 1 deletion(-)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 318 bytes | 318.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   3ee9133..e3fcf1c  main -> main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git diff ft/service-redesign main
diff --git a/services.html b/services.html
index ec362c4..6484b7f 100644
--- a/services.html
+++ b/services.html
@@ -9,7 +9,7 @@

    <h1>Services</h1>

-   <p>This is a change to the services page that'll create a conflict ..</p>
+   <p>This is a change to the services page that'll </p>

 </body>
 </html>
\ No newline at end of file

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git commit
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git commit -a
[ft/service-redesign 4681db9] resolved conflict
 1 file changed, 1 insertion(+), 1 deletion(-)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign|MERGING)
$ git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

nothing to commit, working tree clean

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$
```

## Bundle 4

### Exercise 1

```bash


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 9 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git remote add git-copy https://github.com/IGIRANEZAJosue/bundle-4-exercise-1.git

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git remote
git-copy
origin

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git commit -m "changes to homepage - bundle 4 ex 1"
[main caa2897] changes to homepage - bundle 4 ex 1
 1 file changed, 2 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push origin
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git pull
Merge made by the 'ort' strategy.
 README.md | 317 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 team.html |  13 +++
 2 files changed, 330 insertions(+)
 create mode 100644 team.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push origin
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 631 bytes | 315.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   293ab1c..cb1bb6f  main -> main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git push git-copy
Enumerating objects: 59, done.
Counting objects: 100% (59/59), done.
Delta compression using up to 8 threads
Compressing objects: 100% (56/56), done.
Writing objects: 100% (59/59), 10.66 KiB | 496.00 KiB/s, done.
Total 59 (delta 26), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (26/26), done.
To https://github.com/IGIRANEZAJosue/bundle-4-exercise-1.git
 * [new branch]      main -> main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$

```

### Exercise 2

```bash


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git commit -m "Made changes to some files"
[ft/footer f3fcf38] Made changes to some files
 2 files changed, 4 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git commit -m "Made changes to some files(again)"
[ft/footer c58f366] Made changes to some files(again)
 1 file changed, 7 insertions(+), 1 deletion(-)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 955 bytes | 955.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        home.html
Please commit your changes or stash them before you switch branches.
Aborting

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git push --set-upstream origin ft/footer
Everything up-to-date
branch 'ft/footer' set up to track 'origin/ft/footer'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git push origin ft/footer
Everything up-to-date

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        home.html
Please commit your changes or stash them before you switch branches.
Aborting

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git comit -m "home"
git: 'comit' is not a git command. See 'git --help'.

The most similar command is
        commit

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git comnmit -m "home"
git: 'comnmit' is not a git command. See 'git --help'.

The most similar command is
        commit

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git commit -m "home"
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git commit -m "home"
[ft/footer 9e0efdf] home
 1 file changed, 5 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/squashing)
$ git merge --squash ft/footer
Updating 8de0618..9e0efdf
Fast-forward
Squash commit -- not updating HEAD
 about.html | 8 ++++++++
 home.html  | 7 +++++++
 2 files changed, 15 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/squashing)
$ git commit -m "Footer changes squashing"
[ft/squashing 085d2ad] Footer changes squashing
 2 files changed, 15 insertions(+)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/squashing)
$ git push origin ft/squashing
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 727 bytes | 727.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/squashing)
$

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/squashing)
$

```