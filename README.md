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

Suivre le tutoriel a été jusque là, la chose la plus dure que j'ai eu à faire. 
Arrivé à la treizième minute, j'étais bloqué. Peu importe ce que j'essayais, il n'y avait pas moyen de passer à l'étape suivante.
J'ai été bloqué à onze heures. C'est à vingt-et-une heures que j'ai enfin réussi. Comment ai-je fait ?
J'ai d'abord mis la vidéo en vitesse ralentie(0.75), j'ai regardé encore et encore. J'ai **comparé** chaque résultat que j'obtenais avec celui du gars de la vidéo. Ce n'est qu'ainsi que ma compréhension des outils de Fusion 360 a drastiquement augmenté. 
Entre temps(grâce à la vidéo), je me suis rendu compte que j'avais la possibilité de modéliser le boitier lui même et pas seulement ses côtés. 
Cela m'a amené à reprendre de zéro : 
# From
![Capture d'écran 2024-03-17 092420](https://github.com/purplekan/S.P.A.R.K./assets/162813789/c70f0a86-1e23-43ec-b641-96f3c8b66d01)
# To
![Capture d'écran 2024-03-17 113120](https://github.com/purplekan/S.P.A.R.K./assets/162813789/785b76ec-cf2a-463b-a73d-6a5848fd8410)

## b. Début des hostilités 
Une fois débloqué et déterminé à finir ce modèle, je me suis heurté à un nouveau mur : Comment vais-je gérer la mise en place des élémments dans le boîtier ? Comment vais je pouvoir rendre le boîtier ouvrable ?
J'ai finalement opté pour un système de vis et j'ai continué à suivre le tutoriel avec beaucoup d'interruptions car je travaillais aussi durant le cours pour gagner du temps. 
Petit à petit, les esquisses que l'on a réalisé etaient enfin modélisées. 
Le modèle de base est maintenant fin prêt, mais il continuera à être modifié pour des raisons d'esthétique ou d'efficacité. D'ailleurs, je viens à nouveau de le modifier:
![image](https://github.com/purplekan/S.P.A.R.K./assets/162813789/a4c46916-6948-463a-8736-007cda0caff2)
De retour après deux jours de bataille, après des soucis que nous avons rencontré au niveau des circuits et dont je parlerais un peu plus tard, la boîte a dû être refaite et adaptée à la nouvelle configuration :
![Capture d'écran 2024-03-21 125641](https://github.com/purplekan/S.P.A.R.K./assets/162813789/3bcc2cbe-f0b8-413c-94ef-c1207aab03a2)   ![Capture d'écran 2024-03-21 125726](https://github.com/purplekan/S.P.A.R.K./assets/162813789/be9c5626-6536-4ddb-ad2b-b5251770baab)


## 3. Circuits
## a. L'alarme ⏰ 
Nous avons commencé par la fonctionnalité de base de SPARK, celle qui lui permet de se comporter comme une alarme. Pour ce faire, nous avons suivi un certain nombre d'étapes afin de progressivement réussir :
- faire sonner le buzzer
- arrêter le son en appuyant sur un bouton
- implémenter le bouton reset pour réintinialiser l'alarme
- pouvoir récupérer une heure exacte à partir du RTC
- faire sonner l'alarme(le buzzer) à une heure précise et pouvoir l'arrêter à ce moment
Vous pourrez retrouver le code dans le dossier documentation.
En ce qui concerne le fonctionnement, c'est assez simple. Une constante "state" est créée. C'est elle qui détermine si le buzzer émettra le son ou non.
Si l'heure prévue arrive, "state" prends la valeur 0 et le buzzer sonne. Si par contre l'on appuie sur le bouton d'arrêt, "state" prends la valeur 1 et le buzzer s'arrête. https://github.com/purplekan/S.P.A.R.K./assets/162813789/803af92f-aba5-456c-b046-8ecc90c4031f


## b. L'écran 🖥 
Toutes nos tentatives d'utiliser l'écran LCD avec l'I2C se sont soldées par des échecs. C'est certainement ce qui nous a le plus perdu de temps. En fin de compte, nous n'avons pas réussi à déterminer si le problème venait de l'écran, de l'I2C, du code ou des soudures faites. Nous avons dû nous rabattre sur l'écran LCD purement, ce qui a compliqué les câblages et nous a obligé à revoir les mesures du boîtier. Sur l'écran sera affiché la date et l'heure actuelle. 
Lorsque l'alarme sonnera, l'écran affichera la tâche associée à cette heure une fois l'alrme désactivée.

## c. Le joystick analogique 🕹 
Aussi connu sous le nom de HW 504, c'est ce petit bijou qui servira à naviguer entre les diffférentes tâches 
![HW504_B_back](https://github.com/purplekan/S.P.A.R.K./assets/162813789/cbcde223-0892-4bf4-aa78-3fba7d4e18a3)

## d. Le Real Time Clock 🕒 DS1302
En utilisant les bibliothèques <ThreeWire.h> et <RtcDS1302.h>, nous sommes en mesure de récupérer l'heure et la date précise au moment du téléversement. Cependant je ne sais pas si le RTC se base sur l'heure de l'ordinateur 🖥 ou le GMT.  
**if (now.Hour() == X & now.Minute() == Y & now.Second() == Z)** nous permet de créér une condition avec une heure spécifique. Nous aurions aussi pu ajouter la date.
C'est ce que l'on fera pour notre liste de tâches à afficher : des paramètres pour l'heure et la date de sorte que chaque tâche a des valeurs bien définies 
