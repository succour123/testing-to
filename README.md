sujatakumari@sujata-mca3:/mnt/c$ mkdir testing-to
sujatakumari@sujata-mca3:/mnt/c$ cd testing
testing/    testing-to/
sujatakumari@sujata-mca3:/mnt/c$ cd testing-to
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git init
Initialized empty Git repository in /mnt/c/testing-to/.git/
sujatakumari@sujata-mca3:/mnt/c/testing-to$ ls -a
.  ..  .git
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
sujatakumari@sujata-mca3:/mnt/c/testing-to$ touch README.md
sujatakumari@sujata-mca3:/mnt/c/testing-to$ ls -l
total 0
-rwxrwxrwx 1 sujatakumari sujatakumari 0 Jan 22 08:52 README.md
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)sujatakumari@sujata-mca3:/mnt/c/testing-to$ git add README.MD
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)sujatakumari@sujata-mca3:/mnt/c/testing-to$ git add README.mdd
fatal: pathspec 'README.mdd' did not match any files
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git add README.md
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

sujatakumari@sujata-mca3:/mnt/c/testing-to$ git commit -m "second commit"
[main (root-commit) 38b6b9a] second commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git log
commit 38b6b9a4be744165bf0730366958feb85ab7a322 (HEAD -> main)
Author: succour123 <m2sites3322@gmail.com>
Date:   Sun Jan 22 08:55:01 2023 +0530

    second commit
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git remote add origin git@github.com:succour123/testing-to.git
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git push origin
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

sujatakumari@sujata-mca3:/mnt/c/testing-to$ git status
On branch main
nothing to commit, working tree clean
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git  branch
* main
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 212 bytes | 9.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:succour123/testing-to.git
 * [new branch]      main -> main
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git status
On branch main
nothing to commit, working tree clean
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git log
commit 38b6b9a4be744165bf0730366958feb85ab7a322 (HEAD -> main, origin/main)
Author: succour123 <m2sites3322@gmail.com>
Date:   Sun Jan 22 08:55:01 2023 +0530

    second commit
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git branch -r
  origin/main
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git branch -a
* main
  remotes/origin/main
sujatakumari@sujata-mca3:/mnt/c/testing-to$ git branch --vv
