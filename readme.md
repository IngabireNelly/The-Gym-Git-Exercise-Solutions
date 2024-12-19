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

## Bundler 3

## Exercise 1


'''bash
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/team-page

Switched to a new branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
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
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Created team.html page"

[ft/team-page 5b138ae] Created team.html page
 1 file changed, 2 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/team-page

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 385 bytes | 385.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/contact-page

Switched to a new branch 'ft/contact-page'
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/main, origin/ft/service-redesign, main, ft/service-redesign, ft/contact-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 13:52:14 2024 +0200

    Resolved conflicts with main branch

commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
gymkwigiraii@kwigiras-iMac exercise1 % git switch ft/contact-page

fatal: cannot switch branch while rebasing
Consider "git rebase --quit" or "git worktree add".
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/contact-page

Switched to branch 'ft/contact-page'
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick git switch ft/contact-page

fatal: bad revision 'git'
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
fatal: bad revision 'commit'
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick 4599bc0a088f9334e0fc6c81f0e983bbe41068fd 
error: commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd is a merge but no -m option was given.
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick 639fb66e8412a7e6e264c737e21316b9c0b1188c
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
gymkwigiraii@kwigiras-iMac exercise1 % git log --oneline                                       

639fb66 (HEAD -> ft/contact-page, origin/main, origin/ft/service-redesign, main, ft/service-redesign) Resolved conflicts with main branch
4599bc0 Removed home.html
6b807f8 Updated service page with new service offerings
2a8b6f8 Merge pull request #6 from IngabireNelly/ft/service-redesign
eb59e72 Redesigned the service page
2a6302e saved the changes on merging
b276500 pulled the new answers from branch ft/bundle-2
b44f297 (ft/bundle-2) xi added more exercise answers to the read me file
c1eb43e Merge pull request #4 from IngabireNelly/ft/bundle-2
f3aed0e i created service html and added some staff
d7db203 the second commit.
cca8f8c added and saved some html in about
ff3e947 (origin/dev, dev) saved the unsaved html files
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                                 
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply ff3e947... saved the unsaved html files
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
gymkwigiraii@kwigiras-iMac exercise1 % git log --oneline       

639fb66 (HEAD -> ft/contact-page, origin/main, origin/ft/service-redesign, main, ft/service-redesign) Resolved conflicts with main branch
4599bc0 Removed home.html
6b807f8 Updated service page with new service offerings
2a8b6f8 Merge pull request #6 from IngabireNelly/ft/service-redesign
eb59e72 Redesigned the service page
2a6302e saved the changes on merging
b276500 pulled the new answers from branch ft/bundle-2
b44f297 (ft/bundle-2) xi added more exercise answers to the read me file
c1eb43e Merge pull request #4 from IngabireNelly/ft/bundle-2
f3aed0e i created service html and added some staff
d7db203 the second commit.
cca8f8c added and saved some html in about
ff3e947 (origin/dev, dev) saved the unsaved html files
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947 
error: Cherry-picking is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (fix conflicts and then run "git rebase --continue")
  (use "git rebase --skip" to skip this patch)
  (use "git rebase --abort" to check out the original branch)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   about.html
        both modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue

hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git merge main            
fatal: You have not concluded your cherry-pick (CHERRY_PICK_HEAD exists).
Please, commit your changes before you merge.
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue

hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git config --global core.editor "code --wait"

gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue

hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                      
error: your local changes would be overwritten by cherry-pick.
hint: commit your changes or stash them to proceed.
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

Changes to be committed:
        modified:   about.html
        modified:   readme.md

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "the contact page commit about and readme"
[ft/contact-page 4f6dfd9] the contact page commit about and readme
 Date: Thu Dec 19 12:30:47 2024 +0200
 2 files changed, 8 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                                 
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply ff3e947... saved the unsaved html files
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue
U       about.html
U       readme.md
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "the contact page commit about and readme"
[ft/contact-page 8270f3a] the contact page commit about and readme
 Date: Thu Dec 19 12:30:47 2024 +0200
 2 files changed, 7 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue                              
error: no cherry-pick or revert in progress
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                                 
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply ff3e947... saved the unsaved html files
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --skip    
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on dev: c73e0e6 Merge pull request #2 from IngabireNelly/main
stash@{1}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop 
Auto-merging team.html
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
Dropped refs/stash@{0} (a9f79b38430aab720e3a5b3edff467e042d52201)
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop
Auto-merging about.html
Auto-merging home.html
Auto-merging team.html
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
Dropped refs/stash@{0} (f46759beb823b2f12b0482c0cce4073af57dc354)
gymkwigiraii@kwigiras-iMac exercise1 % git status 
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git log                                 
commit 8270f3ad43408ffbf79daf778d9659caae0be71e (HEAD -> ft/contact-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 12:30:47 2024 +0200

    the contact page commit about and readme

commit 4f6dfd921046eeffb53f97471bb05e750dc7eda5
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 12:30:47 2024 +0200

    the contact page commit about and readme

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/main, origin/ft/service-redesign, main, ft/service-redesign)
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/main, origin/ft/service-redesign, main, ft/service-redesign)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 13:52:14 2024 +0200

    Resolved conflicts with main branch

commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/contact-page
Switched to branch 'ft/contact-page'
gymkwigiraii@kwigiras-iMac exercise1 % git sherry-pick 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
git: 'sherry-pick' is not a git command. See 'git --help'.

The most similar command is
        cherry-pick
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
[ft/contact-page cdaaa19] Created team.html page
 Date: Thu Dec 19 14:41:29 2024 +0200
 1 file changed, 2 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
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
        modified:   about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git .add
git: '.add' is not a git command. See 'git --help'.

The most similar command is
        add
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "commiting changes on contact page i just crea
ted"
[ft/contact-page ef07435] commiting changes on contact page i just created
 2 files changed, 1 deletion(-)
 create mode 100644 contact.html
gymkwigiraii@kwigiras-iMac exercise1 % git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin ft/contact-page
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 8 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (15/15), 1.66 KiB | 1.66 MiB/s, done.
Total 15 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/faq-page             

Switched to a new branch 'ft/faq-page'
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Created FAQ page"

[ft/faq-page 0de7d9c] Created FAQ page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/faq-page

Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 489 bytes | 489.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git revert 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/ft/service-redesign, main, ft/service-redesign)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 13:52:14 2024 +0200

    Resolved conflicts with main branch

commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
gymkwigiraii@kwigiras-iMac exercise1 % git revert 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added changes to faq and created it "
[ft/team-page b129151] added changes to faq and created it
 2 files changed, 12 insertions(+), 2 deletions(-)
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git revert 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d 
On branch ft/team-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit b12915183541c51d1090502c16f27c542dc5a396 (HEAD -> ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 16:33:34 2024 +0200

    added changes to faq and created it

commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/ft/service-redesign, main, ft/service-redesign)
gymkwigiraii@kwigiras-iMac exercise1 % git revert b12915183541c51d1090502c16f27c542dc5a396 
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git revert -m b12915183541c51d1090502c16f27c542dc5a396
error: option `mainline' expects a number greater than zero
gymkwigiraii@kwigiras-iMac exercise1 % git revert b12915183541c51d1090502c16f27c542dc5a396   
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "reverted the changes of the last commit"
[ft/team-page c4e5b73] reverted the changes of the last commit
 2 files changed, 2 insertions(+), 12 deletions(-)
 delete mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin ft/team-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 732 bytes | 732.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   5b138ae..c4e5b73  ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the answers of exercise 2 bundler3 to r
eadme"
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the answers of exercise 2 bundler3 to readme"
[ft/team-page bfdd4f2] added the answers of exercise 2 bundler3 to readme
 1 file changed, 541 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 3.37 KiB | 3.37 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   c4e5b73..bfdd4f2  ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git merge main
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main  
Switched to branch 'main'
Your branch is behind 'origin/main' by 6 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
gymkwigiraii@kwigiras-iMac exercise1 % git merge pull    
merge: pull - not something we can merge
gymkwigiraii@kwigiras-iMac exercise1 % git pull      
Updating 639fb66..8451d2e
Fast-forward
 about.html   |  7 +++++++
 contact.html |  0
 faq.html     | 12 ++++++++++++
 readme.md    |  8 +++++++-
 team.html    |  2 ++
 5 files changed, 28 insertions(+), 1 deletion(-)
 create mode 100644 contact.html
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git push
Everything up-to-date
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   readme.md

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the new exercise to the main branch"
[main 91e56fa] added the new exercise to the main branch
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the new exercise to the main branch"
[main 9c625ad] added the new exercise to the main branch
 2 files changed, 11 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page                                   
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git push
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 849 bytes | 849.00 KiB/s, done.
Total 7 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   8451d2e..9c625ad  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page                           
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git merge main
Updating bfdd4f2..9c625ad
Fast-forward
 about.html   |   7 +
 contact.html |  11 ++
 faq.html     |  12 ++
 readme.md    | 543 +-----------------------------------------------------------------------------
 4 files changed, 31 insertions(+), 542 deletions(-)
 create mode 100644 contact.html
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 9c625ade75584456affba18767f877cc247bbbe8 (HEAD -> ft/team-page, origin/main, main)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 16:53:40 2024 +0200

    added the new exercise to the main branch

commit 91e56faed8ec0ef0438b05a01388cabb392200bd
Merge: 8451d2e bfdd4f2
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 16:52:45 2024 +0200

    added the new exercise to the main branch

commit bfdd4f2ad8e753aa912685c8a390a32e8ce1e39f (origin/ft/team-page)
gymkwigiraii@kwigiras-iMac exercise1 % git revert bfdd4f2ad8e753aa912685c8a390a32e8ce1e39f
Auto-merging readme.md
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 8 commits.
  (use "git push" to publish your local commits)

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % 

''''


## Exercise 2


gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/team-page

Switched to a new branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
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
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Created team.html page"

[ft/team-page 5b138ae] Created team.html page
 1 file changed, 2 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/team-page

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 385 bytes | 385.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/contact-page

Switched to a new branch 'ft/contact-page'
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/main, origin/ft/service-redesign, main, ft/service-redesign, ft/contact-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 13:52:14 2024 +0200

    Resolved conflicts with main branch

commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
gymkwigiraii@kwigiras-iMac exercise1 % git switch ft/contact-page

fatal: cannot switch branch while rebasing
Consider "git rebase --quit" or "git worktree add".
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/contact-page

Switched to branch 'ft/contact-page'
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick git switch ft/contact-page

fatal: bad revision 'git'
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
fatal: bad revision 'commit'
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick 4599bc0a088f9334e0fc6c81f0e983bbe41068fd 
error: commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd is a merge but no -m option was given.
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick 639fb66e8412a7e6e264c737e21316b9c0b1188c
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
gymkwigiraii@kwigiras-iMac exercise1 % git log --oneline                                       

639fb66 (HEAD -> ft/contact-page, origin/main, origin/ft/service-redesign, main, ft/service-redesign) Resolved conflicts with main branch
4599bc0 Removed home.html
6b807f8 Updated service page with new service offerings
2a8b6f8 Merge pull request #6 from IngabireNelly/ft/service-redesign
eb59e72 Redesigned the service page
2a6302e saved the changes on merging
b276500 pulled the new answers from branch ft/bundle-2
b44f297 (ft/bundle-2) xi added more exercise answers to the read me file
c1eb43e Merge pull request #4 from IngabireNelly/ft/bundle-2
f3aed0e i created service html and added some staff
d7db203 the second commit.
cca8f8c added and saved some html in about
ff3e947 (origin/dev, dev) saved the unsaved html files
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                                 
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply ff3e947... saved the unsaved html files
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
gymkwigiraii@kwigiras-iMac exercise1 % git log --oneline       

639fb66 (HEAD -> ft/contact-page, origin/main, origin/ft/service-redesign, main, ft/service-redesign) Resolved conflicts with main branch
4599bc0 Removed home.html
6b807f8 Updated service page with new service offerings
2a8b6f8 Merge pull request #6 from IngabireNelly/ft/service-redesign
eb59e72 Redesigned the service page
2a6302e saved the changes on merging
b276500 pulled the new answers from branch ft/bundle-2
b44f297 (ft/bundle-2) xi added more exercise answers to the read me file
c1eb43e Merge pull request #4 from IngabireNelly/ft/bundle-2
f3aed0e i created service html and added some staff
d7db203 the second commit.
cca8f8c added and saved some html in about
ff3e947 (origin/dev, dev) saved the unsaved html files
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947 
error: Cherry-picking is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (fix conflicts and then run "git rebase --continue")
  (use "git rebase --skip" to skip this patch)
  (use "git rebase --abort" to check out the original branch)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   about.html
        both modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue

hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git merge main            
fatal: You have not concluded your cherry-pick (CHERRY_PICK_HEAD exists).
Please, commit your changes before you merge.
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue

hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git config --global core.editor "code --wait"

gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue

hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                      
error: your local changes would be overwritten by cherry-pick.
hint: commit your changes or stash them to proceed.
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

Changes to be committed:
        modified:   about.html
        modified:   readme.md

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "the contact page commit about and readme"
[ft/contact-page 4f6dfd9] the contact page commit about and readme
 Date: Thu Dec 19 12:30:47 2024 +0200
 2 files changed, 8 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                                 
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply ff3e947... saved the unsaved html files
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue
U       about.html
U       readme.md
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "the contact page commit about and readme"
[ft/contact-page 8270f3a] the contact page commit about and readme
 Date: Thu Dec 19 12:30:47 2024 +0200
 2 files changed, 7 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --continue                              
error: no cherry-pick or revert in progress
fatal: cherry-pick failed
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick ff3e947                                 
Auto-merging about.html
CONFLICT (content): Merge conflict in about.html
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply ff3e947... saved the unsaved html files
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick --skip    
gymkwigiraii@kwigiras-iMac exercise1 % git stash list
stash@{0}: WIP on dev: c73e0e6 Merge pull request #2 from IngabireNelly/main
stash@{1}: WIP on dev: 0c7bc84 Removed home.html
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop 
Auto-merging team.html
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
Dropped refs/stash@{0} (a9f79b38430aab720e3a5b3edff467e042d52201)
gymkwigiraii@kwigiras-iMac exercise1 % git stash pop
Auto-merging about.html
Auto-merging home.html
Auto-merging team.html
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
Dropped refs/stash@{0} (f46759beb823b2f12b0482c0cce4073af57dc354)
gymkwigiraii@kwigiras-iMac exercise1 % git status 
On branch ft/contact-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git log                                 
commit 8270f3ad43408ffbf79daf778d9659caae0be71e (HEAD -> ft/contact-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 12:30:47 2024 +0200

    the contact page commit about and readme

commit 4f6dfd921046eeffb53f97471bb05e750dc7eda5
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 12:30:47 2024 +0200

    the contact page commit about and readme

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/main, origin/ft/service-redesign, main, ft/service-redesign)
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/main, origin/ft/service-redesign, main, ft/service-redesign)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 13:52:14 2024 +0200

    Resolved conflicts with main branch

commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/contact-page
Switched to branch 'ft/contact-page'
gymkwigiraii@kwigiras-iMac exercise1 % git sherry-pick 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
git: 'sherry-pick' is not a git command. See 'git --help'.

The most similar command is
        cherry-pick
gymkwigiraii@kwigiras-iMac exercise1 % git cherry-pick 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
[ft/contact-page cdaaa19] Created team.html page
 Date: Thu Dec 19 14:41:29 2024 +0200
 1 file changed, 2 insertions(+)
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
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
        modified:   about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git .add
git: '.add' is not a git command. See 'git --help'.

The most similar command is
        add
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "commiting changes on contact page i just crea
ted"
[ft/contact-page ef07435] commiting changes on contact page i just created
 2 files changed, 1 deletion(-)
 create mode 100644 contact.html
gymkwigiraii@kwigiras-iMac exercise1 % git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin ft/contact-page
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 8 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (15/15), 1.66 KiB | 1.66 MiB/s, done.
Total 15 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/faq-page             

Switched to a new branch 'ft/faq-page'
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Created FAQ page"

[ft/faq-page 0de7d9c] Created FAQ page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/faq-page

Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 489 bytes | 489.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
gymkwigiraii@kwigiras-iMac exercise1 % git revert 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (HEAD -> ft/team-page, origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/ft/service-redesign, main, ft/service-redesign)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 13:52:14 2024 +0200

    Resolved conflicts with main branch

commit 4599bc0a088f9334e0fc6c81f0e983bbe41068fd
gymkwigiraii@kwigiras-iMac exercise1 % git revert 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added changes to faq and created it "
[ft/team-page b129151] added changes to faq and created it
 2 files changed, 12 insertions(+), 2 deletions(-)
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git revert 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d 
On branch ft/team-page
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit b12915183541c51d1090502c16f27c542dc5a396 (HEAD -> ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 16:33:34 2024 +0200

    added changes to faq and created it

commit 5b138ae3d750f5b344e4f473bb9c24cab0f5d39d (origin/ft/team-page)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 14:41:29 2024 +0200

    Created team.html page

commit 639fb66e8412a7e6e264c737e21316b9c0b1188c (origin/ft/service-redesign, main, ft/service-redesign)
gymkwigiraii@kwigiras-iMac exercise1 % git revert b12915183541c51d1090502c16f27c542dc5a396 
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git revert -m b12915183541c51d1090502c16f27c542dc5a396
error: option `mainline' expects a number greater than zero
gymkwigiraii@kwigiras-iMac exercise1 % git revert b12915183541c51d1090502c16f27c542dc5a396   
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit
hint: Waiting for your editor to close the file... code --wait: code: command not found
error: There was a problem with the editor 'code --wait'.
Please supply the message using either -m or -F option.
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "reverted the changes of the last commit"
[ft/team-page c4e5b73] reverted the changes of the last commit
 2 files changed, 2 insertions(+), 12 deletions(-)
 delete mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin ft/team-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 732 bytes | 732.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   5b138ae..c4e5b73  ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the answers of exercise 2 bundler3 to r
eadme"
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the answers of exercise 2 bundler3 to readme"
[ft/team-page bfdd4f2] added the answers of exercise 2 bundler3 to readme
 1 file changed, 541 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 3.37 KiB | 3.37 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   c4e5b73..bfdd4f2  ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git merge main
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main  
Switched to branch 'main'
Your branch is behind 'origin/main' by 6 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
gymkwigiraii@kwigiras-iMac exercise1 % git merge pull    
merge: pull - not something we can merge
gymkwigiraii@kwigiras-iMac exercise1 % git pull      
Updating 639fb66..8451d2e
Fast-forward
 about.html   |  7 +++++++
 contact.html |  0
 faq.html     | 12 ++++++++++++
 readme.md    |  8 +++++++-
 team.html    |  2 ++
 5 files changed, 28 insertions(+), 1 deletion(-)
 create mode 100644 contact.html
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git push
Everything up-to-date
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   readme.md

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the new exercise to the main branch"
[main 91e56fa] added the new exercise to the main branch
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "added the new exercise to the main branch"
[main 9c625ad] added the new exercise to the main branch
 2 files changed, 11 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page                                   
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git push
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 849 bytes | 849.00 KiB/s, done.
Total 7 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   8451d2e..9c625ad  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page                           
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git merge main
Updating bfdd4f2..9c625ad
Fast-forward
 about.html   |   7 +
 contact.html |  11 ++
 faq.html     |  12 ++
 readme.md    | 543 +-----------------------------------------------------------------------------
 4 files changed, 31 insertions(+), 542 deletions(-)
 create mode 100644 contact.html
 create mode 100644 faq.html
gymkwigiraii@kwigiras-iMac exercise1 % git log
commit 9c625ade75584456affba18767f877cc247bbbe8 (HEAD -> ft/team-page, origin/main, main)
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 16:53:40 2024 +0200

    added the new exercise to the main branch

commit 91e56faed8ec0ef0438b05a01388cabb392200bd
Merge: 8451d2e bfdd4f2
Author: Ingabire Nelly <ingabirenelly72@gmail.com>
Date:   Thu Dec 19 16:52:45 2024 +0200

    added the new exercise to the main branch

commit bfdd4f2ad8e753aa912685c8a390a32e8ce1e39f (origin/ft/team-page)
gymkwigiraii@kwigiras-iMac exercise1 % git revert bfdd4f2ad8e753aa912685c8a390a32e8ce1e39f
Auto-merging readme.md
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 8 commits.
  (use "git push" to publish your local commits)

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently rebasing branch 'dev' on '66295ed'.
  (all conflicts fixed: run "git rebase --continue")

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit m- "committed again the last commit "
error: pathspec 'm-' did not match any file(s) known to git
error: pathspec 'committed again the last commit ' did not match any file(s) known to git
gymkwigiraii@kwigiras-iMac exercise1 % git commit m-  "committed again the last commit "
error: pathspec 'm-' did not match any file(s) known to git
error: pathspec 'committed again the last commit ' did not match any file(s) known to git
gymkwigiraii@kwigiras-iMac exercise1 % git add .                                        
gymkwigiraii@kwigiras-iMac exercise1 % git commit m-  "committed again the last commit "
error: pathspec 'm-' did not match any file(s) known to git
error: pathspec 'committed again the last commit ' did not match any file(s) known to git
gymkwigiraii@kwigiras-iMac exercise1 % git add .                                        
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m
error: switch `m' requires a value
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 9 commits.
  (use "git push" to publish your local commits)

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 6.52 KiB | 6.52 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   bfdd4f2..9b0deaa  ft/team-page -> ft/team-page
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

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
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git merge ft/team-page
Updating 9c625ad..9b0deaa
Fast-forward
 readme.md | 684 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 1 file changed, 683 insertions(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git pull
Already up to date.
gymkwigiraii@kwigiras-iMac exercise1 % git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   9c625ad..9b0deaa  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % git push origin main        
Everything up-to-date
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/team-page

Everything up-to-date
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/faq-page
Switched to branch 'ft/faq-page'
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/home-page-redesign

Switched to a new branch 'ft/home-page-redesign'
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main                    
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Made updates to main branch"
On branch main
Your branch is up to date with 'origin/main'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git add .                                  
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % 
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git add . 
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Made updates to main branch"
[main aa83b8f] Made updates to main branch
 1 file changed, 1 insertion(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin main

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 305 bytes | 305.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   9b0deaa..aa83b8f  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % git checkout ft/home-page-redesign   
Switched to branch 'ft/home-page-redesign'
gymkwigiraii@kwigiras-iMac exercise1 % git rebase main

fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.

gymkwigiraii@kwigiras-iMac exercise1 % rm -fr ".git/rebase-merge 
dquote> 
gymkwigiraii@kwigiras-iMac exercise1 % git rebase main          

fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.

gymkwigiraii@kwigiras-iMac exercise1 % git status

On branch ft/home-page-redesign
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git rebase --continue

error: update_ref failed for ref 'refs/heads/dev': cannot lock ref 'refs/heads/dev': is at ff3e947eff441487026a7b55de424579434d759c but expected 0c7bc845d3af87ca45cff2a53675b7b2e38d3d28
error: could not update refs/heads/dev
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/home-page-redesign
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git rebase --continue

error: update_ref failed for ref 'refs/heads/dev': cannot lock ref 'refs/heads/dev': is at ff3e947eff441487026a7b55de424579434d759c but expected 0c7bc845d3af87ca45cff2a53675b7b2e38d3d28
error: could not update refs/heads/dev
gymkwigiraii@kwigiras-iMac exercise1 % git status           
On branch ft/home-page-redesign
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/home-page-redesign --force

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
gymkwigiraii@kwigiras-iMac exercise1 % 

''''

## Bundler 4

## Exercise 1


'''bash
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main

Already on 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git remote add git-copy https://github.com/IngabireNelly/THE-GYM-Exercises-copy
gymkwigiraii@kwigiras-iMac exercise1 % git remote -v

git-copy        https://github.com/IngabireNelly/THE-GYM-Exercises-copy (fetch)
git-copy        https://github.com/IngabireNelly/THE-GYM-Exercises-copy (push)
origin  https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git (push)
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch main
Your branch is up to date with 'origin/main'.

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
        modified:   faq.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "Updated home page"
[main fe850e8] Updated home page
 1 file changed, 1 insertion(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin main

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 320 bytes | 320.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
   7bccf49..fe850e8  main -> main
gymkwigiraii@kwigiras-iMac exercise1 % git push git-copy main

Enumerating objects: 101, done.
Counting objects: 100% (101/101), done.
Delta compression using up to 8 threads
Compressing objects: 100% (95/95), done.
Writing objects: 100% (101/101), 21.85 KiB | 7.28 MiB/s, done.
Total 101 (delta 45), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (45/45), done.
To https://github.com/IngabireNelly/THE-GYM-Exercises-copy
 * [new branch]      main -> main
gymkwigiraii@kwigiras-iMac exercise1 % 

'''


## Exercise 2



'''bash
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/footer
Switched to a new branch 'ft/footer'
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/footer
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
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "made some changes on team html"
[ft/footer e9b8ede] made some changes on team html
 1 file changed, 1 insertion(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git status                                    
On branch ft/footer
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
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "made some changes on services html"
[ft/footer 48b0fcc] made some changes on services html
 1 file changed, 1 insertion(+), 1 deletion(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/footer

Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 658 bytes | 658.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
gymkwigiraii@kwigiras-iMac exercise1 % git checkout main

Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymkwigiraii@kwigiras-iMac exercise1 % git checkout -b ft/squashing

Switched to a new branch 'ft/squashing'
gymkwigiraii@kwigiras-iMac exercise1 % git merge --squash ft/footer
Updating 2915c64..48b0fcc
Fast-forward
Squash commit -- not updating HEAD
 services.html | 2 +-
 team.html     | 2 +-
 2 files changed, 2 insertions(+), 2 deletions(-)
gymkwigiraii@kwigiras-iMac exercise1 % git status
On branch ft/squashing
Last commands done (2 commands done):
   pick f47f316 the second commit.
   pick 0c7bc84 Removed home.html
No commands remaining.
You are currently editing a commit while rebasing branch 'dev' on '66295ed'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html
        modified:   team.html

gymkwigiraii@kwigiras-iMac exercise1 % git add .
gymkwigiraii@kwigiras-iMac exercise1 % git commit -m "footer changes squashing"

[ft/squashing e48e4f4] footer changes squashing
 2 files changed, 2 insertions(+), 2 deletions(-)
gymkwigiraii@kwigiras-iMac exercise1 % git push origin ft/squashing

Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 423 bytes | 423.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote: 
To https://github.com/IngabireNelly/The-Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
gymkwigiraii@kwigiras-iMac exercise1 % 

'''