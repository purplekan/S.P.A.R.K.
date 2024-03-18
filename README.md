# S.P.A.R.K.
DOCUMENTATION PROJET BOOTCAMP 2024

Ce projet vous est présenté par les étudiants d’Eseo-Togo : 
-	NONVIGNON Kenneth
-	BANKA Wilfried
-	MEGUIDA Adebayo
-	BADJA Jules
# I. Introduction 
A l'occasion de l'Arduino's Day, notre école(Cours-Lumière Eseo-Togo) a été sélectionnée. C'est alors une occasion pour nous de mettre en pratique l'ensemble des connaissances accumulées depuis le début de l'année. Nous sommes 17 étudiants en tout encadrés par 5 experts en électronique. Parmi eux se trouve notre professeur de Projet SI : M. HANKEM Justin.
Après nous avoir expliqué en quoi devait consister le travail, nous avons été divisés en 4 groupes. C'est ainsi que Wilfried, Adebayo, Jules et Kenneth(moi) comme le responsable avons été réunis. 
![WhatsApp Image 2024-03-16 à 11 12 30_8e713fb9](https://github.com/purplekan/S.P.A.R.K./assets/162813789/06a1ec63-34f9-4546-a001-493c2e0c38f2)

Il est important d'être méthodique et d'évoluer progressivement, c'est pourquoi nous avons commencé par se réunir et proprement se définir en tant que groupe : V Team.
![image](https://github.com/purplekan/S.P.A.R.K./assets/162813789/453f7e84-2da2-4e54-819c-c35d618d3670)

C'est dans ce groupe que nous avons échangé jusqu'à présent. Nous avons préféré d'éviter au maximum les messages vocaux afin de faciliter l'extraction d'informations un peu plus tard. 

## 1. Problématique
Pour avancer, il faut une raison. Qu'est ce qui nous a poussé à concevoir S.P.A.R.K. ?
![image](https://github.com/purplekan/S.P.A.R.K./assets/162813789/566ce750-a140-473e-a32b-714a58df361e)
Il y a d'abord eu quelques idées de robots que nous avons eu mais c'est S.P.A.R.K. qui, au final, nous a intéressé du fait de son utilité, de sa simplicité et du thème du Bootcamp.
Il vient résoudre le problème de mauvaise organisation auquel nombre d'entre nous fait face. 
S.P.A.R.K. doit être capable de **donner envie** de réaliser la tâche. Un grand effort sera donc consacré afin que l'apparence comme le comportement du robot soit intéressant. 

## 2. Fonctionnalités
Après discussion, nous avons enfin pu dégager les fonctionnalités de notre robot. Cela a nécessité la suppression de nombreuses autres fonctionnalités dû aux contraintes de matériel et de temps(deux semaines pour la conception). Voici les fonctionnalités qui ont été retenues :
| Fonctionnalités             | Description                                                                                                                                 | Degré d'Importance |
|-----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|-------------------|
| Alarme                      | Définit des alarmes pour différentes heures de la journée afin de réveiller les utilisateurs ou de les rappeler à des événements importants. | Élevé             |
| Agenda                      | Fournit les tâches et les événements prévus pour la journée, aidant ainsi les utilisateurs à planifier leur emploi du temps.              | Élevé             |
| Interaction Sociale         | Fait des blagues ou donne des mots d'encouragement pour divertir et amuser les utilisateurs.                                                | Moyen             |
| Gestion des Tâches          | Permet aux utilisateurs de créer, modifier et supprimer des listes de tâches pour rester organisés.                                         | Élevé             |
| Mobilité de SPARK           | Capacité de se déplacer de manière autonome pour accéder à différentes pièces ou zones.                                                      | Moyen             |
| Livraison d'Objets (Optionnel) | Possibilité de transporter et de livrer des objets légers d'un endroit à un autre.                                                           | Faible            |

Une fois ces fonctionnalités clairement définies, nous sommes passés aux choix de composants nécessaires à l'implémentation des fonctionnalités. 

## 3. Liste du matériel
Vu la limite de temps de deux semaines, nous avons dû choisir des composants simples et rapidement accessibles. Ensemble, nous avons réfléchi à quel matériel utiliser pour chaque fonctionnalité de S.P.A.R.K. 
| Matériel                | Description                                                                                             |
|-------------------------|---------------------------------------------------------------------------------------------------------|
| Buzzer                  | Pour simuler le son d'une alarme.                                                                       |
| Boutons poussoirs       | Pour gérer tout type de touches et commander le robot.                                                  |
| Écran LCD 16 * 2        | Pour afficher les informations.                                                                         |
| Joystick analogique     | Pour accéder facilement au menu des fonctions du robot.                                      |
| Arduino UNO             | Microcontrôleur principal du robot.                                                                     |
| Module RTC              | Pour avoir l'heure en temps réel.                                                                       |
| Module haut-parleur     | Pour produire du son à partir de l'Arduino.                                                              |
| Batterie 9V             | Pour l'alimentation du robot.                                                                           |
| Fils de connexion et Breadboard | Pour connecter les composants électroniques.                                                   |
| LED témoin              | Pour indiquer l'état ou le fonctionnement du robot.                                                    |
| PLA                     | Matériau pour le boîtier du robot.                                                                      |
| Vis et écrous           | Pour assembler les composants du robot.                                                                 |
| Pistolet à colle chaude et ruban adhésif | Pour le montage et la fixation des composants.                                           |

# II. Il est temps de se mettre au travail !
## 1. Répartition des tâches 
Après avoir clairement défini nos objectifs et ce dont on aura besoin pour les réaliser, il était enfin temps de partitionner le travail afin qu'il soit réalisé efficacement. Nous avions donc un groupe qui s'occupait des circuits à réaliser puis de l'autre, le groupe chargé de la modélisation 3D du robot.
Bien entendu, il y a eu des moments où nous avons eu à discuter tous les quatres afin d'harmoniser nos travaux, afin de s'entraider et de s'échanger des conseils. 

## 2. Modélisation 3D
La modélisation du boîtier de S.P.A.R.K. n'a pas été de tout repos. En effet, après avoir décidé de la forme générale de notre robot, nous avons fais les esquisses des principales faces de ce boîtier. Il faut dire que c'était une première expérience pour nous, surtout que cela demandait des bases en dessin technique afin d'avoir un résultat potable. C'est non sans mal que nous sommes parvenus en quelque sorte à la face principale de S.P.A.R.K. Voyez plutôt par vous même : 
![WhatsApp Image 2024-03-16 à 13 03 51_c4468697](https://github.com/purplekan/S.P.A.R.K./assets/162813789/67f42845-9552-4efc-916a-84e16ef20593)

C'est très loin du niveau attendu d'un étudiant en prépa, mais je crois fermement que le plus important dans une représentation c'est que tous les détails y figurent. Après tout, le dessin peut etre arrangé. Je vous laisse entrevoir ce que c'est devenu une fois modélisé : 
![image](https://github.com/purplekan/S.P.A.R.K./assets/162813789/7f0a8d09-e304-4d0e-abe2-646b47bf58c4)

Comme vous avez pu le remarquer, il y a eu entre temps quelques modifications mais nous y reviendrons.

## a. Essai de modélisation 
Il m'était d'abord venu à l'idée, de modéliser les 6 faces séparément afin de ne pas avoir de complications lors du montage du circuit.
Nous avons alors entamé la face principale, celle du devant : 
![Capture d'écran 2024-03-17 085742](https://github.com/purplekan/S.P.A.R.K./assets/162813789/1916ad9d-7b65-44de-8657-1d5f5063a6ca)
L'idée était de créér un trou de la taille des composants dans la face afin que nous puissions les insérer aisément plus tard. Ah quel naïf j'étais ! Comment aurais-je puis savoir que je m'enfonçais dans un piège. Le premier problème s'est posé quand je me suis retrouvé dans l'incapacité de mettre créér un trou de la forme du composant alors que j'avais enfin réussi à l'encastrer dans la face. Je me suis alors tourné vers mes supérieurs. Monsieur OLANLO me donna plus d'explications concernant ce qui me troublait, et comme pour appuyer ses paroles, il nous partagea le lien d'une vidéo youtube qui expliquait en partie comment parvenir au résultat souhaité. 
https://youtu.be/83E3qum343k?si=9i2ab8cILzj7SOyi



