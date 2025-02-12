# git--demo


# git session":-
-demo> git branch
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b dev      
Switched to a new branch 'dev'
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev

  (use "git add <file>..." to include in what will be committed)
        test.txt.py

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Prerana\Documents\project\git-demo> git checkout master
error: pathspec 'master' did not match any file(s) known to git
PS C:\Users\Prerana\Documents\project\git-demo> git checkout-b  master
git: 'checkout-b' is not a git command. See 'git --help'.
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b  master
Switched to a new branch 'master'
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev

No commits yet

PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b  master
Switched to a new branch 'master'
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev

No commits yet

PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev

No commits yet

On branch dev

No commits yet


No commits yet

No commits yet


Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test.py

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Prerana\Documents\project\git-demo> git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Disable this message with "git config advice.addEmptyPathspec false"
PS C:\Users\Prerana\Documents\project\git-demo> git add test.py
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   test.py

PS C:\Users\Prerana\Documents\project\git-demo> git commit -m "added test python code"
[dev (root-commit) 869f508] added test python code
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test.py
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev
nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
        modified:   test.py

no changes added to commit (use "git add" and/or "git commit -a")        
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b dev
fatal: a branch named 'dev' already exists
PS C:\Users\Prerana\Documents\project\git-demo> git branch               
* dev                                                                    
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b dev
fatal: a branch named 'dev' already exists                               
PS C:\Users\Prerana\Documents\project\git-demo> git checkout dev   
M       test.py
Already on 'dev'
PS C:\Users\Prerana\Documents\project\git-demo> git checkout master
error: pathspec 'master' did not match any file(s) known to git
PS C:\Users\Prerana\Documents\project\git-demo> git checkout -b master
Switched to a new branch 'master'
PS C:\Users\Prerana\Documents\project\git-demo> git checkout master   
M       test.py
Already on 'master'
PS C:\Users\Prerana\Documents\project\git-demo> git stat
git: 'stat' is not a git command. See 'git --help'.

The most similar commands are
        status
        stage
        stash
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
        modified:   test.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        new.py
        testing.py

no changes added to commit (use "git add" and/or "git commit -a")        
PS C:\Users\Prerana\Documents\project\git-demo> git restore --staged new.py
error: pathspec 'new.py' did not match any file(s) known to git
PS C:\Users\Prerana\Documents\project\git-demo> git status               
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
        modified:   test.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        new.py
        testing.py

no changes added to commit (use "git add" and/or "git commit -a")        
PS C:\Users\Prerana\Documents\project\git-demo> git add .
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.py
        modified:   test.py
        new file:   testing.py

PS C:\Users\Prerana\Documents\project\git-demo> git restore -- staged test.py
error: pathspec 'staged' did not match any file(s) known to git
PS C:\Users\Prerana\Documents\project\git-demo> git restore --staged test.py 
PS C:\Users\Prerana\Documents\project\git-demo> git status               
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.py
        new file:   testing.py

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)  
        modified:   test.py

PS C:\Users\Prerana\Documents\project\git-demo> git add .                
PS C:\Users\Prerana\Documents\project\git-demo> git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.py
        modified:   test.py
        new file:   testing.py

PS C:\Users\Prerana\Documents\project\git-demo> git log
commit 869f5082d18c92cd80a842b7dda7d21ab673bc1e (HEAD -> master, dev)
Author: prernask <karandeprerna@gmail.com>
Date:   Wed Feb 12 13:04:20 2025 +0530

    added test python code
PS C:\Users\Prerana\Documents\project\git-demo> git branch
  dev
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.py
        modified:   test.py
        new file:   testing.py

PS C:\Users\Prerana\Documents\project\git-demo> git commit -m "added new text file"
[master 46bee27] added new text file
 3 files changed, 8 insertions(+)
 create mode 100644 new.py
 create mode 100644 testing.py
PS C:\Users\Prerana\Documents\project\git-demo> git add new_dev.txt
PS C:\Users\Prerana\Documents\project\git-demo> git commit -m "added new dev.txt to dev"
[master b793065] added new dev.txt to dev
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new_dev.txt
PS C:\Users\Prerana\Documents\project\git-demo>


#github session:-
PS C:\Users\Prerana\Documents\project\github> git clone https://github.com/prernask/git--demo.git
Cloning into 'git--demo'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)    
Receiving objects: 100% (6/6), done.
PS C:\Users\Prerana\Documents\project\github> git sttaus
git: 'sttaus' is not a git command. See 'git --help'.

The most similar command is
        status
PS C:\Users\Prerana\Documents\project\github> git status
fatal: not a git repository (or any of the parent directories): .git
PS C:\Users\Prerana\Documents\project\github> cd git-demo
cd : Cannot find path 
'C:\Users\Prerana\Documents\project\github\git-demo' because it does 
not exist.
At line:1 char:1
+ cd git-demo
+ ~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\Preran...github  
   \git-demo:String) [Set-Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Command  
   s.SetLocationCommand

PS C:\Users\Prerana\Documents\project\github> cd git--demo
PS C:\Users\Prerana\Documents\project\github\git--demo> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git add .  
PS C:\Users\Prerana\Documents\project\github\git--demo> git commit -m "added my msg"
PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin main
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/prernask/git--demo.git/'
it/'
PS C:\Users\Prerana\Documents\project\github\git--demo> git status       
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin/main
fatal: 'origin/main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin main
PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin main
info: please complete authentication in your browser...
Everything up-to-date
PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin main
Everything up-to-date
PS C:\Users\Prerana\Documents\project\github\git--demo



# added file from local to github repo

PS C:\Users\Prerana\Documents\project\github> cd git--demo                
PS C:\Users\Prerana\Documents\project\github\git--demo> git add .
PS C:\Users\Prerana\Documents\project\github\git--demo> git status                  
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   README.md

PS C:\Users\Prerana\Documents\project\github\git--demo> git commit -m "added my msg"
[main 5ccdf86] added my msg
PS C:\Users\Prerana\Documents\project\github\git--demo> git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git commit -m "added my msg"
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git add .   
PS C:\Users\Prerana\Documents\project\github\git--demo> git add text.py
PS C:\Users\Prerana\Documents\project\github\git--demo> git status     
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git commit -m "added my msg"
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo> dir            


    Directory: C:\Users\Prerana\Documents\project\github\git--demo


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        12-02-2025     13:51           9951 README.md
-a----        12-02-2025     13:42             25 text.py


PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 556 bytes | 556.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/prernask/git--demo.git
   b82ce73..5ccdf86  main -> main
PS C:\Users\Prerana\Documents\project\github\git--demo> git push origin main
Everything up-to-date
PS C:\Users\Prerana\Documents\project\github\git--demo> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\Prerana\Documents\project\github\git--demo>

















