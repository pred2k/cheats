
##### Change remote from https to SSH (to allow push via ssh public key)

    git remote set-url origin git@github.com:<USERNAME>/<REPONAME>.git

##### Neuen Branch anlegen und auschecken

    git checkout -b [newBranch]

    git checkout -b [FeatureBranch] [SourceBranch]
    git checkout -b feature/TicketNr develop

##### List all repo CONTRIBUTORS:

    git log --format='%aN <%aE>' | sort -u


***

## Links:

- [A successful Git branching model (git flow)](http://nvie.com/posts/a-successful-git-branching-model/)
