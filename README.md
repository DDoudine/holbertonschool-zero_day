# GIT

## Résumé:

Git est un système de gestion de versions décentralisé largement utilisé dans le développement logiciel. Voici un résumé des concepts clés de Git :

1. Dépôt (Repository) :

* Un dépôt Git est un espace de stockage qui contient l'historique des modifications d'un projet.
* Il peut être local sur votre machine ou distant sur un serveur.

2. Commit :

* Un commit représente une modification spécifique dans le projet, accompagnée d'un message descriptif.
* Il crée un point dans l'historique du projet.

3. Branche (Branch) :

* Une branche est une ligne de développement indépendante qui permet de travailler sur des fonctionnalités ou corrections sans affecter la branche principale (généralement appelée "master" ou "main").

4. Fusion (Merge) :

* La fusion combine les modifications de deux branches différentes.
* Cela permet d'incorporer les développements réalisés sur une branche dans une autre.

5. Pull Request (Demande de tirage) :

* Une Pull Request (PR) est une fonctionnalité de certains services Git, tels que GitHub, permettant de soumettre des modifications pour examen avant la fusion.

6. Clone :

* Cloner un dépôt signifie créer une copie locale d'un dépôt distant sur votre machine.

7. Pousser (Push) :

* Pousser signifie envoyer les modifications locales vers un dépôt distant.

8. Tirer (Pull) :

* Tirer récupère les modifications d'un dépôt distant et les intègre dans votre dépôt local.

9. Récapitulatif (Status) :

* La commande "git status" affiche l'état des fichiers dans le dépôt, indiquant s'ils ont été modifiés, ajoutés ou supprimés.

10. Ignorer des fichiers (Gitignore) :

* Un fichier ```bash.gitignore``` spécifie les fichiers et répertoires à ignorer lors des opérations Git, tels que les fichiers temporaires ou les fichiers de configuration.

En résumé, Git est un système de gestion de versions qui permet de suivre les modifications, de collaborer sur des projets, de travailler sur des fonctionnalités indépendantes via des branches, et de fusionner les changements de manière contrôlée. Les commandes de base incluent commit, branch, merge, pull, push, status, et ignore.

## Concepts:
For this projects, we expect you to look at these concepts :
* [Source Code Management](https://intranet.hbtn.io/concepts/878)
* [Git And Github Cheat Sheet](https://intranet.hbtn.io/concepts/879)
* [The Framework](https://intranet.hbtn.io/concepts/880)
* [Approaching A Project](https://intranet.hbtn.io/concepts/881)


# Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General
* What is source code management
* What is Git
* What is GitHub
* What is the difference between Git and GitHub
* How to create a repository
* What is a README
* How to write good READMEs
* How to commit
* How to write helpful commit messages
* How to push code
* How to pull updates
* How to create a branch
* How to merge branches
* How to work as collaborators on a project
* Which files should and which files should not appear in your repo

# Requirements
## General
* A README.md file at the root of the repo, containing a description of the repository
* A README.md file, at the root of the folder of this project (i.e. git), describing what this project is about
* Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
* Your answer files should only contain the command, and nothing else

# More Info
## Install git
### If git is not already installed on your terminal:

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```

# Basic usage
## At the end of this project you should be able to reproduce and understand these command lines:

```bash
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main 
```