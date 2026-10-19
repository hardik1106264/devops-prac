
this is basic git and github devops practical 

and all this command 

PS C:\Users\Admin\OneDrive\Desktop\It_143> cd git_143
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git init
Initialized empty Git repository in C:/Users/Admin/OneDrive/Desktop/It_143/git_143/.git/
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git add .
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git commit -m "first commit"
[master (root-commit) d379013] first commit
 1 file changed, 13 insertions(+)
 create mode 100644 index.html
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git log
commit d379013647b95221f7ac5cad5362df103a8981a7 (HEAD -> master)
Author: hardik1106264 <24itucs124@gmail.com>
Date:   Mon Oct 19 10:45:14 2026 +0530

    first commit
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git log --graph --all
* commit d379013647b95221f7ac5cad5362df103a8981a7 (HEAD -> master)
  Author: hardik1106264 <24itucs124@gmail.com>
  Date:   Mon Oct 19 10:45:14 2026 +0530
  
      first commit
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git status                  
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git add .
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git commit -m "second change"
[master b501cb6] second change
 1 file changed, 2 insertions(+)
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git log
commit b501cb6cca75e73ad8f6dc2f5e2d850cd9c9a41d (HEAD -> master)
Author: hardik1106264 <24itucs124@gmail.com>
Date:   Mon Oct 19 10:46:50 2026 +0530

    second change

commit d379013647b95221f7ac5cad5362df103a8981a7
Author: hardik1106264 <24itucs124@gmail.com>
Date:   Mon Oct 19 10:45:14 2026 +0530

PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git log --oneline --graph
* b501cb6 (HEAD -> master) second change
* d379013 first commit
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git branch devlopment
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git checkout devlopment
Switched to branch 'devlopment'
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git branch
* devlopment
  master
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git status
On branch devlopment
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git commit -m "new branch"
On branch devlopment
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git add .
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git commit -m "new branch"
[devlopment fe88d51] new branch
 1 file changed, 21 insertions(+)
 create mode 100644 about.html
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> ^C
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git remote add origin https://github.com/hardik1106264/devops-prac.git

PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git checkout master
Switched to branch 'master'
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git merge devlopment
Updating b501cb6..fe88d51
Fast-forward
 about.html | 21 +++++++++++++++++++++
 1 file changed, 21 insertions(+)
 create mode 100644 about.html
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> git push -u origin master
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (9/9), 1.10 KiB | 75.00 KiB/s, done.
Total 9 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/hardik1106264/devops-prac/pull/new/master
remote: 
To https://github.com/hardik1106264/devops-prac.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> 
