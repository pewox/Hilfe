https://www.atlassian.com/de/git/tutorials/install-git ```\n```
https://git-scm.com/docs/git#_git_commands

## Git-Commands
```
git config --global user.name "peter"
git config --global user.email "peter@haha.de"
git config --global core.editor "code --wait"  #Vs Code als Standardeditor setzen
git config --list
```
### lokales repo erstellen
```
git init
git init -b <branchname>  # Hier Branchname auf main setzen
#oder git config --global init.defaultBranch main
git add README.md
```
#### Dateien zum Repo hinzufügen
```
git add --all (staged)
git commit -m "first commit"
git branch -M master #(oder main, je nachdem)
git status
```
#### zu vorhandenem github-repo hinzufügen
```
git remote add origin git@github.com:pewox/Hilfe.git  # origin ist das Haupt-Remote-Repo
git remote -v  #überprüfen
git push origin master
#oder
git push -u origin master
#oder
git push -u origin --all

git remote add origin https://github.com/pewox/Hilfe.git
git branch -M main
git push -u origin master
```
### URL ändern
```
git remote set-url origin https://github.com/pewox/Hilfe.git
```
### repo clonen
```
git clone https://github.com/pewox/Hilfe.git  #über https-Verbindung
git clone git@github.com:pewox/Hilfe.git      #über ssh-Verbindung
```
### Änderungen aus Remote-Repo herunterladen
```
git fetch  #lädt aktuellen Stand herunter und aktualisiert lokale kopie
git pull    # führt git fetch und dann git merge aus 
```
### Änderungen in Remote-Repo hochladen
```
git push
```
### Branch erstellen
```
git checkout -b branchname
git branch -m neuername   #Branch umbenennen
```
### Branch löschen
```
git branch -d mein-Branch  # nur löschen, wenn er keine ungemergten Änderungen enthält
```
