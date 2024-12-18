# Git exercise 


## Bundle 1


## Exercises 1

'''bash
gymkwigiraii@kwigiras-iMac exercise1 % git init
Initialized empty Git repository in /Users/gymkwigiraii/exercise1/.git/
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git branch
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "initial commit"
[main (root-commit) 3ac5c55] initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 readme.md
gymkwigiraii@kwigiras-iMac exercise1 % git branch -m main master 
gymkwigiraii@kwigiras-iMac exercise1 % git status                
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git branch -m main        
gymkwigiraii@kwigiras-iMac exercise1 % git add .  
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   readme.md

gymkwigiraii@kwigiras-iMac exercise1 % git commit
[main 66295ed] the first commit.
 1 file changed, 3 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git remote add origin https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
gymkwigiraii@kwigiras-iMac exercise1 % git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 479 bytes | 479.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b dev
Switched to a new branch 'dev'
gymkwigiraii@kwigiras-iMac exercise1 % git staus
git: 'staus' is not a git command. See 'git --help'.

The most similar command is
        status
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch dev
nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/dev
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b test              
Switched to a new branch 'test'
gymkwigiraii@kwigiras-iMac exercise1 % git push                          
fatal: The current branch test has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin test

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/test
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
branch 'test' set up to track 'origin/test'.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout dev                   
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.
gymkwigiraii@kwigiras-iMac exercise1 % git branch -D test
Deleted branch test (was 66295ed).
gymkwigiraii@kwigiras-iMac exercise1 % git push orign --delete test
fatal: 'orign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main           
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git push orign --delete test
fatal: 'orign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout dev            
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.
gymkwigiraii@kwigiras-iMac exercise1 % git push orign --delete test
fatal: 'orign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
gymkwigiraii@kwigiras-iMac exercise1 % git branch -r               
  origin/dev
  origin/main
  origin/test
gymkwigiraii@kwigiras-iMac exercise1 % git branch -a
* dev
  main
  remotes/origin/dev
  remotes/origin/main
  remotes/origin/test
gymkwigiraii@kwigiras-iMac exercise1 % git push origin --delete test

To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 - [deleted]         test
gymkwigiraii@kwigiras-iMac exercise1 % 

'''


## Exercise 2

