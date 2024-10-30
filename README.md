user@c01-16 MINGW64 ~/maryam (main)
$ ssh -T git@github.com
ssh: connect to host github.com port 22: Connection timed out

user@c01-16 MINGW64 ~/maryam (main)
$ git remote -v
origin  https://github.com/engeneyoi/Maryam.midterm.git (fetch)
origin  https://github.com/engeneyoi/Maryam.midterm.git (push)

user@c01-16 MINGW64 ~/maryam (main)
$ git credential-cache exit

user@c01-16 MINGW64 ~/maryam (main)
$ ssh -T git@github.com
ssh: connect to host github.com port 22: Connection timed out

user@c01-16 MINGW64 ~/maryam (main)
$ 

user@c01-16 MINGW64 ~/maryam (main)
$ 

user@c01-16 MINGW64 ~/maryam (main)
$ 

user@c01-16 MINGW64 ~/maryam (main)
$ 

user@c01-16 MINGW64 ~/maryam (main)
$ 

user@c01-16 MINGW64 ~/maryam (main)
$ nano ~/.ssh/config

user@c01-16 MINGW64 ~/maryam (main)
$ ssh -T git@github.com
The authenticity of host '[ssh.github.com]:443 ([140.82.121.36]:443)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[ssh.github.com]:443' (ED25519) to the list of known hosts.
git@ssh.github.com: Permission denied (publickey).

user@c01-16 MINGW64 ~/maryam (main)
$ ssh-add /c/Users/user/.ssh/heya
Could not open a connection to your authentication agent.

user@c01-16 MINGW64 ~/maryam (main)
$ eval "$(ssh-agent -s)"
Agent pid 2158

user@c01-16 MINGW64 ~/maryam (main)
$ ssh-add /c/Users/user/.ssh/heya
Enter passphrase for /c/Users/user/.ssh/heya: 
Identity added: /c/Users/user/.ssh/heya (user@c01-16)

user@c01-16 MINGW64 ~/maryam (main)
$ ssh -T git@github.com
Hi engeneyoi! You've successfully authenticated, but GitHub does not provide shell access.

user@c01-16 MINGW64 ~/maryam (main)
$ git push -u origin main
remote: Permission to engeneyoi/Maryam.midterm.git denied to ArghenXpro.
fatal: unable to access 'https://github.com/engeneyoi/Maryam.midterm.git/': The requested URL returned error: 403

user@c01-16 MINGW64 ~/maryam (main)
$ git remote add origin git@github.com:engeneyoi/Maryam.midterm.git
error: remote origin already exists.

user@c01-16 MINGW64 ~/maryam (main)
$ git branch -M main

user@c01-16 MINGW64 ~/maryam (main)
$ git push -u origin main
remote: Permission to engeneyoi/Maryam.midterm.git denied to ArghenXpro.
fatal: unable to access 'https://github.com/engeneyoi/Maryam.midterm.git/': The requested URL returned error: 403

user@c01-16 MINGW64 ~/maryam (main)
$ git remote remove origin

user@c01-16 MINGW64 ~/maryam (main)
$ push --force
bash: push: command not found

user@c01-16 MINGW64 ~/maryam (main)
$ git push --force
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


user@c01-16 MINGW64 ~/maryam (main)
$ git push --force git@github.com:engeneyoi/Maryam.midterm.git
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream git@github.com:engeneyoi/Maryam.midterm.git main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@c01-16 MINGW64 ~/maryam (main)
$     git push --set-upstream git@github.com:engeneyoi/Maryam.midterm.git main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 606 bytes | 606.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:engeneyoi/Maryam.midterm.git
 * [new branch]      main -> main
branch 'main' set up to track 'git@github.com:engeneyoi/Maryam.midterm.git/main'.

user@c01-16 MINGW64 ~/maryam (main)
$
