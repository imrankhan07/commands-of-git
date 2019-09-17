# commands-of-git
Linux command
=======================================

1. present working directory---pwd
2. List of files and Folders---ls
3. clear
4. change the direcotry---cd
5. create the folder or Directory---mkdir
    mkdir<FOLDERNAME>
6. create a file under the same directory(pythonprogramming).
    a.touch:create a file
    b.nano
    c.gedit
    d.cat:used to read the file data.
    e.echo:used to write the data to file.
       1.echo 'Git Exploring' > data.txt
       2.echo 'Git learning process'>> data.txt ---used to append
 
GIT COMMAND:-
======================================

1.git version---TO check the current version in loacal computer.
2.mkdir git
3.git init---used for to create a new project.
4.showing hidden file/folder(ls -a)
  $ ls -a
./  ../  .git/  data.txt  data.txtecho  Git/
5.configure the git
5.1 git config user.name 'YourName' ----$ git config user.name 'Imrankhan'  (TO configure)
                                    ---$ git config user.name       (Test configure)                                                                                                                             Imrankhan
5.2 git config user.email 'YourEmail' (same as above)
==============================================================================================
6.6.1git status--- which will notify that the file is tracked or not.(step1-check status)
   $ git status
output:On branch master

No commits yet


Untracked files:
  (use "git add <file>..." to include in what will be committed)
        data.txt
        data.txtecho
nothing added to commit but untracked files present (use "git add" to track)
===============================================================================================
6.2 $ git add data.txt                                               (step2-ADD status)
warning: LF will be replaced by CRLF in data.txt.
The file will have its original line endings in your working directory
================================================================================================
6.3 $ git status                                                     (step3-AGAIN,check status.)
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   data.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        data.txtecho
===========================================================================
7.$ git commit -m 'First commit of Data.txt'                                                                                                                              [master (root-commit) 474d2bf] First commit of Data.txt
 1 file changed, 2 insertions(+)
 create mode 100644 data.txt
========================================================================
8.git status
========================================================================
9.nano---used to edit the file 
   $ nano data.txt  
    anything u can eidt or write then once we done
   ufhfguhgguhujhngunjbfugbgu 
   1st ctrl+X
   2nd press yes y
   3rd press enter.
==========================================================================
10.cat----used to display the content
    cat data.txt
=========================================================================
11.git status:

Imran@DESKTOP-0PU8M8J MINGW64 ~/desktop/pythonprogramming (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   data.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        data.txtecho

no changes added to commit (use "git add" and/or "git commit -a")

Imran@DESKTOP-0PU8M8J MINGW64 ~/desktop/pythonprogramming (master)
$ git add data.txt
warning: LF will be replaced by CRLF in data.txt.
The file will have its original line endings in your working directory

Imran@DESKTOP-0PU8M8J MINGW64 ~/desktop/pythonprogramming (master)
$ git commit -m 'Second commit'
[master eb72eb0] Second commit
 1 file changed, 6 insertions(+)
========================================================================
12.git log-----(To check how many time we are commiting)
$ git log
commit eb72eb04db01a71f494bc59e2acc8526641b5ee6 (HEAD -> master)
Author: Imrankhan <theikimran@gmail.com>
Date:   Tue Sep 17 11:46:23 2019 +0530

    Second commit

commit 474d2bff25e8d10d0dd758bb8597447b595e032d
Author: Imrankhan <theikimran@gmail.com>
Date:   Tue Sep 17 11:35:59 2019 +0530

    First commit of Data.txt
=======================================================================
13.$ git remote add mkdir commands-of-git https://github.com/imrankhan07/commands-of-git 
=======================================================================================
14.$ git remote show                                                                                                                                                       commands-of-git
======================================================================================
15.$ git remote -v                                                                                                                                                           commands-of-git https://github.com/imrankhan07/commands-of-git (fetch)
     commands-of-git https://github.com/imrankhan07/commands-of-git (push)
========================================================================================
16.$ git pull commands-of-git         #pull the data                                                                                                                         fatal: unable to access 'https://github.com/imrankhan07/commands-of-git/': Failed to connect to github.com port 443: Timed out
======================================================================================================================================
17.$ git push -u commands-of-git     #push the data                                                                                                                         fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream commands-of-git master
18.$ git push --set-upstream commands-of-git
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream commands-of-git master


    
      
