# Projet Informatique :
## Notice Technique

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
- Le premier joueur qui gagne déclenche une explosion de saveur sous la forme d'un **STM32 qui fait bip **
---
## Organigramme de l’équipe projet :

Chef de projet | Commercial | Système Administeur | Architecte Programme
 :---: | :---: | :---:  | :---: 
![oliv](./asset/images/notice/oliv.png)| ![moi](./asset/images/notice/moi.png) | ![julien](./asset/images/notice/julien.png) | ![flo](./asset/images/notice/flo.png) 
Olivier MAHE | Adrien KAISER | Julien TERRIER | Florent VILLENEUVE
         
---
## Mise en place du projet :

