# git_github_tut
Repository code has been cloned
test 1
PS C:\laur\work\git_folder> git clone https://github.com/ailacos/git_github_tut.git
Cloning into 'git_github_tut'...
warning: You appear to have cloned an empty repository.
PS C:\laur\work\git_folder> git status
fatal: not a git repository (or any of the parent directories): .git
PS C:\laur\work\git_folder> ls

    Directory: C:\laur\work\git_folder


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----          9/9/2024   4:16 AM                git_github_tut



No commits yet

  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md

PS C:\laur\work\git_folder\git_github_tut> get add readme.md
get : The term 'get' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if a path was included,        
+ get add readme.md
+ ~~~
 
PS C:\laur\work\git_folder\git_github_tut> git add .        
PS C:\laur\work\git_folder\git_github_tut> git commit -m "changes by adding readme.md file"
[main (root-commit) 70bbe1f] changes by adding readme.md file
 1 file changed, 3 insertions(+)
 create mode 100644 readme.md
PS C:\laur\work\git_folder\git_github_tut> git status
On branch main
Your branch is based on 'origin/main', but the upstream is gone.

nothing to commit, working tree clean
PS C:\laur\work\git_folder\git_github_tut> git branch --unset-upstream
PS C:\laur\work\git_folder\git_github_tut> git status
PS C:\laur\work\git_folder\git_github_tut> git diff
PS C:\laur\work\git_folder\git_github_tut> git add .
that the path is correct and try again.
At line:1 char:1
+ c
+ ~
    + CategoryInfo          : ObjectNotFound: (c:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
 
[main afd1c13] add two files requirents.txt and etl.ipynb
 2 files changed, 176 insertions(+)
 create mode 100644 etl.ipynb
 create mode 100644 requirements.txt
PS C:\laur\work\git_folder\git_github_tut> git diff
PS C:\laur\work\git_folder\git_github_tut> git status
On branch main
nothing to commit, working tree clean
PS C:\laur\work\git_folder> cd .\git_github_tut\
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   etl.ipynb
no changes added to commit (use "git add" and/or "git commit -a")
gir : The term 'gir' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if a path was included,        
At line:1 char:1
+ gir commit -a "added numpy in etl.ipynb"
    + CategoryInfo          : ObjectNotFound: (gir:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\laur\work\git_folder\git_github_tut> git commit -a "added numpy in etl.ipynb"
fatal: paths 'added numpy in etl.ipynb ...' with -a does not make sense
PS C:\laur\work\git_folder\git_github_tut> git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
PS C:\laur\work\git_folder\git_github_tut> git add .
warning: in the working copy of 'etl.ipynb', LF will be replaced by CRLF the next time Git touches it
PS C:\laur\work\git_folder\git_github_tut> git commit -a "added numpy in etl.ipynb"
fatal: paths 'added numpy in etl.ipynb ...' with -a does not make sense
PS C:\laur\work\git_folder\git_github_tut> git commit  "added numpy in etl.ipynb"
error: pathspec 'added numpy in etl.ipynb' did not match any file(s) known to git
PS C:\laur\work\git_folder\git_github_tut> git commit  -m "added numpy in etl.ipynb"
[main 66ce129] added numpy in etl.ipynb
 1 file changed, 1 insertion(+)
PS C:\laur\work\git_folder\git_github_tut> git push
To push the current branch and set the remote as upstream, use
    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\laur\work\git_folder\git_github_tut>  git push --set-upstream origin main
Enumerating objects: 10, done.
Delta compression using up to 4 threads
Writing objects: 100% (10/10), 2.83 KiB | 413.00 KiB/s, done.
Total 10 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ailacos/git_github_tut.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\laur\work\git_folder\git_github_tut> git checkout -b "modify-libraries-used-in-etl" 
Switched to a new branch 'modify-libraries-used-in-etl'
PS C:\laur\work\git_folder\git_github_tut> git commit -m "add ploting library to etl module"
On branch modify-libraries-used-in-etl
Changes not staged for commit:
  (use "git restore <file>..." to discard changes in working directory)
        modified:   etl.ipynb

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\laur\work\git_folder\git_github_tut> git add etl.ipynb
warning: in the working copy of 'etl.ipynb', LF will be replaced by CRLF the next time Git touches it
PS C:\laur\work\git_folder\git_github_tut> git commit -m "add ploting library to etl module"
[modify-libraries-used-in-etl ae392d9] add ploting library to etl module
 1 file changed, 1 insertion(+)
PS C:\laur\work\git_folder\git_github_tut> git push
fatal: The current branch modify-libraries-used-in-etl has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin modify-libraries-used-in-etl
To have this happen automatically for branches without a tracking

PS C:\laur\work\git_folder\git_github_tut> git push --set-upstream origin modify-libraries-used-in-etl
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 406 bytes | 81.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'modify-libraries-used-in-etl' on GitHub by visiting:
remote:      https://github.com/ailacos/git_github_tut/pull/new/modify-libraries-used-in-etl
remote:
To https://github.com/ailacos/git_github_tut.git
 * [new branch]      modify-libraries-used-in-etl -> modify-libraries-used-in-etl
branch 'modify-libraries-used-in-etl' set up to track 'origin/modify-libraries-used-in-etl'.
Switched to a new branch 'add-plot-feature-in-etl'
PS C:\laur\work\git_folder\git_github_tut> git commit -m "add-math-function"
On branch add-plot-feature-in-etl
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   etl.ipynb

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\laur\work\git_folder\git_github_tut> git push
fatal: The current branch add-plot-feature-in-etl has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin add-plot-feature-in-etl

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\laur\work\git_folder\git_github_tut> git push --set-upstream origin add-plot-feature-in-etl
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'add-plot-feature-in-etl' on GitHub by visiting:
remote:      https://github.com/ailacos/git_github_tut/pull/new/add-plot-feature-in-etl
remote:
To https://github.com/ailacos/git_github_tut.git
 * [new branch]      add-plot-feature-in-etl -> add-plot-feature-in-etl
branch 'add-plot-feature-in-etl' set up to track 'origin/add-plot-feature-in-etl'.
PS C:\laur\work\git_folder\git_github_tut> 