## :gear: OnboardingGit
Un court tutoriel pour apprendre les commandes basiques et essentielles de Git.

## 🧰 Tutoriel Git : Les bases indispensables
### 📌 Qu’est-ce que Git ?

Git est un système de contrôle de version distribué.
Il permet de :
  - Suivre l’historique des modifications d’un projet
  - Travailler à plusieurs sans écraser le travail des autres
  - Créer des branches pour développer des fonctionnalités séparément
  - Revenir facilement en arrière en cas d’erreur
  - Git fonctionne en local, sur ton ordinateur : tu possèdes ta propre copie complète du dépôt.

https://www.youtube.com/watch?v=2ReR1YJrNOM 

### 📌 Qu’est-ce que GitHub ?

GitHub est une plateforme en ligne (un service) hébergeant des dépôts Git.
Il permet de :
  - Stocker ton code dans le cloud
  - Collaborer via des Pull Requests
  - Réviser du code
  - Gérer les tickets, la documentation, la CI/CD, etc.

⚠️ GitHub n’est pas Git, c’est un hébergeur et un écosystème autour de Git.

https://www.youtube.com/watch?v=pBy1zgt0XPc

### 📌 Différences entre Git et GitHub
| **Git** | **GitHub** |
|:-|:-|
| Outil installé sur ton ordinateur | Plateforme web en ligne |
| Permet de versionner et gérer les commits  | Permet de partager, collaborer, faire des PR |
| Fonctionne même sans internet  | Nécessite internet |
| Gratuit, open-source | Gratuit + options payantes |
| Commandes en ligne de commande  | Interface web + API + intégrations |```

En résumé :
👉 Git = Le moteur
👉 GitHub = Le garage où tu stockes et partages ton moteur

https://www.youtube.com/watch?v=wpISo9TNjfU

## 📖 Commande de bases

Nous allons utiliser un repo test pour manipuler les commandes les plus courantes.
Ces exercices supposent que le dépôt existe déjà sur GitHub.

Assure-toi d’avoir :
  - Git installé
  - VS Code avec l’extension GitHub recommandée par VS Code.

## 1️⃣ Cloner un dépôt (Clone)
### Via VS Code

1. Ouvre VS Code
2. Clique sur Clone Git Repository sur la page d'accueil.
4. Colle l’URL GitHub : 
5. Choisis un dossier de destination.
6. VS Code propose d’ouvrir le dossier → clique sur Open.

➡️ Le dépôt est maintenant en local.

## 2️⃣ Récupérer les dernières modifications (Pull)

Dans VS Code :
1. Ouvre le menu Source Control.
2. En haut, clique sur les …
3. Sélectionne Pull.

➡️ VS Code télécharge et fusionne automatiquement les changements.

## 3️⃣ Récupérer sans modifier le code local (Fetch)

Toujours dans Source Control :
1. Menu … → Fetch
  
➡️ Met à jour les infos distantes sans toucher à tes fichiers locaux.

## 4️⃣ Enregistrer une modification (Commit)

1. Modifie un fichier dans VS Code.
2. Ouvre Source Control.
3. Tous les fichiers modifiés apparaissent.
4. Tape un message dans la zone Message -> Il faut qu'il soit le plus personnalisé et en rapport avec la modification que possible.
5. Clique sur Commit.

➡️ Le commit est enregistré localement.

## 5️⃣ Envoyer les commits sur GitHub (Push)

Après un commit, un bouton Sync ou Push apparaît en haut du Source Control :
1. Clique sur Push

➡️ VS Code envoie les commits sur GitHub.

## 6️⃣ Synchroniser les changements (Sync)

Le bouton Sync effectue automatiquement :
- un Pull
- puis un Push

C’est l’action recommandée si tu travailles en équipe.

## 7️⃣ Créer une nouvelle branche (Create Branch)

Dans VS Code :
1. Clique sur le nom de la branche en bas à gauche (ex : main).
2. Choisis Create new branch.
3. Donne un nom : feature/nouvelle-fonctionnalité.
4. Publier la branche sur le GitHub grâce au bouton publish.

VS Code se place automatiquement sur la nouvelle branche.

## 8️⃣ Fusionner une branche (Merge)

1. En bas à gauche → clique sur ta branche actuelle
2. Sélectionne la branche sur laquelle tu souhaites fusionner tes modifications pour revenir dessus
3. Menu … → Branch → Merge Branch...
4. Choisis la branche à fusionner from (ex : branche de travail).

➡️ La fusion est appliquée localement, pense ensuite à Push.

## 9️⃣ Ouvrir une Pull Request (PR)

Après avoir push une branche :
1. Aller sur le compte GitHub du repository, et un bouton devrait apparaître, "Create Pull Request".
2. Vérifier bien de rabattre la branche avec les modifications sur la branche voulue. (Branche perso ➡️ Branche dev)
3. S'il n'y a pas de conflits, faire la demande de Pull request. Si conflits, veuillez les résoudre sur votre branche de travail en faisant un merge de la branche de dev sur votre branche de travail.
4. Attendre qu'elle soit validée par un admin du projet.

➡️ La PR est créée sur GitHub.

## 🔟 Supprimer une branche (Delete branch)

Après avoir merger ou effectuer une pull request :
1. Allez sur la branche sur laquelle vous avez mergé vos modifications (la branche d'arrivée)
2. Menu … → Branch → Delete Branch...
3. Séléctionnez la branche à supprimer.
   ⚠️ On ne peut pas supprimer une branche lorsque l’on s’y trouve. Il faut d’abord changer de branche avant de pouvoir la supprimer.
4. Menu … → Branch → Delete Remote Branch...
5. Séléctionnez la même branche de travail à supprimer sur le serveur GitHub.

## Pratiquer
Voici un site web explicant et permettant la pratique des mécaniques principales de git.
[Learn Git Branching](https://learngitbranching.js.org/?locale=fr_FR)

Le site permet de suivre plusieurs tutoriels et exercices portant sur la gestion des systèmes de git, dans un environnement simple.

## 🧪 Tutoriel

### ⏬ Récuperer le projet
D'après les commandes de bases vues au-dessus, récupérez le projet grâce à VS Code.

### 🔃 Changer de branche
Changer de branche, et aller sur la branch "Development".

### ➕ Créer une nouvelle branche
Créer une nouvelle branche qui s'appelle "Votre-nom-dev".

### 💱 Modifier un fichier
Ouvrir le fichier "List_all_participant.txt" et ajouter une nouvelle ligne avec votre prénom.

### 🗨️ Ecrire un commit
Ecrire le commit correspondant à votre modification.

### ⏫ Push
Poussez alors la modification sur le GitHub.

### 🔀 Merge
Une fois que vous voyez votre modification dans votre arbre de suivi, réalisez le merge de votre branch sur la branch "Development".

### ⤵️ Pull request
Afin de rabattre vos modifications, vous devez faire une demande de pull request afin de faire valider votre travail par un admin.

### ❎ Delete branch
Enfin, il est de coutume de supprimer sa branche de travail lorsque l'on a cloturé un point. Supprimer votre branche de travail.
