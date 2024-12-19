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

gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git add home.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash
Saved working directory and index state WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{1}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git add about.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash
Saved working directory and index state WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
gymkwigiraii@kwigiras-iMac exercise1 % git status 
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git stash
Saved working directory and index state WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{1}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{2}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{3}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (fb76fb8cb6a1e1555b1a41827bc8bfbc2da44b92)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git stash
Saved working directory and index state WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{1}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{2}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{3}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{2} (71453b708ff71c12a22b41118e2ea9f1f2724e44)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

gymkwigiraii@kwigiras-iMac exercise1 % git add home.html
gymkwigiraii@kwigiras-iMac exercise1 % git commit
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git stash        
Saved working directory and index state WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped refs/stash@{0} (45f1e24ec7a4bf29923fce52e8bdf59e593e2bc1)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit 
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "home commit"
[main 584b4d1] home commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 home.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{1}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{2}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop stash@{1}
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (3fdb8fb0c3ce4d7a2447e6a1b68f767c2f1a8e3b)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "about was commit" 
[main d65ae45] about was commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 about.html
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Last command done (1 command done):
   pick f47f316 the second commit.
Next command to do (1 remaining command):
   pick 0c7bc84 Removed home.html
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{1}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git add .                       
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "team was commit"
[main 52e9ec4] team was commit
 1 file changed, 9 insertions(+)
 create mode 100644 team.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash list                  
stash@{0}: WIP on main: 208b4da Merge pull request #1 from IngabireNelly/dev
stash@{1}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git push      
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (8/8), 855 bytes | 855.00 KiB/s, done.
Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   208b4da..52e9ec4  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % git checkout dev
Switched to branch 'dev'
Your branch is behind 'origin/dev' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
gymkwigiraii@kwigiras-iMac exercise1 % git pull
Updating c5111cc..c73e0e6
Fast-forward
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % 

## Bundler 2


## Exercise 1

'''bash
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/bundle-2
Already on 'ft/bundle-2'
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/bundle-2
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "i created service html and added some staff"
[ft/bundle-2 f3aed0e] i created service html and added some staff
 1 file changed, 9 insertions(+)
 create mode 100644 services.html
gymkwigiraii@kwigiras-iMac exercise1 % git merge main
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/bundle-2

Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 422 bytes | 422.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
gymkwigiraii@kwigiras-iMac exercise1 % 

''''

## Exercise 2

'''bash

gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/service-redesign                      

Switched to a new branch 'ft/service-redesign'
gymkwigiraii@kwigiras-iMac exercise1 % git add service.html

fatal: pathspec 'service.html' did not match any files
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/service-redesign
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Redesigned the service page"

[ft/service-redesign eb59e72] Redesigned the service page
 1 file changed, 1 insertion(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/service-redesign

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 361.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/service-redesign
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Updated service page with new service offerings"
[main 6b807f8] Updated service page with new service offerings
 1 file changed, 2 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin main
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
gymkwigiraii@kwigiras-iMac exercise1 % git pull
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
gymkwigiraii@kwigiras-iMac exercise1 % git pull
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 578 bytes | 578.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   2a8b6f8..4599bc0  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % 