# GIT

## Résumé:

## GIT

Git est un système de gestion de versions qui permet de suivre les modifications dans un projet. Les commits enregistrent des snapshots du code, les branches permettent le développement parallèle, et les fusions intègrent les changements. Les Pull Requests facilitent la collaboration en permettant l'examen avant la fusion. Cloner crée une copie locale, pousser envoie des commits vers un dépôt distant, et tirer récupère les changements. La commande "git status" donne l'état des fichiers, et le fichier .gitignore spécifie ceux à ignorer. En résumé, Git offre un contrôle précis sur l'évolution des projets, favorise la collaboration et permet une gestion efficace des versions.

## GITHUB

GitHub est une plateforme de développement collaborative basée sur Git, offrant des fonctionnalités avancées pour le stockage, la gestion et la collaboration autour des dépôts Git.

1. Dépôts :

GitHub héberge des dépôts Git, qui sont des espaces de stockage pour les projets, contenant l'historique des versions et les fichiers associés.

2. Collaboration :

Facilite la collaboration entre développeurs en permettant le partage de dépôts, les Pull Requests pour l'examen de code, et les discussions autour des modifications.

3. Gestion de Projet :

Offre des fonctionnalités de gestion de projet avec des tableaux Kanban, des problèmes, et des projets, facilitant le suivi des tâches et des problèmes.

4. Intégration Continue :

Prise en charge de l'intégration continue avec des services comme Actions GitHub, permettant l'automatisation des tests et des déploiements.

5. Hébergement de Pages :

Permet l'hébergement de sites web statiques directement depuis les dépôts, utilisant le service GitHub Pages.

6. Réseau Social :

GitHub fonctionne comme un réseau social pour les développeurs, facilitant la découverte de projets, le suivi d'autres développeurs, et la participation à des communautés open source.

En résumé, GitHub est une plateforme complète qui simplifie la gestion de projets Git, favorise la collaboration entre les développeurs, offre des outils de gestion de projet avancés, et fonctionne comme une communauté sociale pour les passionnés de développement.

## GIT et GITHUB

L'utilisation de Git et GitHub implique plusieurs étapes, de la configuration initiale à la gestion quotidienne des projets. Voici un guide général :

### Configuration initiale :
1. Installer Git :

* Téléchargez et installez Git depuis git-scm.com.
* Configurez votre nom d'utilisateur et votre adresse e-mail via la commande :
```bash
git config --global user.name "Votre Nom"
git config --global user.email "votre@email.com"
```

2. Créer un compte GitHub :

* Allez sur GitHub et créez un compte.

3. Générer une paire de clés SSH (optionnel mais recommandé) :

* Suivez les instructions ici pour générer des clés SSH.

### Créer un nouveau dépôt (repository) :
1. Initialiser un dépôt local :

* Utilisez la commande git init dans le répertoire de votre projet.
2. Ajouter des fichiers au suivi de Git :

* Utilisez git add pour ajouter des fichiers au suivi de Git.
```bash
git add fichier1 fichier2
```

3. Faire un commit :

* Enregistrez les modifications avec un commit.
```bash
git commit -m "Message descriptif"
```

### Travailler avec des branches :
1. Créer une nouvelle branche :

* Utilisez git branch pour créer une nouvelle branche.
```bash
git branch nom_de_la_branche
```

2. Basculer entre les branches :

* Utilisez git checkout pour changer de branche.
```bash
git checkout nom_de_la_branche
```

3. Fusionner des branches :

* Fusionnez une branche avec git merge.
```bash
git merge nom_de_la_branche
```

### Travailler avec GitHub :
1. Créer un dépôt sur GitHub :

* Sur GitHub, créez un nouveau dépôt.

2. Lier le dépôt local à GitHub :

* Ajoutez le dépôt distant avec git remote.
```bash
git remote add origin lien_vers_votre_depot_github.git
```

3. Pousser des commits sur GitHub :

* Utilisez git push pour envoyer vos commits sur GitHub.
```bash
git push -u origin nom_de_votre_branche
```

4. Créer une Pull Request (PR) :

* Sur GitHub, créez une PR pour demander la fusion de vos modifications.

5. Récupérer des modifications depuis GitHub :

* Utilisez git pull pour récupérer les modifications depuis GitHub.
```bash
git pull origin nom_de_votre_branche
```


## Resources:
* [Resources To Learn Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
* [Git And Github Cheat Sheet](https://intranet.hbtn.io/concepts/879)
* [The Framework](https://intranet.hbtn.io/concepts/880)
* [Approaching A Project](https://intranet.hbtn.io/concepts/881)

## Requirements:

* A README.md file at the root of the repo, containing a description of the repository
* A README.md file, at the root of the folder of this project (i.e. git), describing what this project is about
* Do not use GitHub’s web UI, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
* Your answer files should only contain the command, and nothing else

## More Info

### Install git

If git is not already installed on your terminal:

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```

### Basic usage

At the end of this project you should be able to reproduce and understand these command lines:

```bash
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```
## TASKS: 

### 0. Create And Setup Your Git And Github Account
#### Step 0 - Create an account on GitHub

You will need a GitHub account for all your projects. You can create an account for free here

#### Step 1 - Create a Personal Access Token on Github

To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow this tutorial to create a token.

#### Step 2 - Update your profile on the Intranet

Update your Intranet profile by adding your Github username here

If it’s not done the Checker won’t be able to correct your work

#### Step 3 - Create your first repository

Using the graphic interface on the github website, create your first repository.

* Name: Look at the bottom of the project to see the name of the repository
* Description: This is my first repository as a full-stack engineer
* Public repo
* No README, .gitignore, or license

#### Step 4 - Open the sandbox

On the intranet, just under the task, click on the button >_Get a sandbox and run to start the machine. Once the container is started, click on >_Webterm to open a shell where you can start work from.

#### Step 5 - Clone your repository

On the webterm of the sandbox, do the following:

* Clone your repository

```bash
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                  
Cloning into '{YOUR_REPO}'...
warning: You appear to have cloned an empty repository.
```

* Replace {YOUR_PERSONAL_TOKEN} with your token from step 1
* Replace {YOUR_USERNAME} with your username from step 0 and 1
* Replace {YOUR_REPO} with the name of the reposotiry at the bottom of the task

#### Step 6 - Create the README.md and push the modifications

* Navigate to this new directory. Tips

```bash
root@896cf839cf9a:/# cd {YOUR_REPO}/
root@896cf839cf9a:/{YOUR_REPO}#
```

* Create the file README.md with the content My first readme. Tips

```bash
root@896cf839cf9a:/{YOUR_REPO}# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/{YOUR_REPO}# cat README.md                                                                                      
My first readme                                                                                                                       
```                                                                                                         
* Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin

```bash
root@896cf839cf9a:/{YOUR_REPO}# git add .
root@896cf839cf9a:/{YOUR_REPO}# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/{YOUR_REPO}# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                                                                                       
 * [new branch]      master -> master 
```

Good job!

You pushed your first file in your first repository.
You can now check your repository on GitHub to see if everything is good.

### 1. Repo-Session
Create a new directory called git in your repo.
Make sure you include a not empty README.md in your directory:

* at the root of your repository
* AND in the directory git

And important part: Make sure your commit and push your code to Github - otherwise the Checker will always fail.

### 2. Coding Fury Road
For the moment we have an empty project directory containing only a README.md. It’s time to code !

* Create these directories at the root of your project: bash, c, js
* Create these empty files:
 * c/c_is_fun.c
 * js/main.js
 * js/index.js

* Create a file bash/best with these two lines inside: #!/bin/bash and echo "Best"
* Create a file bash/school with these two lines inside: #!/bin/bash and echo "School"
* Add all these new files to git
* Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

3. Collaboration Is The Base Of a Company
A branch is like a copy of your project. It’s used mainly for:

* adding a feature in development
* collaborating on the same project with other developers
* not breaking your entire repository
* not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch update_script and in this branch:

* Create an empty file named bash/98
* Update bash/best by replacing echo "Best" with echo "Best School"
* Update bash/school by replacing echo "School" with echo "The school is open!"
* Add and commit these changes (message: “My personal work”)
* Push this new branch Tips

Perfect! You did an amazing update in your project and it’s isolated correctly from the main branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

* Change branch to main
* Update the file bash/best by replacing echo "Best" with echo "This School is so cool!"
* Delete the directory js
* Commit your changes (message: “Hot fix”) and push to the origin

### 4. Collaboration: Be Up To Date
Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – and only for this task – please update your file README.md in the main branch from GitHub.com. It’s the only time you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

* Get all changes of the main branch locally (i.e. your README.md file will be updated)
* Create a new file up_to_date at the root of your directory and in it, write the git command line used
* Add up_to_date to git, commit (message: “How to be up to date in git”), and push to the origin

### 5. Haaa What Did You Do ???
Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch update_script to main: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

HHHHHHHAAAAAAAA

```bash
CONFLICT (content): Merge conflict in bash/best
```


As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch update_script, and push the result to the origin.

At the end, you should have all your work from the branch update_script (new file and two updated files) and all latest main commits (new files, delete folder, etc.), without conflicts.

### 6. Never Push Too Much
Create a .gitignore file and define a rule to never push ~ files (generated by Emacs). Tips
