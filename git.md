
##### Einrichtung

    # Editor für commit-msg ändern:
    git config --global core.editor "vim"

    git config --global user.name [myusername]
    git config --global user.name [username@host.com]

    # Rename Detection als Default einstellen:
    git config --global diff.renames true

    git clone pr3d@ubunas:~/my_scripts
    # Start new Repo on my server:
    git init --bare foldername.git

    git checkout [brachname]

##### Log mit Dateiänderungen anzeigen:
    git log -p
    git log --oneline
    git log --stat

##### verschoben und kopiert mit anzeigen:
    git log --follow

##### nur die letzten 5 Einträge anzeigen
    git log -5

    # just a list all repo CONTRIBUTORS:
    git log --format='%aN <%aE>' | sort -u

    git status --short

##### alle geänderten und hinzugefügten Dateien vom aktuellen VZ und unter-VZs zum staging hinzufügen
    git add .

##### Datei ‚unstagen'
    git reset <filePath>

##### direktes commit ohne staging
    git commit --all
    git commit file1.txt file2.txt

##### Alle Änderungen am Workspace in Zwischenspeicher übernehmen
    git stash --include-untracked

##### letzten Änderungen zurückholen
    git stash pop

##### Merge abbrechen
    git reset --merge

##### Change remote from https to SSH (to allow push via ssh public key)

    git remote set-url origin git@github.com:<USERNAME>/<REPONAME>.git
    git remote add [name] file:///User/name/path/repo.git

##### Zeige konfigurierte Remotes an (push/fetch)
    git remote --verbose
    git remote show [name]

##### Zeige Verknüpfungen von lokalen branches zu Upstream-Branches an
    git branch --list -vv


##### Neuen Branch anlegen und auschecken

    git checkout -b [newBranch]

    git checkout -b [FeatureBranch] [SourceBranch]
    git checkout -b feature/TicketNr develop

***

## Links:

- [A successful Git branching model (git flow)](http://nvie.com/posts/a-successful-git-branching-model/)
