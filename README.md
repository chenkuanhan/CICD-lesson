[git_branch.txt](https://github.com/user-attachments/files/15756747/git_branch.txt)# CICD-lesson
### 參考檔案
[git_pull.pdf](https://github.com/user-attachments/files/15756066/git_pull.pdf)
[git fetch & git pull.txt](https://github.com/user-attachments/files/15756014/git.fetch.git.pull.txt)

[Uploading git_branWindows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。

安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Users\Asus> cd C:\Users\Asus\Documents\Web-lesson
PS C:\Users\Asus\Documents\Web-lesson> git init
Initialized empty Git repository in C:/Users/Asus/Documents/Web-lesson/.git/
PS C:\Users\Asus\Documents\Web-lesson> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        "\346\210\220\347\202\272\347\266\262\351\240\201\350\250\255\350\250\210\345\270\253\347\232\204\347\254\254\344\270\200\346\255\245/"

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\Web-lesson> git remote origin https://github.com/chenkuanhan/Web-lesson.git
error: unknown subcommand: `origin'
usage: git remote [-v | --verbose]
   or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
   or: git remote rename [--[no-]progress] <old> <new>
   or: git remote remove <name>
   or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
   or: git remote [-v | --verbose] show [-n] <name>
   or: git remote prune [-n | --dry-run] <name>
   or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
   or: git remote set-branches [--add] <name> <branch>...
   or: git remote get-url [--push] [--all] <name>
   or: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    -v, --[no-]verbose    be verbose; must be placed before a subcommand

PS C:\Users\Asus\Documents\Web-lesson> git remote add origin https://github.com/chenkuanhan/Web-lesson.git
PS C:\Users\Asus\Documents\Web-lesson> git remote -v
origin  https://github.com/chenkuanhan/Web-lesson.git (fetch)
origin  https://github.com/chenkuanhan/Web-lesson.git (push)
PS C:\Users\Asus\Documents\Web-lesson> git remote
origin
PS C:\Users\Asus\Documents\Web-lesson> git branch -v
PS C:\Users\Asus\Documents\Web-lesson> git pull origin master
remote: Enumerating objects: 628, done.
remote: Counting objects: 100% (628/628), done.
remote: Compressing objects: 100% (482/482), done.
remote: Total 628 (delta 111), reused 627 (delta 110), pack-reused 0
Receiving objects: 100% (628/628), 691.23 KiB | 832.00 KiB/s, done.
Resolving deltas: 100% (111/111), done.
From https://github.com/chenkuanhan/Web-lesson
 * branch            master     -> FETCH_HEAD
 * [new branch]      master     -> origin/master
PS C:\Users\Asus\Documents\Web-lesson> start .
PS C:\Users\Asus\Documents\Web-lesson> git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        "\346\210\220\347\202\272\347\266\262\351\240\201\350\250\255\350\250\210\345\270\253\347\232\204\347\254\254\344\270\200\346\255\245/"

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\Web-lesson> git add .
error: '成為網頁設計師的第一步/' does not have a commit checked out
fatal: adding files failed
PS C:\Users\Asus\Documents\Web-lesson> git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        "\346\210\220\347\202\272\347\266\262\351\240\201\350\250\255\350\250\210\345\270\253\347\232\204\347\254\254\344\270\200\346\255\245/"

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\Web-lesson> start .
PS C:\Users\Asus\Documents\Web-lesson> git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        The_first_step_for_a_web_designer/

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\Web-lesson> git add .
error: 'The_first_step_for_a_web_designer/' does not have a commit checked out
fatal: adding files failed
PS C:\Users\Asus\Documents\Web-lesson> git add --all
error: 'The_first_step_for_a_web_designer/' does not have a commit checked out
fatal: adding files failed
PS C:\Users\Asus\Documents\Web-lesson> git log
commit 6d6921c6a1e86bdc620d53ddf7fa8a5b2dc36520 (HEAD -> master, origin/master)
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 20:16:47 2024 +0800

    5 commit

commit 1c2657e7dec48a9a8cbacbdc5c3d03071b4ee04b
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 20:13:08 2024 +0800

    4 commit

commit 53f1235a0a1fc685dd198acd99ca7a99e3e32b2b
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 14:30:17 2024 +0800

    3rd commit

commit f6bb90390b75bcb8d8c717470d1bea437f57ec85
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 14:09:27 2024 +0800

    2nd commit

commit 790c7e5ad9cd7dc0376b16f711336e0fb543bbb0
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 13:48:52 2024 +0800

    first commit
PS C:\Users\Asus\Documents\Web-lesson>
PS C:\Users\Asus\Documents\Web-lesson> git add .
error: 'The_first_step_for_a_web_designer/' does not have a commit checked out
fatal: adding files failed
PS C:\Users\Asus\Documents\Web-lesson> start .
PS C:\Users\Asus\Documents\Web-lesson> git remote
origin
PS C:\Users\Asus\Documents\Web-lesson> git remote -v
origin  https://github.com/chenkuanhan/Web-lesson.git (fetch)
origin  https://github.com/chenkuanhan/Web-lesson.git (push)
PS C:\Users\Asus\Documents\Web-lesson> git add .
warning: in the working copy of 'The_first_step_for_a_web_designer/style.css', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'The_first_step_for_a_web_designer/練習檔.html', LF will be replaced by CRLF the next time Git touches it
PS C:\Users\Asus\Documents\Web-lesson> git add --all
PS C:\Users\Asus\Documents\Web-lesson> git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   The_first_step_for_a_web_designer/0.html
        new file:   The_first_step_for_a_web_designer/0.txt
        new file:   The_first_step_for_a_web_designer/01.html
        new file:   The_first_step_for_a_web_designer/01.png
        new file:   The_first_step_for_a_web_designer/01.txt
        new file:   The_first_step_for_a_web_designer/02.html
        new file:   The_first_step_for_a_web_designer/02.txt
        new file:   The_first_step_for_a_web_designer/03/03.html
        new file:   The_first_step_for_a_web_designer/03/03.txt
        new file:   The_first_step_for_a_web_designer/03/style.css
        new file:   The_first_step_for_a_web_designer/04/04-1.png
        new file:   The_first_step_for_a_web_designer/04/04-1.txt
        new file:   The_first_step_for_a_web_designer/04/04-2.png
        new file:   The_first_step_for_a_web_designer/04/04-2.txt
        new file:   The_first_step_for_a_web_designer/04/04-3.txt
        new file:   The_first_step_for_a_web_designer/04/Layout01.html
        new file:   The_first_step_for_a_web_designer/04/header_nav_main.png
        new file:   "The_first_step_for_a_web_designer/04/header\350\243\241\351\235\242\346\234\211nav.png"
        new file:   The_first_step_for_a_web_designer/04/layout02.html
        new file:   The_first_step_for_a_web_designer/05.html
        new file:   The_first_step_for_a_web_designer/05.txt
        new file:   "The_first_step_for_a_web_designer/HTML_CSS\347\267\264\347\277\222\346\252\224.zip"
        new file:   The_first_step_for_a_web_designer/style.css
        new file:   "The_first_step_for_a_web_designer/\345\215\200\345\241\212\345\205\203\347\264\240\345\217\212\350\241\214\345\205\247\345\205\203\347\264\240.png"
        new file:   "The_first_step_for_a_web_designer/\347\267\264\347\277\222\346\252\224.html"
        new file:   "The_first_step_for_a_web_designer/\351\207\221\351\255\232\351\203\275\350\203\275\346\207\202\347\266\262\351\240\201\350\250\255\350\250\210\345\205\245\351\226\200/temp.html"

PS C:\Users\Asus\Documents\Web-lesson> git branch
* master
PS C:\Users\Asus\Documents\Web-lesson> git branch -m branch2
PS C:\Users\Asus\Documents\Web-lesson> git branch
* branch2
PS C:\Users\Asus\Documents\Web-lesson> git remote -v
origin  https://github.com/chenkuanhan/Web-lesson.git (fetch)
origin  https://github.com/chenkuanhan/Web-lesson.git (push)
PS C:\Users\Asus\Documents\Web-lesson> git push origin branch2
Everything up-to-date
PS C:\Users\Asus\Documents\Web-lesson> git log
commit 6d6921c6a1e86bdc620d53ddf7fa8a5b2dc36520 (HEAD -> branch2, origin/master, origin/branch2)
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 20:16:47 2024 +0800

    5 commit

commit 1c2657e7dec48a9a8cbacbdc5c3d03071b4ee04b
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 20:13:08 2024 +0800

    4 commit

commit 53f1235a0a1fc685dd198acd99ca7a99e3e32b2b
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 14:30:17 2024 +0800

    3rd commit

commit f6bb90390b75bcb8d8c717470d1bea437f57ec85
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 14:09:27 2024 +0800

    2nd commit

commit 790c7e5ad9cd7dc0376b16f711336e0fb543bbb0
Author: Hank <kuanc1784@gmail.com>
Date:   Sun Jun 9 13:48:52 2024 +0800

    first commit
PS C:\Users\Asus\Documents\Web-lesson>
ch.txt…]()








## git fetch & git pull



**第一個實驗:(git pull origin master)**


```
Windows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。
安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Users\Asus> cd C:\Users\Asus\Documents\CICD-lesson
PS C:\Users\Asus\Documents\CICD-lesson> cd C:\Users\Asus\Documents\筆記
PS C:\Users\Asus\Documents\筆記> git init
Initialized empty Git repository in C:/Users/Asus/Documents/筆記/.git/
PS C:\Users\Asus\Documents\筆記> git remote -v
PS C:\Users\Asus\Documents\筆記> echo "筆記第一行內容" >> note.md
PS C:\Users\Asus\Documents\筆記> git remote set-url origin https://github.com/chenkuanhan/CICD-lesson.git
error: No such remote 'origin'
PS C:\Users\Asus\Documents\筆記> git fetch origin master
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Asus\Documents\筆記> git fetch origin
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Asus\Documents\筆記> git fetch origin/master
fatal: 'origin/master' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Asus\Documents\筆記> git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=<remote>/<branch> master

PS C:\Users\Asus\Documents\筆記> git pull origin master
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Asus\Documents\筆記> git remote -v
PS C:\Users\Asus\Documents\筆記> git remote set-url origin https://github.com/chenkuanhan/CICD-lesson.git
error: No such remote 'origin'
PS C:\Users\Asus\Documents\筆記> git remote set-url https://github.com/chenkuanhan/CICD-lesson.git
usage: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    --[no-]push           manipulate push URLs
    --[no-]add            add URL
    --[no-]delete         delete URLs

PS C:\Users\Asus\Documents\筆記> git remote set-url origin https://github.com/chenkuanhan/CICD-lesson.git
error: No such remote 'origin'
PS C:\Users\Asus\Documents\筆記> git remote add origin https://github.com/chenkuanhan/CICD-lesson.git
PS C:\Users\Asus\Documents\筆記> git remote -v
origin  https://github.com/chenkuanhan/CICD-lesson.git (fetch)
origin  https://github.com/chenkuanhan/CICD-lesson.git (push)
PS C:\Users\Asus\Documents\筆記> git pull
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.74 KiB | 222.00 KiB/s, done.
From https://github.com/chenkuanhan/CICD-lesson
 * [new branch]      master     -> origin/master
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> master

PS C:\Users\Asus\Documents\筆記> git pull origin master
From https://github.com/chenkuanhan/CICD-lesson
 * branch            master     -> FETCH_HEAD
PS C:\Users\Asus\Documents\筆記> start .
PS C:\Users\Asus\Documents\筆記> git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        note.md

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\筆記> git log
commit c8aebcb33cdb20476efad5f640d1104bfdebeedd (HEAD -> master, origin/master)
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:00:21 2024 +0800

    Update README.md

commit 3bc9589ea0a7bce1f24b6cd36ca1a198d7a30266
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 10:57:44 2024 +0800

    Initial commit
PS C:\Users\Asus\Documents\筆記> git commit -m "update file:note.md"
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        note.md

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\筆記> git add .
PS C:\Users\Asus\Documents\筆記> git commit -m "update file:note.md"
[master 742cbcc] update file:note.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 note.md
PS C:\Users\Asus\Documents\筆記> git status
On branch master
nothing to commit, working tree clean
PS C:\Users\Asus\Documents\筆記> git log
commit 742cbcc8da6ba78c9da1c1036e802d33bfa0e798 (HEAD -> master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:08:53 2024 +0800

    update file:note.md

commit c8aebcb33cdb20476efad5f640d1104bfdebeedd (origin/master)
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:00:21 2024 +0800

    Update README.md

commit 3bc9589ea0a7bce1f24b6cd36ca1a198d7a30266
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 10:57:44 2024 +0800

    Initial commit
PS C:\Users\Asus\Documents\筆記>
PS C:\Users\Asus\Documents\筆記> git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 20 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 294 bytes | 294.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/chenkuanhan/CICD-lesson.git
   c8aebcb..742cbcc  master -> master
PS C:\Users\Asus\Documents\筆記>

```

**第三個實驗:**

 **#Step.**

1. **git fetch**
2. **.git pull origin master**
```
PS C:\Users\Asus\Documents\筆記> git log
commit 27e41abf6821f06b79baabeeac721107a985f76d (HEAD -> master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:40:03 2024 +0800

    local 5th total 9th commits

commit 742cbcc8da6ba78c9da1c1036e802d33bfa0e798 (origin/master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:08:53 2024 +0800

    update file:note.md

commit c8aebcb33cdb20476efad5f640d1104bfdebeedd
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:00:21 2024 +0800

    Update README.md

commit 3bc9589ea0a7bce1f24b6cd36ca1a198d7a30266
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 10:57:44 2024 +0800

    Initial commit
PS C:\Users\Asus\Documents\筆記> git fetch
remote: Enumerating objects: 41, done.
remote: Counting objects: 100% (41/41), done.
remote: Compressing objects: 100% (39/39), done.
remote: Total 39 (delta 16), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (39/39), 18.90 KiB | 261.00 KiB/s, done.
From https://github.com/chenkuanhan/CICD-lesson
   742cbcc..920a8fc  master     -> origin/master
PS C:\Users\Asus\Documents\筆記> git log
commit 27e41abf6821f06b79baabeeac721107a985f76d (HEAD -> master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:40:03 2024 +0800

    local 5th total 9th commits

commit 742cbcc8da6ba78c9da1c1036e802d33bfa0e798
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:08:53 2024 +0800

    update file:note.md

commit c8aebcb33cdb20476efad5f640d1104bfdebeedd
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:00:21 2024 +0800

    Update README.md

commit 3bc9589ea0a7bce1f24b6cd36ca1a198d7a30266
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 10:57:44 2024 +0800

    Initial commit
PS C:\Users\Asus\Documents\筆記>


```

**第三個實驗:
1.git fetch
2.git pull origin master
**

```
PS C:\Users\Asus\Documents\筆記> git log
commit 27e41abf6821f06b79baabeeac721107a985f76d (HEAD -> master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:40:03 2024 +0800

    local 5th total 9th commits

commit 742cbcc8da6ba78c9da1c1036e802d33bfa0e798 (origin/master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:08:53 2024 +0800

    update file:note.md

commit c8aebcb33cdb20476efad5f640d1104bfdebeedd
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:00:21 2024 +0800

    Update README.md

commit 3bc9589ea0a7bce1f24b6cd36ca1a198d7a30266
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 10:57:44 2024 +0800

    Initial commit
PS C:\Users\Asus\Documents\筆記> git fetch
remote: Enumerating objects: 41, done.
remote: Counting objects: 100% (41/41), done.
remote: Compressing objects: 100% (39/39), done.
remote: Total 39 (delta 16), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (39/39), 18.90 KiB | 261.00 KiB/s, done.
From https://github.com/chenkuanhan/CICD-lesson
   742cbcc..920a8fc  master     -> origin/master
PS C:\Users\Asus\Documents\筆記> git log
commit 27e41abf6821f06b79baabeeac721107a985f76d (HEAD -> master)
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:40:03 2024 +0800

    local 5th total 9th commits

commit 742cbcc8da6ba78c9da1c1036e802d33bfa0e798
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:08:53 2024 +0800

    update file:note.md

commit c8aebcb33cdb20476efad5f640d1104bfdebeedd
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:00:21 2024 +0800

    Update README.md

commit 3bc9589ea0a7bce1f24b6cd36ca1a198d7a30266
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 10:57:44 2024 +0800

    Initial commit
PS C:\Users\Asus\Documents\筆記> git pull origin master
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 1.29 KiB | 59.00 KiB/s, done.
From https://github.com/chenkuanhan/CICD-lesson
 * branch            master     -> FETCH_HEAD
   920a8fc..02cddff  master     -> origin/master
Merge made by the 'ort' strategy.
 README.md                                          | 224 +++++++++
 mysql_log/Mysql0.txt                               |  19 +
 mysql_log/Mysql02.txt                              | 194 ++++++++
 mysql_log/Mysql03.txt                              | 448 ++++++++++++++++++
 mysql_log/Mysql04.txt                              | 519 +++++++++++++++++++++
 mysql_log/Mysql05.txt                              |  45 ++
 mysql_log/Mysql08.txt                              |  52 +++
 mysql_log/Mysql09.txt                              |  71 +++
 mysql_log/Mysql10.txt                              |  56 +++
 mysql_log/Mysql11.txt                              |  29 ++
 mysql_log/Mysql12.txt                              |  19 +
 mysql_log/Mysql13.txt                              |  94 ++++
 mysql_log/Mysql14.txt                              |  79 ++++
 mysql_log/Mysql15.txt                              | 119 +++++
 mysql_log/Mysql16.txt                              | 119 +++++
 mysql_log/Mysql17.txt                              | 156 +++++++
 mysql_log/Mysql18.txt                              | 460 ++++++++++++++++++
 mysql_log/Mysql19.txt                              |  77 +++
 mysql_log/Mysql20.txt                              | 174 +++++++
 mysql_log/Mysql21.txt                              | 481 +++++++++++++++++++
 mysql_log/Mysql22.txt                              |  92 ++++
 sql_code/cru.sql                                   |  14 +
 sql_code/insert_update.sql                         |  25 +
 ...346\226\207\345\255\227_drop_create_insert.sql" |  39 ++
 sql_code/setting.sql                               |  12 +
 ...17\222\345\205\245\350\263\207\346\226\231.sql" |  17 +
 26 files changed, 3634 insertions(+)
 create mode 100644 mysql_log/Mysql0.txt
 create mode 100644 mysql_log/Mysql02.txt
 create mode 100644 mysql_log/Mysql03.txt
 create mode 100644 mysql_log/Mysql04.txt
 create mode 100644 mysql_log/Mysql05.txt
 create mode 100644 mysql_log/Mysql08.txt
 create mode 100644 mysql_log/Mysql09.txt
 create mode 100644 mysql_log/Mysql10.txt
 create mode 100644 mysql_log/Mysql11.txt
 create mode 100644 mysql_log/Mysql12.txt
 create mode 100644 mysql_log/Mysql13.txt
 create mode 100644 mysql_log/Mysql14.txt
 create mode 100644 mysql_log/Mysql15.txt
 create mode 100644 mysql_log/Mysql16.txt
 create mode 100644 mysql_log/Mysql17.txt
 create mode 100644 mysql_log/Mysql18.txt
 create mode 100644 mysql_log/Mysql19.txt
 create mode 100644 mysql_log/Mysql20.txt
 create mode 100644 mysql_log/Mysql21.txt
 create mode 100644 mysql_log/Mysql22.txt
 create mode 100644 sql_code/cru.sql
 create mode 100644 sql_code/insert_update.sql
 create mode 100644 "sql_code/ithema_insert_\346\233\277\344\273\243\346\226\207\345\255\227_drop_create_insert.sql"
 create mode 100644 sql_code/setting.sql
 create mode 100644 "sql_code/\346\217\222\345\205\245\350\263\207\346\226\231.sql"
PS C:\Users\Asus\Documents\筆記> git log
commit 9f36bdc61df7cc27038774270d45903733f576d2 (HEAD -> master)
Merge: 27e41ab 02cddff
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:43:06 2024 +0800

    Merge branch 'master' of https://github.com/chenkuanhan/CICD-lesson

    先執行git fetch 後執行 git pull origin master

commit 02cddff6869e94d9eca65a107f338c6c6f0b6371 (origin/master)
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:42:03 2024 +0800

    Update README.md

commit 27e41abf6821f06b79baabeeac721107a985f76d
Author: Hank <kuanc1784@gmail.com>
Date:   Mon Jun 10 11:40:03 2024 +0800

    local 5th total 9th commits

commit 920a8fc9c3beb05efd3296afa17f7d6e84d0e6ee
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:33:22 2024 +0800

    Add files via upload

commit baa4f9dba7a490841d13a8c6cc69064fac5a04de
Author: chenkuanhan <104495841+chenkuanhan@users.noreply.github.com>
Date:   Mon Jun 10 11:23:37 2024 +0800

    Update README.md

commit 1b6bdaaa802a9bcd69d1e5cc394e136762238a37
```



![螢幕擷取畫面 2024-06-10 114407](https://github.com/chenkuanhan/CICD-lesson/assets/104495841/b4cf89db-bd70-4b3b-9475-d7095b5bf6d5)



