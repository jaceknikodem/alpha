# Project boilerplate

## Generate SSH keys

```
ssh-keygen -t rsa -b 4096 -C "COMMENT" -f "/Users/USER/.ssh/id_rsa" -N "PASSPHRASE"
ssh-add ~/.ssh/id_rsa
pbcopy < ~/.ssh/id_rsa.pub
```
Go to [github](https://github.com/settings/keys) and add a new key.

## Clone the repo

```
mkdir code; cd code
git clone git@github.com:jaceknikodem/alpha.git
```

## Create .gitignore file

Ignore Python code objects and Pycharm subdirectory:
```
*.py[cod]
.idea/*
```

## Commit the changes

```
git add .
git commit -a
git push origin master
```