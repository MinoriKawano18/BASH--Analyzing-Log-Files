# Unsure of why my code is crossed out.


# BASH--Analyzing-Log-Files
ubuntu@ip-172-31-83-6:~$ git clone https://github.com/kura-labs-org/install-sh.git
Cloning into 'install-sh'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.
ubuntu@ip-172-31-83-6:~$ cd install.sh
-bash: cd: install.sh: No such file or directory
ubuntu@ip-172-31-83-6:~$ cd install-sh
ubuntu@ip-172-31-83-6:~/install-sh$ auth_log.log
auth_log.log: command not found
ubuntu@ip-172-31-83-6:~/install-sh$ /var/log/auth_log.log
-bash: /var/log/auth_log.log: No such file or directory
ubuntu@ip-172-31-83-6:~/install-sh$ sudo nano /var/log/auth_log.log
ubuntu@ip-172-31-83-6:~/install-sh$ sudo nano /usr/local/bin/check_suspicious_activity.sh
ubuntu@ip-172-31-83-6:~/install-sh$ sudo nano /var/log/auth_log.log
ubuntu@ip-172-31-83-6:~/install-sh$ sudo nano /usr/local/bin/check_suspicious_activity.sh
ubuntu@ip-172-31-83-6:~/install-sh$ sudo chmod +x /usr/local/bin/check_suspicious_activity.sh
ubuntu@ip-172-31-83-6:~/install-sh$ cat /var/log/suspicious_activity.log
cat: /var/log/suspicious_activity.log: No such file or directory
ubuntu@ip-172-31-83-6:~/install-sh$ cat /var/log/auth_log.log
#!/bin/bash

#identify the log file and what the output is
Log_file="/var/log/auth_log.log"
Output_file="/var/log/suspicious_activity.log"

#identify keywords for suspicious activity
Keywords=("failed" "invalid" "failure")

#clear out output file
. "$Output_file"

#loop through keywords and search
for Keyword in "$Keywords[@]}"; do
        grep "Keywords" "$Log_file" >> "$Output_file"
done

echo "Check for suspicious activity done. Results stored in Output_file."


ubuntu@ip-172-31-83-6:~/install-sh$ sudo crontab -e
no crontab for root - using an empty one

Select an editor.  To change later, run 'select-editor'.
  1. /bin/nano        <---- easiest
  2. /usr/bin/vim.basic
  3. /usr/bin/vim.tiny
  4. /bin/ed

Choose 1-4 [1]: 1
crontab: installing new crontab
ubuntu@ip-172-31-83-6:~/install-sh$ sudo /usr/local/bin/check_suspicious_activity.sh
/usr/local/bin/check_suspicious_activity.sh: line 11: /var/log/suspicious_activity.log: No such file or directory
Check for suspicious activity done. Results stored in Output_file.
ubuntu@ip-172-31-83-6:~/install-sh$ sudo crontab -l

0 1 * * * /usr/local/bin/check_suspicious_activity.sh
ubuntu@ip-172-31-83-6:~/install-sh$ ls
auth_log_creation.sh  vscode_install.sh
ubuntu@ip-172-31-83-6:~/install-sh$ cd suspicious_activity
-bash: cd: suspicious_activity: No such file or directory
ubuntu@ip-172-31-83-6:~/install-sh$ ./suspicious_activity.sh
-bash: ./suspicious_activity.sh: No such file or directory
ubuntu@ip-172-31-83-6:~/install-sh$ git remote add origin https://github.com/MinoriKawano18/BASH--Analyzing-Log-Files.git
error: remote origin already exists.
ubuntu@ip-172-31-83-6:~/install-sh$ git branch -M main
ubuntu@ip-172-31-83-6:~/install-sh$ git push -u origin main
Username for 'https://github.com': MinoriKawano18
Password for 'https://MinoriKawano18@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/kura-labs-org/install-sh.git/'
ubuntu@ip-172-31-83-6:~/install-sh$ git branch -M main
ubuntu@ip-172-31-83-6:~/install-sh$ git push -u origin main
Username for 'https://github.com': MinoriKawano18
Password for 'https://MinoriKawano18@github.com': 
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ ssh -i /path/to/your-key.pem ec2-user@your-ec2-instance-public-dns
Warning: Identity file /path/to/your-key.pem not accessible: No such file or directory.
ssh: Could not resolve hostname your-ec2-instance-public-dns: Temporary failure in name resolution
ubuntu@ip-172-31-83-6:~/install-sh$ echo "# BASH--Analyzing-Log-Files" >> README.md
ubuntu@ip-172-31-83-6:~/install-sh$ git init
Reinitialized existing Git repository in /home/ubuntu/install-sh/.git/
ubuntu@ip-172-31-83-6:~/install-sh$ git add README.md
ubuntu@ip-172-31-83-6:~/install-sh$ git commit -m "first commit"
[main 0521520] first commit
 Committer: Ubuntu <ubuntu@ip-172-31-83-6.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 README.md
ubuntu@ip-172-31-83-6:~/install-sh$ git branch -M main
ubuntu@ip-172-31-83-6:~/install-sh$ git remote add origin https://github.com/MinoriKawano18/BASH--Analyzing-Log-Files.git
error: remote origin already exists.
ubuntu@ip-172-31-83-6:~/install-sh$ git push -u origin main
Username for 'https://github.com': MinoriKawano18
Password for 'https://MinoriKawano18@github.com': 
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ echo "# BASH--Analyzing-Log-Files" >> README.md
ubuntu@ip-172-31-83-6:~/install-sh$ git init
Reinitialized existing Git repository in /home/ubuntu/install-sh/.git/
ubuntu@ip-172-31-83-6:~/install-sh$ git add README.md
ubuntu@ip-172-31-83-6:~/install-sh$ git commit -m "first commit"
[main ad2e9ac] first commit
 Committer: Ubuntu <ubuntu@ip-172-31-83-6.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
ubuntu@ip-172-31-83-6:~/install-sh$ git branch -M main
ubuntu@ip-172-31-83-6:~/install-sh$ git remote add origin https://github.com/MinoriKawano18/BASH--Analyzing-Log-Files.git
error: remote origin already exists.
ubuntu@ip-172-31-83-6:~/install-sh$ git push -u origin main
Username for 'https://github.com': MinoriKaawano18
Password for 'https://MinoriKaawano18@github.com': 
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ git remote set-url origin https://MinoriKawano18:                                  @github.com/kura-labs-org/install-sh.gi
t
ubuntu@ip-172-31-83-6:~/install-sh$ git clone https://github.com/MinoriKawano18/BASH--Analyzing-Log-Files.git
Cloning into 'BASH--Analyzing-Log-Files'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
ubuntu@ip-172-31-83-6:~/install-sh$ git pull origin main
From https://github.com/kura-labs-org/install-sh
 * branch            main       -> FETCH_HEAD
Already up to date.
ubuntu@ip-172-31-83-6:~/install-sh$ git push origin main
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ git credential-cache exit
ubuntu@ip-172-31-83-6:~/install-sh$ git remote set-url origin https://MinoriKawano18:                               @github.com/kura-labs-org/install-sh.gi
t
ubuntu@ip-172-31-83-6:~/install-sh$ git clone https://github.com/kura-labs-org/install-sh.git
Cloning into 'install-sh'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.
ubuntu@ip-172-31-83-6:~/install-sh$ git pull origin main
From https://github.com/kura-labs-org/install-sh
 * branch            main       -> FETCH_HEAD
Already up to date.
ubuntu@ip-172-31-83-6:~/install-sh$ git push origin main
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ git clone
fatal: You must specify a repository to clone.

usage: git clone [<options>] [--] <repo> [<dir>]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    --reject-shallow      don't clone shallow repository
    -n, --no-checkout     don't create a checkout
    --bare                create a bare repository
    --mirror              create a mirror repository (implies bare)
    -l, --local           to clone from a local repository
    --no-hardlinks        don't use local hardlinks, always copy
    -s, --shared          setup as shared repository
    --recurse-submodules[=<pathspec>]
                          initialize submodules in the clone
    --recursive ...       alias of --recurse-submodules
    -j, --jobs <n>        number of submodules cloned in parallel
    --template <template-directory>
                          directory from which templates will be used
    --reference <repo>    reference repository
    --reference-if-able <repo>
                          reference repository
    --dissociate          use --reference only while cloning
    -o, --origin <name>   use <name> instead of 'origin' to track upstream
    -b, --branch <branch>
                          checkout <branch> instead of the remote's HEAD
    -u, --upload-pack <path>
                          path to git-upload-pack on the remote
    --depth <depth>       create a shallow clone of that depth
    --shallow-since <time>
                          create a shallow clone since a specific time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --single-branch       clone only one branch, HEAD or --branch
    --no-tags             don't clone any tags, and make later fetches not to follow them
    --shallow-submodules  any cloned submodules will be shallow
    --separate-git-dir <gitdir>
                          separate git dir from working tree
    -c, --config <key=value>
                          set config inside the new repository
    --server-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only
    --filter <args>       object filtering
    --remote-submodules   any cloned submodules will use their remote-tracking branch
    --sparse              initialize sparse-checkout file to include only files at root

ubuntu@ip-172-31-83-6:~/install-sh$ git clone https://github.com/MinoriKawano18/BASH--Analyzing-Log-Files.git
fatal: destination path 'BASH--Analyzing-Log-Files' already exists and is not an empty directory.
ubuntu@ip-172-31-83-6:~/install-sh$ git push git push origin main
error: src refspec push does not match any
error: failed to push some refs to 'git'
ubuntu@ip-172-31-83-6:~/install-sh$ git push origin main
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ git config --global user.name
ubuntu@ip-172-31-83-6:~/install-sh$ git config --global user.name "Minori Kawano"
ubuntu@ip-172-31-83-6:~/install-sh$ git config --global user.email "minorikawano1@gmail.com"
ubuntu@ip-172-31-83-6:~/install-sh$ git init
Reinitialized existing Git repository in /home/ubuntu/install-sh/.git/
ubuntu@ip-172-31-83-6:~/install-sh$ git add .
warning: adding embedded git repository: BASH--Analyzing-Log-Files
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint: 
hint:   git submodule add <url> BASH--Analyzing-Log-Files
hint: 
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint: 
hint:   git rm --cached BASH--Analyzing-Log-Files
hint: 
hint: See "git help submodule" for more information.
warning: adding embedded git repository: install-sh
ubuntu@ip-172-31-83-6:~/install-sh$ git rm --cached BASH--Analyzing-Log-Files
error: the following file has staged content different from both the
file and the HEAD:
    BASH--Analyzing-Log-Files
(use -f to force removal)
ubuntu@ip-172-31-83-6:~/install-sh$ git commit -m "Initial commit"
[main 6c704e1] Initial commit
 2 files changed, 2 insertions(+)
 create mode 160000 BASH--Analyzing-Log-Files
 create mode 160000 install-sh
ubuntu@ip-172-31-83-6:~/install-sh$ git remote add https://github.com/MinoriKawano18/BASH--Analyzing-Log-Files.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

ubuntu@ip-172-31-83-6:~/install-sh$ git push -u origin master
error: src refspec master does not match any
error: failed to push some refs to 'https://github.com/kura-labs-org/install-sh.git'
ubuntu@ip-172-31-83-6:~/install-sh$ git push -u origin main
remote: Permission to kura-labs-org/install-sh.git denied to MinoriKawano18.
fatal: unable to access 'https://github.com/kura-labs-org/install-sh.git/': The requested URL returned error: 403
ubuntu@ip-172-31-83-6:~/install-sh$ 
