# Projet Informatique :
## Notice Technique
---
![quiEstCe](./asset/images/guide/quiEstCe.jpg "quiEstCe")
---
### Réaliser par :
Florent VILLENEUVE - Julien TERRIER - Adrien KAISER - Olivier MAHE

## Introduction :

Le but du projet et d'implémenter un "Qui est-ce ?" compétitif en ligne de commande qui permettra à la classe de fraterniser joyeusement durant les pauses.
Notre implémentation du jeu consistera à ce que chaque élève affronte l'ordinateur et devine le plus vite possible le personnage de celui-ci. Un classement sera effectué selon le temps mis par la classe et un gagnant pourra être désigné ainsi. L'interface étant purement textuel il faudra que les personnages utilisés soient connus de tous, nous prendront donc les élèves de la classe.
---
## Cahier des charges :

Pour le mode de jeu de base décrit plus haut :
- Un élève sera choisi aléatoirement parmi la base de données
- La liste des personnages sera affiché à l'écran de l'utilisateur comme un vrai joueur devant son plateau de jeu
- Les élèves pourront poser des questions à l'ordinateur/au serveur. 
*Exemple : "Le personnage a-t-il les yeux bleus ?"* Ces choix ne seront pas tapés à la main mais choisie à l'aide d'un menu
- Ce cycle de question réponse se poursuit jusqu'à ce que le joueur trouve le personnage
- Le premier joueur qui gagne déclenche l'arret de la partie
---
## Organigramme de l’équipe projet :

Chef de projet | Commercial | Système Administeur | Architecte Programme
 :---: | :---: | :---:  | :---: 
![oliv](./asset/images/notice/oliv.png "oliv")| ![moi](./asset/images/notice/moi.png "moi") | ![julien](./asset/images/notice/julien.png "julien") | ![flo](./asset/images/notice/flo.png "flo") 
Olivier MAHE | Adrien KAISER | Julien TERRIER | Florent VILLENEUVE
         
---
## Mise en place du projet :

### Prémice du projet
Nous avons dans un premier temps défini, les grandes lignes du projet en se réunissant autour d'un diagramme explicatif de nos idées.
Une fois nos idées misent en accords, nous avons commencé les tests avec la réalisations de pipe nommés,  la base de données...

---
![arch](./asset/images/notice/arch.png "arch")
---

Des que notre base fut établie, nous nous sommes lancé dans l'élaboration d'une architecture viable. C'est-à-dire d'avoir une base qui fait tourner le programme sur une RPI avec une connection des clients en ssh,
Pour plus de détails, nous avons réaliser deux programmes fonctionnant sur la même machine qui communique via des pipes.

### Première base

Après avoir conçu notre première architecture nous avons pu affiner notre vision du projet et nous recentrer sur une même vision des choses,
en modifiant le fonctionnement du programme serveur pour qu'il créer un processus fils à chaque connection d'un client qui renvoyer un une réponse au client pour savoir si tout c'est bien créer.

---
![arch2](./asset/images/notice/arch2.png "arch2")
---

Une fois la communication fonctionnelle nous avons commencé l'élaboration du menu permettant de jouer dans le programme client pour réduire le nombre d'échange serveur/client.

### Architecture finale

Enfin, après avoir réussi à implémenter tout nos attente, nous avons choisi d'ajouter une carte olimex avec un écran à notre système pour afficher le nom du gagnant, et également parfaire l'ensemble du projet 

---
![arch3](./asset/images/notice/arch3.png "arch3")
---

 
