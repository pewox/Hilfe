## Git-Commands
```
git config --global user.name "peter"
git config --global user.email "peter@haha.de"
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
git branch -M master (oder main, je nachdem)
```
#### zu vorhandenem github-repo hinzufügen
```
git remote add origin https://github.com/pewox/Hilfe.git
git push -u origin master

git remote add origin https://github.com/pewox/Hilfe.git
git branch -M main
git push -u origin master
```
