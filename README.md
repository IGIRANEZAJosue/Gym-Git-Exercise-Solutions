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

## Bundle 3

### Exercise 1

```bash


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git branch ft/team-page

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  ft/team-page
  main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/service-redesign)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git status
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git commit -a -m "Created Team page"
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git commit -a -m "Created Team page"
[ft/team-page c35d0e0] Created Team page
 1 file changed, 13 insertions(+)
 create mode 100644 team.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ ^C

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$  git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 437 bytes | 437.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 6 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch ft/contact-page

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
* main

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git log
commit c35d0e0644ffbea7d0d040b7a8169a97edd42d6b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:49:55 2024 +0200

    Created Team page

commit 9e9fa8892a480b9445f2615cd3c5b34eac3d9b35 (origin/ft/service-redesign, ft/service-redesign)
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:44:17 2024 +0200

    Updated Readme

commit a9b900b841a56a06c6e0b4126ebeeb35511283b8
Merge: 4681db9 e3fcf1c
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:40:42 2024 +0200

    Merge branch 'main' into ft/service-redesign

commit 4681db951d582c03a7eecf92aeb6ee941a1c5d9c
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:38:24 2024 +0200

    resolved conflict

commit e3fcf1cd7a0d480a65609ac719aed9fc64993d23 (main, ft/contact-page)
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:27:16 2024 +0200


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git cherry-pick ^C

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git cherry-pick c35d0e0644ffbea7d0d040b7a8169a97edd42d6b
[ft/contact-page 6feb281] Created Team page
 Date: Mon Apr 22 17:49:55 2024 +0200
 1 file changed, 13 insertions(+)
 create mode 100644 team.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git commit -m 'Created contact page'
[ft/contact-page 90792ca] Created contact page
 1 file changed, 13 insertions(+)
 create mode 100644 contact.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ ^C

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 716 bytes | 716.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git branch ft/faq-page

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/contact-page)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git add .

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git status
On branch ft/faq-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   faq.html


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git commit -m "Create FAQ page"
[ft/faq-page 8933389] Create FAQ page
 1 file changed, 13 insertions(+)
 create mode 100644 faq.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 430 bytes | 430.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git log
commit 8933389d2d1b724c65bbc51eb1d6ff7977d281e8 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 19:43:41 2024 +0200

    Create FAQ page

commit 90792cae3dd089f57e1b988fc6509aae2e7a97cf (origin/ft/contact-page, ft/contact-page)
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 19:36:44 2024 +0200

    Created contact page

commit 6feb281068532e5baee5327e0fc2bca031166ee0
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:49:55 2024 +0200

    Created Team page

commit e3fcf1cd7a0d480a65609ac719aed9fc64993d23 (main)
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:27:16 2024 +0200

    Change in the service page

commit 3ee9133a5d5c7dcbc5b30e4755060fcfb4307bc4
Author: Josue Igiraneza <igiranezaj28@gmail.com>
Date:   Mon Apr 22 17:10:21 2024 +0200

    Made changes to services

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git revert 6feb281068532e5baee5327e0fc2bca031166ee0
[ft/faq-page 0346b1f] Revert "Created Team page"
 1 file changed, 13 deletions(-)
 delete mode 100644 team.html

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 280 bytes | 280.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/IGIRANEZAJosue/Gym-Git-Exercise-Solutions.git
   8933389..0346b1f  ft/faq-page -> ft/faq-page

Igiraneza@DESKTOP-2M35984 MINGW64 ~/Desktop/Native/git-exercises (ft/faq-page)
$

```
