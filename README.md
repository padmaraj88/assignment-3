# assignment-3
ubuntu@ip-172-31-17-0:~$ ls
ubuntu@ip-172-31-17-0:~$ whoami
ubuntu
ubuntu@ip-172-31-17-0:~$ mkdir assignment3
ubuntu@ip-172-31-17-0:~$ cd assignment3
ubuntu@ip-172-31-17-0:~/assignment3$ git init
Initialized empty Git repository in /home/ubuntu/assignment3/.git/
ubuntu@ip-172-31-17-0:~/assignment3$ touch master.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git add master.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git commit --m "master"
[master (root-commit) e5111f5] master
 Committer: Ubuntu <ubuntu@ip-172-31-17-0.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 master.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git branch
* master
ubuntu@ip-172-31-17-0:~/assignment3$ git branch devlop
ubuntu@ip-172-31-17-0:~/assignment3$ git branch f1
ubuntu@ip-172-31-17-0:~/assignment3$ git branch f2
ubuntu@ip-172-31-17-0:~/assignment3$ git branch
  devlop
  f1
  f2
* master
ubuntu@ip-172-31-17-0:~/assignment3$ git checkout devlop
Switched to branch 'devlop'
ubuntu@ip-172-31-17-0:~/assignment3$ touch devlop.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git add devlop.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git commit --m "devlop"
[devlop 01d5e59] devlop
 Committer: Ubuntu <ubuntu@ip-172-31-17-0.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 devlop.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git checkout f1
Switched to branch 'f1'
ubuntu@ip-172-31-17-0:~/assignment3$ touch f1.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git add f1.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git commit --m "f1"
[f1 bff7210] f1
 Committer: Ubuntu <ubuntu@ip-172-31-17-0.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 f1.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git checkout f2
Switched to branch 'f2'
ubuntu@ip-172-31-17-0:~/assignment3$ touch f2.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git add f2.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git commit --m "f2"
[f2 2a71ee7] f2
 Committer: Ubuntu <ubuntu@ip-172-31-17-0.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 f2.txt
ubuntu@ip-172-31-17-0:~/assignment3$ git checkout master
Switched to branch 'master'
ubuntu@ip-172-31-17-0:~/assignment3$ git branch
  devlop
  f1
  f2
* master
ubuntu@ip-172-31-17-0:~/assignment3$ git remote add orgin https://github.com/padmaraj88/assignment-3.git
ubuntu@ip-172-31-17-0:~/assignment3$ git push --all
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>

ubuntu@ip-172-31-17-0:~/assignment3$ git remote add origin https://github.com/padmaraj88/assignment-3.git
ubuntu@ip-172-31-17-0:~/assignment3$ git push --all
Username for 'https://github.com': padmaraj88
Password for 'https://padmaraj88@github.com':
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Compressing objects: 100% (7/7), done.
Writing objects: 100% (9/9), 712 bytes | 712.00 KiB/s, done.
Total 9 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/padmaraj88/assignment-3.git
 * [new branch]      devlop -> devlop
 * [new branch]      f1 -> f1
 * [new branch]      f2 -> f2
 * [new branch]      master -> master
ubuntu@ip-172-31-17-0:~/assignment3$ git branch -D f2
Deleted branch f2 (was 2a71ee7).
ubuntu@ip-172-31-17-0:~/assignment3$ git branch
  devlop
  f1
* master
ubuntu@ip-172-31-17-0:~/assignment3$ git checkout master
Already on 'master'
ubuntu@ip-172-31-17-0:~/assignment3$ git push origin --delete f2
Username for 'https://github.com': padmaraj88
Password for 'https://padmaraj88@github.com':
To https://github.com/padmaraj88/assignment-3.git
 - [deleted]         f2
ubuntu@ip-172-31-17-0:~/assignment3$
