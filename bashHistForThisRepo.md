yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder$ mkdir repo2
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder$ cd repo2
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ touch .gitignore
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ echo "*.txt" > .gitignore
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls -a
.  ..  .gitignore
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ cat .gitignore 
*.txt
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ echo "What should we have in readme, add welcome message." > README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ echo "# WELCOME TO TEST REPO > This repo will be deleted. [] bye!" > README.MD
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ LS
LS: command not found
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git sta
stage    stash    status   
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git sta
stage    stash    status   
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   ../Project-Yrke-Akademi-YH-AV24TR
	new file:   ../README.txt
	new file:   ../YhAkademinExercises

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   ../Project-Yrke-Akademi-YH-AV24TR (new commits)
	modified:   ../YhAkademinExercises (new commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	../repo/
	./

yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit -m "Initial commit"
[main (root-commit) 9e6000a] Initial commit
 3 files changed, 3 insertions(+)
 create mode 160000 Project-Yrke-Akademi-YH-AV24TR
 create mode 100644 README.txt
 create mode 160000 YhAkademinExercises
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git remote add origin git@github.com:Yaq8bi/secondRepoForTest.git
error: remote origin already exists.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git remote add git@github.com:Yaq8bi/secondRepoForTest.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch main
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   ../Project-Yrke-Akademi-YH-AV24TR (new commits)
	modified:   ../YhAkademinExercises (new commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	../repo/
	./

no changes added to commit (use "git add" and/or "git commit -a")
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin master
error: src refspec master does not match any
error: failed to push some refs to 'https://github.com/Yaq8bi/YhAkademinExercises.git'
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin main
Username for 'https://github.com': Yaq8bi
Password for 'https://Yaq8bi@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/Yaq8bi/YhAkademinExercises.git/'
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git remote add git@github.com:Yaq8bi/secondRepoForTest.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git remote add origin git@github.com:Yaq8bi/secondRepoForTest.git
error: remote origin already exists.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin master
error: src refspec master does not match any
error: failed to push some refs to 'https://github.com/Yaq8bi/YhAkademinExercises.git'
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin main
Username for 'https://github.com': ^C
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /home/yaq8bi/Documents/myprojects/myGithubFolder/repo2/.git/
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git remote add origin git@github.com:Yaq8bi/secondRepoForTest.git
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'github.com:Yaq8bi/secondRepoForTest.git'
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin master
error: src refspec master does not match any
error: failed to push some refs to 'github.com:Yaq8bi/secondRepoForTest.git'
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git branch 
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git branch -a
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git stat
git: 'stat' is not a git command. See 'git --help'.

The most similar commands are
	status
	stage
	stash
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.gitignore
	README.MD
	README.TXT

nothing added to commit but untracked files present (use "git add" to track)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
fatal: your current branch 'master' does not have any commits yet
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit -m "Initial commit"
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.gitignore
	README.MD
	README.TXT

nothing added to commit but untracked files present (use "git add" to track)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git add .
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit -m "Initial commit"
[master (root-commit) 88c66a8] Initial commit
 3 files changed, 3 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.MD
 create mode 100644 README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin master 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 413 bytes | 413.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:Yaq8bi/secondRepoForTest.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git checkout -b develop
Switched to a new branch 'develop'
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push -u origin develop 
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'develop' on GitHub by visiting:
remote:      https://github.com/Yaq8bi/secondRepoForTest/pull/new/develop
remote: 
To github.com:Yaq8bi/secondRepoForTest.git
 * [new branch]      develop -> develop
Branch 'develop' set up to track remote branch 'develop' from 'origin'.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch develop
Your branch is up to date with 'origin/develop'.

nothing to commit, working tree clean
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
88c66a8 (HEAD -> develop, origin/master, origin/develop, master) HEAD@{0}: checkout: moving from master to develop
88c66a8 (HEAD -> develop, origin/master, origin/develop, master) HEAD@{1}: commit (initial): Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git branch 
* develop
  master
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ touch main.c; git add main.c
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch develop
Your branch is up to date with 'origin/develop'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   main.c

yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit -m "second commit, main.c created"
[develop a4d7408] second commit, main.c created
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 main.c
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit --amend -m "Added source file, main.c, this is an ammend to change the second commits msg"
[develop 8383590] Added source file, main.c, this is an ammend to change the second commits msg
 Date: Sat Oct 19 13:51:04 2024 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 main.c
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git pull origin develop 
From github.com:Yaq8bi/secondRepoForTest
 * branch            develop    -> FETCH_HEAD
Already up to date.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch develop
Your branch is ahead of 'origin/develop' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin develop 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 314 bytes | 314.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Yaq8bi/secondRepoForTest.git
   88c66a8..8383590  develop -> develop
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git log --oneline
8383590 (HEAD -> develop, origin/develop) Added source file, main.c, this is an ammend to change the second commits msg
88c66a8 (origin/master, master) Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git merge develop 
Updating 88c66a8..8383590
Fast-forward
 main.c | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 main.c
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag latestMergeFromDevToMas
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git branch 
  develop
* master
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git branch -d develop 
Deleted branch develop (was 8383590).
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin --delete develop
To github.com:Yaq8bi/secondRepoForTest.git
 - [deleted]         develop
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin master --tags
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 314 bytes | 314.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Yaq8bi/secondRepoForTest.git
   88c66a8..8383590  master -> master
 * [new tag]         latestMergeFromDevToMas -> latestMergeFromDevToMas
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push
Everything up-to-date
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git branch 
* master
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls -a
.  ..  .git  .gitignore  main.c  README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ touch theREADMEfromTheStep15.md
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git add theREADMEfromTheStep15.md 
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit -m "the Readme from step 15"
[master 41702bb] the Readme from step 15
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 theREADMEfromTheStep15.md
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag
latestMergeFromDevToMas
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -d latestMergeFromDevToMas
Deleted tag 'latestMergeFromDevToMas' (was 8383590)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -a latestReadMeQ15 -m "latestREADME.MD for Q15"
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag
latestReadMeQ15
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -a
usage: git tag [-a | -s | -u <key-id>] [-f] [-m <msg> | -F <file>]
               <tagname> [<head>]
   or: git tag -d <tagname>...
   or: git tag -l [-n[<num>]] [--contains <commit>] [--no-contains <commit>] [--points-at <object>]
               [--format=<format>] [--merged <commit>] [--no-merged <commit>] [<pattern>...]
   or: git tag -v [--format=<format>] <tagname>...

    -l, --list            list tag names
    -n[<n>]               print <n> lines of each tag message
    -d, --delete          delete tags
    -v, --verify          verify tags

Tag creation options
    -a, --annotate        annotated tag, needs a message
    -m, --message <message>
                          tag message
    -F, --file <file>     read message from file
    -e, --edit            force edit of tag message
    -s, --sign            annotated and GPG-signed tag
    --cleanup <mode>      how to strip spaces and #comments from message
    -u, --local-user <key-id>
                          use another key to sign the tag
    -f, --force           replace the tag if exists
    --create-reflog       create a reflog

Tag listing options
    --column[=<style>]    show tag list in columns
    --contains <commit>   print only tags that contain the commit
    --no-contains <commit>
                          print only tags that don't contain the commit
    --merged <commit>     print only tags that are merged
    --no-merged <commit>  print only tags that are not merged
    --sort <key>          field name to sort on
    --points-at <object>  print only tags of the object
    --format <format>     format to use for the output
    --color[=<when>]      respect format colors
    -i, --ignore-case     sorting and filtering are case insensitive

yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 288 bytes | 288.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Yaq8bi/secondRepoForTest.git
   8383590..41702bb  master -> master
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin --tags --force
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 181 bytes | 181.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:Yaq8bi/secondRepoForTest.git
 * [new tag]         latestReadMeQ15 -> latestReadMeQ15
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git log --oneline 
41702bb (HEAD -> master, tag: latestReadMeQ15, origin/master) the Readme from step 15
8383590 Added source file, main.c, this is an ammend to change the second commits msg
88c66a8 Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
41702bb (HEAD -> master, tag: latestReadMeQ15, origin/master) HEAD@{0}: commit: the Readme from step 15
8383590 HEAD@{1}: merge develop: Fast-forward
88c66a8 HEAD@{2}: checkout: moving from develop to master
8383590 HEAD@{3}: commit (amend): Added source file, main.c, this is an ammend to change the second commits msg
a4d7408 HEAD@{4}: commit: second commit, main.c created
88c66a8 HEAD@{5}: checkout: moving from master to develop
88c66a8 HEAD@{6}: commit (initial): Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git checkout 8383590
Note: switching to '8383590'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 8383590 Added source file, main.c, this is an ammend to change the second commits msg
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git commit --amend -m "Added Main.c as on Q17"
[detached HEAD e0557c0] Added Main.c as on Q17
 Date: Sat Oct 19 13:51:04 2024 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 main.c
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git status 
HEAD detached from 8383590
nothing to commit, working tree clean
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git checkout master 
Warning: you are leaving 1 commit behind, not connected to
any of your branches:

  e0557c0 Added Main.c as on Q17

If you want to keep it by creating a new branch, this may be a good time
to do so with:

 git branch <new-branch-name> e0557c0

Switched to branch 'master'
Your branch is up to date with 'origin/master'.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT  theREADMEfromTheStep15.md
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --on
fatal: unrecognized argument: --on
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
41702bb (HEAD -> master, tag: latestReadMeQ15, origin/master) HEAD@{0}: checkout: moving from e0557c0816b83ceb3ca9bdcd1a0b1a5183fcad9a to master
e0557c0 HEAD@{1}: commit (amend): Added Main.c as on Q17
8383590 HEAD@{2}: checkout: moving from master to 8383590
41702bb (HEAD -> master, tag: latestReadMeQ15, origin/master) HEAD@{3}: commit: the Readme from step 15
8383590 HEAD@{4}: merge develop: Fast-forward
88c66a8 HEAD@{5}: checkout: moving from develop to master
8383590 HEAD@{6}: commit (amend): Added source file, main.c, this is an ammend to change the second commits msg
a4d7408 HEAD@{7}: commit: second commit, main.c created
88c66a8 HEAD@{8}: checkout: moving from master to develop
88c66a8 HEAD@{9}: commit (initial): Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push --force
Everything up-to-date
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag
latestReadMeQ15
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -d latestReadMeQ15 
Deleted tag 'latestReadMeQ15' (was b31a78c)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -a latestQ18 -m "Main.cExists"
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin --tags --force
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 172 bytes | 172.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:Yaq8bi/secondRepoForTest.git
 * [new tag]         latestQ18 -> latestQ18
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
41702bb (HEAD -> master, tag: latestQ18, origin/master) HEAD@{0}: checkout: moving from e0557c0816b83ceb3ca9bdcd1a0b1a5183fcad9a to master
e0557c0 HEAD@{1}: commit (amend): Added Main.c as on Q17
8383590 HEAD@{2}: checkout: moving from master to 8383590
41702bb (HEAD -> master, tag: latestQ18, origin/master) HEAD@{3}: commit: the Readme from step 15
8383590 HEAD@{4}: merge develop: Fast-forward
88c66a8 HEAD@{5}: checkout: moving from develop to master
8383590 HEAD@{6}: commit (amend): Added source file, main.c, this is an ammend to change the second commits msg
a4d7408 HEAD@{7}: commit: second commit, main.c created
88c66a8 HEAD@{8}: checkout: moving from master to develop
88c66a8 HEAD@{9}: commit (initial): Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git rebase -i a4d7408
warning: skipped previously applied commit 8383590
hint: use --reapply-cherry-picks to include skipped commits
hint: Disable this message with "git config advice.skippedCherryPicks false"
Successfully rebased and updated refs/heads/master.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
2ef89cd (HEAD -> master) HEAD@{0}: rebase (finish): returning to refs/heads/master
2ef89cd (HEAD -> master) HEAD@{1}: rebase (pick): the Readme from step 15
a4d7408 HEAD@{2}: rebase (start): checkout a4d7408
41702bb (tag: latestQ18, origin/master) HEAD@{3}: checkout: moving from e0557c0816b83ceb3ca9bdcd1a0b1a5183fcad9a to master
e0557c0 HEAD@{4}: commit (amend): Added Main.c as on Q17
8383590 HEAD@{5}: checkout: moving from master to 8383590
41702bb (tag: latestQ18, origin/master) HEAD@{6}: commit: the Readme from step 15
8383590 HEAD@{7}: merge develop: Fast-forward
88c66a8 HEAD@{8}: checkout: moving from develop to master
8383590 HEAD@{9}: commit (amend): Added source file, main.c, this is an ammend to change the second commits msg
a4d7408 HEAD@{10}: commit: second commit, main.c created
88c66a8 HEAD@{11}: checkout: moving from master to develop
88c66a8 HEAD@{12}: commit (initial): Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
main.c  README.MD  README.TXT  theREADMEfromTheStep15.md
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git rebase -i 88c66a8
Successfully rebased and updated refs/heads/master.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
README.MD  README.TXT  theREADMEfromTheStep15.md
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git reflog --oneline
9d7160f (HEAD -> master) HEAD@{0}: rebase (finish): returning to refs/heads/master
9d7160f (HEAD -> master) HEAD@{1}: rebase (pick): the Readme from step 15
88c66a8 HEAD@{2}: rebase (start): checkout 88c66a8
2ef89cd HEAD@{3}: rebase (finish): returning to refs/heads/master
2ef89cd HEAD@{4}: rebase (pick): the Readme from step 15
a4d7408 HEAD@{5}: rebase (start): checkout a4d7408
41702bb (tag: latestQ18, origin/master) HEAD@{6}: checkout: moving from e0557c0816b83ceb3ca9bdcd1a0b1a5183fcad9a to master
e0557c0 HEAD@{7}: commit (amend): Added Main.c as on Q17
8383590 HEAD@{8}: checkout: moving from master to 8383590
41702bb (tag: latestQ18, origin/master) HEAD@{9}: commit: the Readme from step 15
8383590 HEAD@{10}: merge develop: Fast-forward
88c66a8 HEAD@{11}: checkout: moving from develop to master
8383590 HEAD@{12}: commit (amend): Added source file, main.c, this is an ammend to change the second commits msg
a4d7408 HEAD@{13}: commit: second commit, main.c created
88c66a8 HEAD@{14}: checkout: moving from master to develop
88c66a8 HEAD@{15}: commit (initial): Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git log --oneline 
9d7160f (HEAD -> master) the Readme from step 15
88c66a8 Initial commit
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin 
FETCH_HEAD      HEAD            latestQ18       master          ORIG_HEAD       origin/master 
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin master 
To github.com:Yaq8bi/secondRepoForTest.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'github.com:Yaq8bi/secondRepoForTest.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git checkout master 
Already on 'master'
Your branch and 'origin/master' have diverged,
and have 1 and 2 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ ls
README.MD  README.TXT  theREADMEfromTheStep15.md
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push --force
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Yaq8bi/secondRepoForTest.git
 + 41702bb...9d7160f master -> master (forced update)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -d latestQ18 
Deleted tag 'latestQ18' (was c7f1c9f)
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git tag -a latestQ20 -m "Last Q20 tag"
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ git push origin --tags --force
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 168 bytes | 168.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:Yaq8bi/secondRepoForTest.git
 * [new tag]         latestQ20 -> latestQ20
yaq8bi@yaq8bisLaptop:~/Documents/myprojects/myGithubFolder/repo2$ 


