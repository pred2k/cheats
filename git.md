
##### Change remote from https to SSH (to allow push via ssh public key)

`git remote set-url origin git@github.com:<USERNAME>/<REPONAME>.git`

##### Neuen Branch anlegen und auschecken

`git checkout -b [newbranch]`

##### List all repo CONTRIBUTORS:

`git log --format='%aN <%aE>' | sort -u`
