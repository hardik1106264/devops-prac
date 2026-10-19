# devops-prac

simple devops practical about git and github and this all and use so many command also fo rthat inspect this 

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
PS C:\Users\Admin\OneDrive\Desktop\It_143\git_143> 
