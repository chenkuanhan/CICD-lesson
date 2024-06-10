# CICD-lesson

## git fetch & git pull

[git fetch & git pull.txt](https://github.com/user-attachments/files/15756014/git.fetch.git.pull.txt)

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
