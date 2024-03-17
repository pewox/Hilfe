## Git-Commands
```
git config --global user.name "peter"
git config --global user.email "peter@haha.de"
git config --list
```
### lokales repo erstellen
```
git init
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
git remote add origin https://github.com/pewox/Hilfe.git
git remote -v  #überprüfen
git push origin master
#oder
git push -u origin master

git remote add origin https://github.com/pewox/Hilfe.git
git branch -M main
git push -u origin master
```
### repo clonen
```
git clone https://github.com/pewox/Hilfe.git  #über https-Verbindung
git clone git@github.com:pewox/Hilfe.git      #über ssh-Verbindung
```
