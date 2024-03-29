# S.P.A.R.K.
DOCUMENTATION PROJET BOOTCAMP 2024

Ce projet vous est présenté par les étudiants d’Eseo-Togo : 
-	NONVIGNON Kenneth
-	BANKA Wilfried
-	MEGUIDA Adebayo
-	BADJA Jules
# I. Introduction 
A l'occasion de l'Arduino's Day, notre école(Cours-Lumière Eseo-Togo) a été sélectionnée. C'est alors une occasion pour nous de mettre en pratique l'ensemble des connaissances accumulées depuis le début de l'année.  
Nous sommes 17 étudiants en tout encadrés par 5 experts en électronique. Parmi eux se trouve notre professeur de Projet SI : M. HANKEM Justin.  
Après nous avoir expliqué en quoi devait consister le travail, nous avons été divisés en 4 groupes. C'est ainsi que Wilfried, Adebayo, Jules et Kenneth(moi) comme le responsable avons été réunis. 
![WhatsApp Image 2024-03-16 à 11 12 30_8e713fb9](https://github.com/purplekan/S.P.A.R.K./assets/162813789/06a1ec63-34f9-4546-a001-493c2e0c38f2)

Il est important d'être méthodique et d'évoluer progressivement, c'est pourquoi nous avons commencé par nous réunir et proprement se définir en tant que groupe : V Team.  
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
| Mobilité de SPARK (Optionnel)          | Capacité de se déplacer de manière autonome pour accéder à différentes pièces ou zones.                                                      | Faible             |
| Livraison d'Objets (Optionnel) | Possibilité de transporter et de livrer des objets légers d'un endroit à un autre.                                                           | Faible            |

Une fois ces fonctionnalités clairement définies, nous sommes passés aux choix de composants nécessaires à l'implémentation des fonctionnalités. 

## 3. Liste du matériel
---
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
La modélisation du boîtier de S.P.A.R.K. n'a pas été de tout repos. En effet, après avoir décidé de la forme générale de notre robot, nous avons fais les esquisses des principales faces de ce boîtier. Il faut dire que c'était une première expérience pour nous, surtout que cela demandait des bases en dessin technique afin d'avoir un résultat potable.  
C'est non sans mal que nous sommes parvenus en quelque sorte à la face principale de S.P.A.R.K. Voyez plutôt par vous même :  
![WhatsApp Image 2024-03-16 à 13 03 51_c4468697](https://github.com/purplekan/S.P.A.R.K./assets/162813789/67f42845-9552-4efc-916a-84e16ef20593)

C'est très loin du niveau attendu d'un étudiant en prépa, mais je crois fermement que le plus important dans une représentation c'est que tous les détails y figurent. Après tout, le dessin peut etre arrangé.  
Je vous laisse entrevoir ce que c'est devenu une fois modélisé : 
![image](https://github.com/purplekan/S.P.A.R.K./assets/162813789/7f0a8d09-e304-4d0e-abe2-646b47bf58c4)  

J'en profite pour préciser que nous avons travaillé sur la version éducative de Fusion 360.
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
![Capture d'écran 2024-03-21 215242](https://github.com/purplekan/S.P.A.R.K./assets/162813789/f03192f5-db98-404a-9f2a-e9a4bc75c936)


## b. Début des hostilités 
Une fois débloqué et déterminé à finir ce modèle, je me suis heurté à un nouveau mur : comment vais-je gérer la mise en place des élémments dans le boîtier ? Comment vais je pouvoir rendre le boîtier ouvrable ?  
J'ai finalement opté pour un système de vis et j'ai continué à suivre le tutoriel avec beaucoup d'interruptions car je travaillais aussi durant le cours pour gagner du temps.  
Petit à petit, les esquisses que l'on a réalisé etaient enfin modélisées.  
Le modèle de base est maintenant fin prêt, mais il continuera à être modifié pour des raisons d'esthétique ou d'efficacité. D'ailleurs, je viens à nouveau de le modifier:  
![image](https://github.com/purplekan/S.P.A.R.K./assets/162813789/a4c46916-6948-463a-8736-007cda0caff2)  
  
De retour après deux jours de bataille, après des soucis que nous avons rencontré au niveau des circuits et dont je parlerais un peu plus tard, la boîte a dû être refaite et adaptée à la nouvelle configuration :  
  
![Capture d'écran 2024-03-21 125641](https://github.com/purplekan/S.P.A.R.K./assets/162813789/3bcc2cbe-f0b8-413c-94ef-c1207aab03a2)    
 
  
![Capture d'écran 2024-03-21 125726](https://github.com/purplekan/S.P.A.R.K./assets/162813789/be9c5626-6536-4ddb-ad2b-b5251770baab)


## 3. Circuits
## a. L'alarme ⏰ 
Nous avons commencé par la fonctionnalité de base de SPARK, celle qui lui permet de se comporter comme une alarme. Pour ce faire, nous avons suivi un certain nombre d'étapes afin de progressivement réussir :
- faire sonner le buzzer
- arrêter le son en appuyant sur un bouton
- implémenter le bouton reset pour réintinialiser l'alarme
- pouvoir récupérer une heure exacte à partir du RTC
- faire sonner l'alarme(le buzzer) à une heure précise et pouvoir l'arrêter à ce moment.
Vous pourrez retrouver le code dans le dossier documentation.
En ce qui concerne le fonctionnement, c'est assez simple. Une constante "state" est créée. C'est elle qui détermine si le buzzer émettra le son ou non.
Si l'heure prévue arrive, "state" prends la valeur 0 et le buzzer sonne. Si par contre l'on appuie sur le bouton d'arrêt, "state" prends la valeur 1 et le buzzer s'arrête. 
https://github.com/purplekan/S.P.A.R.K./assets/162813789/803af92f-aba5-456c-b046-8ecc90c4031f


## b. L'écran 🖥 
Toutes nos tentatives d'utiliser l'écran LCD avec l'I2C se sont soldées par des échecs. C'est certainement ce qui nous a le plus perdu de temps. En fin de compte, nous n'avons pas réussi à déterminer si le problème venait de l'écran, de l'I2C, du code ou des soudures faites. Nous avons dû nous rabattre sur l'écran LCD purement, ce qui a compliqué les câblages et nous a obligé à revoir les mesures du boîtier. Sur l'écran sera affiché la date et l'heure actuelle. 
Lorsque l'alarme sonnera, l'écran affichera la tâche associée à cette heure une fois l'alrme désactivée.

## c. Le joystick analogique 🕹 
Aussi connu sous le nom de HW 504, c'est ce petit bijou qui servira à naviguer entre les diffférentes tâches 
![HW504_B_back](https://github.com/purplekan/S.P.A.R.K./assets/162813789/cbcde223-0892-4bf4-aa78-3fba7d4e18a3)

## d. Le Real Time Clock 🕒 DS1302
En utilisant les bibliothèques <ThreeWire.h> et <RtcDS1302.h>, nous sommes en mesure de récupérer l'heure et la date précise au moment du téléversement. Cependant je ne sais pas si le RTC se base sur l'heure de l'ordinateur 🖥 ou le GMT.  
```python
if (now.Hour() == X & now.Minute() == Y & now.Second() == Z)
```   
nous permet de créér une condition avec une heure spécifique. Nous aurions aussi pu ajouter la date.
C'est ce que l'on fera pour notre liste de tâches à afficher : des paramètres pour l'heure et la date de sorte que chaque tâche a des valeurs bien définies.  

# III- Fonctionnement de S.P.A.R.K.
## 1. Diagramme de flux de l'alarme 
```mermaid
graph TD;
    A[Associer une tâche à une heure précise] --> B{Heure programmée atteinte ?};
    B -->|Oui| C[Déclencher l'alarme];
    C --> D[Effacer l'écran];
    D --> E[Afficher la tâche associée];
    E --> F[Attendre l'appui sur le bouton poussoir d'arrêt];
    F --> G[Arrêter l'alarme];
    G --> H[Afficher la prochaine tâche pendant 10 secondes];



    H --> I[Effacer l'écran];
    I --> J[Afficher l'heure et la date actuelles];
    B -->|Non| B;


```
Comment est ce que ça marche ?  
---
A l'aide du module RTC DS1302, nous nous assurons dans un premier temps de récupérer l'heure avec précision. On vérifie ensuite si l'heure actuelle correspond à l'heure définie pour la tâche.  

Si c'est le cas, cela déclenche l'alarme, affiche la tâche associée sur l'écran LCD. Lorsqu'on appuie sur le bouton poussoir d'arrêt, l'alarme s'arrête, la prochaine tâche est affichée pendant dix secondes et enfin, la date et l'heure actuelles. Notons qu'il y a un intervalle d'une minute entre les vérifications.

## 2. Diagramme de flux de la naviguation entre les tâches 
```mermaid
graph TD;
    A[Afficher la tâche] --> B{Déplacement du joystick vers le bas ?};
    B -->|Oui| C[Afficher la tâche suivante];
    C --> D;
    D --> E{Valeur de X négative et bouton enfoncé ?};
    E -->|Oui| F[Retour à la page d'accueil];
    F --> G[Effacer l'écran];
    G --> H[Afficher la date et l'heure];
    E -->|Non| D;
    B -->|Non| I{Valeur de X positive et bouton enfoncé ?};
    I -->|Oui| J[Supprimer la tâche actuelle];
    J --> K[Afficher la tâche précédente ou suivante];
    I -->|Non| B;
```

Que se passe t-il lorsqu'on veut défiler les tâches vers le bas ?
---
 L'utilisateur peut naviguer entre les tâches à l'aide du joystick analogique (HW 504).
 Lorsque l'utilisateur glisse le joystick vers le bas, la tâche suivante est affichée.
 Lorsque la valeur X du joystick est négative et le bouton du joystick est enfoncé, la fonction "retour" est activée :
   - L'écran est effacé.
   - La page d'accueil, affichant la date et l'heure, est affichée.
   
Lorsque la valeur X du joystick est positive et le bouton du joystick est enfoncé, la fonction "supprimer" est activée :
   - La tâche actuellement affichée est effacée de l'écran.
   - La tâche précédente ou suivante est affichée, selon le mouvement du joystick.

# Programme Arduino et explication
# I. Cas avec l'écran LCD
## 1. Fonction Accueil() 🕰️
## a. Code arduino 
```python
void Accueil() {
  RtcDateTime now = Rtc.GetDateTime();
  // Afficher la date et l'heure actuelles sur l'écran LCD
  lcd.clear();
  lcd.setCursor(0, 0);
  lcd.print(now.Day());
  lcd.print("/");
  lcd.print(now.Month());
  lcd.print("/");
  lcd.print(now.Year());
  lcd.setCursor(0, 1);
  lcd.print(now.Hour());
  lcd.print(":");
  lcd.print(now.Minute());
  lcd.print(":");
  lcd.print(now.Second());
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Récupération de la date et heure actuelles];
    B --> C[Affichage de la date et l'heure sur l'écran LCD];
    C --> D[Fin];
```
## 2. Fonction Gestion() 📜
## a. Code arduino
```python
void Gestion() {
 RtcDateTime now = Rtc.GetDateTime();
 if(now.Hour() == 7 & now.Minute() == 29 & now.Second() == 54) {
  Tache = Tache_1;
 } else if(now.Hour() == 9 & now.Minute() == 44 & now.Second() == 54) {
  Tache = Tache_2;
 } else if(now.Hour() == 13 & now.Minute() == 14 & now.Second() == 54) {
  Tache = Tache_3;
 } else {
  //
 }
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Récupération de l'heure actuelle];
    B --> C[Vérification de l'heure];
    C -->|Heure spécifique?| D[Affectation de la tâche correspondante];
    C -->|Non| E[Fin];
    D --> E[Fin];

```
## 3. Fonction Afficher() 🖥️
## a. Code arduino
```python
void Afficher(String tache) {
  // Effacer l'écran LCD
  lcd.clear();
  
  // Afficher la tâche sur l'écran LCD
  lcd.setCursor(0, 0);
  lcd.print(tache);
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Effacer l'écran LCD];
    B --> C[Afficher la tâche sur l'écran LCD];
    C --> D[Fin];
    D --> A;

```
## 4. Fonction afficherTacheSuivante() ➡️
a. Code arduino 
```python
void afficherTacheSuivante() {
  Gestion();
  if (Tache == Tache_1) {
    Afficher(Tache_2);
  } else if (Tache == Tache_2) {
    Afficher(Tache_3);
  } else if (Tache == Tache_3) {
    Afficher(Tache_1);
  } else {
    //
  }
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Gestion des tâches];
    B --> C{Tâche == Tache_1?};
    C -->|Oui| D[Afficher Tache_2];
    C -->|Non| E{Tâche == Tache_2?};
    E -->|Oui| F[Afficher Tache_3];
    E -->|Non| G[Afficher Tache_1];

```
## 5. Fonction supprimer() ❌
## a. Code arduino 
```python
void supprimer() {
  // Effacer la tâche actuellement affichée sur l'écran LCD
  lcd.clear();
  afficherTacheSuivante();
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Effacement de l'écran LCD];
    B --> C[Appel de la fonction afficherTacheSuivante];
    C --> D[Fin];
```
## 5. Fonction sonnerie() 🔔 
## a. Code arduino 
```python
void sonnerie() {
  // Déclencher l'alarme en mettant la sortie du buzzer à HIGH
  digitalWrite(Buzzer, HIGH);

  // Attendre jusqu'à ce que le bouton poussoir soit enfoncé pour arrêter l'alarme
  while (digitalRead(Arret) == LOW) {
    delay(100); // Attendre 100 ms avant de vérifier à nouveau l'état du bouton poussoir
  }

  // Arrêter l'alarme en mettant la sortie du buzzer à LOW
  digitalWrite(Buzzer, LOW);
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Déclenchement de l'alarme];
    B --> C[Attente d'appui sur le bouton pour arrêter l'alarme];
    C --> D[Arrêt de l'alarme];
    D --> E[Fin];

```
## 5. Void loop() 🧑‍💻
## a. Code arduino 
```python
void loop() {
  RtcDateTime now = Rtc.GetDateTime();
  ValeurX = analogRead(joyX);
  ValeurY = analogRead(joyY);
  // Gestion des tâches
  Gestion();

  // Si l'heure correspond à une tâche spécifique
  if (now.Hour() == 7 && now.Minute() == 29 && now.Second() == 54) {
    // Afficher la tâche et sonner l'alarme
    Afficher(Tache);
    sonnerie();
    Afficher(Tache_2);
    // Attendre pendant 10 secondes avant d'afficher la tâche suivante
    delay(10000);
  } else if (now.Hour() == 9 && now.Minute() == 44 && now.Second() == 54) {
    Afficher(Tache);
    sonnerie();
    Afficher(Tache_3);
    delay(10000);
  } else if (now.Hour() == 13 && now.Minute() == 14 && now.Second() == 54) {
    Afficher(Tache);
    sonnerie();
    Afficher(Tache_1);
    delay(10000);
  }
  // Afficher la date et l'heure 
  Accueil();
  if (ValeurY == 1) {
    // Afficher la tâche suivante
    afficherTacheSuivante();
  }

  // Si la valeur X du joystick est négative et le bouton du joystick est enfoncé
  if (ValeurX == 1 && digitalRead(HW) == HIGH) {
    // Activer la fonction "retour"
    retour();
  }

  // Si la valeur X du joystick est positive et le bouton du joystick est enfoncé
  if (ValeurX == 1040 && digitalRead(HW) == HIGH) {
    // Activer la fonction "supprimer"
    supprimer();
  }
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Récupération de la date et heure actuelles];
    B --> C[Gestion des tâches];
    C --> D[Condition heure spécifique ?];
    D -->|Oui| E[Affichage de la tâche et sonnerie];
    E --> F[Attente];
    F --> G[Affichage de la tâche suivante];
    G --> H[Fin];
    D -->|Non| I[Affichage de l'accueil];
    I --> J[Condition déplacement joystick vers le bas ?];
    J -->|Oui| K[Affichage tâche suivante];
    K --> L[Fin];
    J -->|Non| M[Condition joystick déplacé vers le haut et bouton enfoncé ?];
    M -->|Oui| N[Retour];
    N --> O[Fin];
    M -->|Non| P[Condition joystick déplacé vers le bas et bouton enfoncé ?];
    P -->|Oui| Q[Supprimer];
    Q --> R[Fin];
    P -->|Non| S[Fin];

```
# II. Cas avec LCD + I2C
## 1. Afficher la date et l'heure 
## a. Code Arduino
```python
#include <Wire.h> 
#include <LiquidCrystal_I2C.h>
#include <ThreeWire.h>
#include <RtcDS1302.h>

LiquidCrystal_I2C lcd(0x27, 16, 2);  // set the LCD address to 0x27 for a 16 chars and 2 line display
ThreeWire myWire(3, 6, 5); // DAT, CLK, RST
RtcDS1302<ThreeWire> Rtc(myWire);

void setup()
{
  Serial.begin(9600); // Initialise la communication série
  lcd.init();                      // initialize the lcd 
  lcd.backlight();
  Rtc.Begin();
  RtcDateTime currentTime = RtcDateTime(__DATE__,__TIME__);
  Rtc.SetDateTime(currentTime);

  // Affiche les informations de démarrage dans le moniteur série
  Serial.println("Initialisation terminée.");
  Serial.print("Date et heure actuelles : ");
  Serial.print(currentTime.Year());
  Serial.print("-");
  Serial.print(currentTime.Month());
  Serial.print("-");
  Serial.print(currentTime.Day());
  Serial.print(" ");
  Serial.print(currentTime.Hour());
  Serial.print(":");
  Serial.print(currentTime.Minute());
  Serial.print(":");
  Serial.println(currentTime.Second());
}
void afficherHeure() {
  RtcDateTime currentTime = Rtc.GetDateTime(); // Obtention de l'heure actuelle

  // Effacer la ligne précédente
  lcd.setCursor(0, 0);
  lcd.print("                "); // Effacez la ligne avec des espaces

  // Afficher l'heure sur l'écran LCD
  lcd.setCursor(0, 0); // Positionnez le curseur au début de la ligne
  lcd.print("Heure : ");
  lcd.print(currentTime.Hour()); // Afficher l'heure
  lcd.print(":");
  lcd.print(currentTime.Minute()); // Afficher les minutes
  lcd.print(":");
  lcd.print(currentTime.Second()); // Afficher les secondes

  //Affiche la date
  // Effacer la ligne précédente
  lcd.setCursor(0, 1);
  lcd.print("                "); // Effacez la ligne avec des espaces
  // Afficher la date sur l'écran LCD
  lcd.setCursor(0, 1); // Positionnez le curseur au début de la ligne
  lcd.print("Date : ");
  lcd.print(currentTime.Day()); // Afficher l'heure
  lcd.print(":");
  lcd.print(currentTime.Month()); // Afficher les minutes
  lcd.print(":");
  lcd.print(currentTime.Year()); // Afficher les secondes

  // Affiche les informations de l'heure actuelle dans le moniteur série
  Serial.print("Heure actuelle : ");
  Serial.print(currentTime.Hour());
  Serial.print(":");
  Serial.print(currentTime.Minute());
  Serial.print(":");
  Serial.println(currentTime.Second());

  delay(500); // Attendre une seconde avant de mettre à jour l'écran LCD
}
void loop() {
  afficherHeure();
}
```
## b. Diagramme de flux
```mermaid
graph TD;
    A[Début] --> B[Initialisation];
    B --> C[Initialisation de la communication série];
    C --> D[Initialisation de l'écran LCD];
    D --> E[Activation du rétroéclairage];
    E --> F[Initialisation du module RTC];
    F --> G[Récupération de l'heure actuelle];
    G --> H[Affichage de l'heure sur l'écran LCD];
    H --> I[Affichage de la date sur l'écran LCD];
    I --> J[Affichage des informations dans le moniteur série];
    J --> K[Attente de 500 millisecondes];
    K --> G;

```
# ino Spark

Nous avons finalement pu régler le soucis que nous avions avec l'I2C, en plus d'un souci de cablage avec le RTC nous sommes enfin parvenus à finaliser les parties importantes du code. Il ne reste plus qu'à importer les fonctions déjà vues plus haut.
Gardez à l'esprit que le problème peut venir d'un mauvais cablage ou d'un composant donc aidez vous de votre moniteur série pour vérifier ce qui s'affiche sur l'écran LCD 

```cpp
#include <Wire.h> 
#include <LiquidCrystal_I2C.h>
#include <ThreeWire.h>
#include <RtcDS1302.h>

#define Buzzer 2
#define Arret 4
LiquidCrystal_I2C lcd(0x27, 16, 2);  // set the LCD address to 0x27 for a 16 chars and 2 line display
ThreeWire myWire(3, 6, 5); // DAT, CLK, RST
RtcDS1302<ThreeWire> Rtc(myWire);
const int HW = 52;
const int joyX = A0;
const int joyY = A1;
int ValeurX ;
int ValeurY ;
String Tache_1 = "Automatique";
String Tache_2 = "Electronique";
String Tache_3 = "Electromagnetisme";
String Tache = Tache_1;

void setup()
{
  Serial.begin(9600); // Initialise la communication série
  lcd.init();                      // initialize the lcd 
  lcd.backlight();
  Rtc.Begin();
  RtcDateTime currentTime = RtcDateTime(__DATE__,__TIME__);
  Rtc.SetDateTime(currentTime);

  // Affiche les informations de démarrage dans le moniteur série
  Serial.println("Initialisation terminée.");
  Serial.print("Date et heure actuelles : ");
  Serial.print(currentTime.Year());
  Serial.print("-");
  Serial.print(currentTime.Month());
  Serial.print("-");
  Serial.print(currentTime.Day());
  Serial.print(" ");
  Serial.print(currentTime.Hour());
  Serial.print(":");
  Serial.print(currentTime.Minute());
  Serial.print(":");
  Serial.println(currentTime.Second());
}
void afficherHeure() {
  RtcDateTime currentTime = Rtc.GetDateTime(); // Obtention de l'heure actuelle

  // Effacer la ligne précédente
  lcd.setCursor(0, 0);
  lcd.print("                "); // Effacez la ligne avec des espaces

  // Afficher l'heure sur l'écran LCD
  lcd.setCursor(0, 0); // Positionnez le curseur au début de la ligne
  lcd.print("Heure : ");
  lcd.print(currentTime.Hour()); // Afficher l'heure
  lcd.print(":");
  lcd.print(currentTime.Minute()); // Afficher les minutes
  lcd.print(":");
  lcd.print(currentTime.Second()); // Afficher les secondes

  //Affiche la date
  // Effacer la ligne précédente
  lcd.setCursor(0, 1);
  lcd.print("                "); // Effacez la ligne avec des espaces
  // Afficher la date sur l'écran LCD
  lcd.setCursor(0, 1); // Positionnez le curseur au début de la ligne
  lcd.print("Date : ");
  lcd.print(currentTime.Day()); // Afficher l'heure
  lcd.print(":");
  lcd.print(currentTime.Month()); // Afficher les minutes
  lcd.print(":");
  lcd.print(currentTime.Year()); // Afficher les secondes

  // Affiche les informations de l'heure actuelle dans le moniteur série
  Serial.print("Heure actuelle : ");
  Serial.print(currentTime.Hour());
  Serial.print(":");
  Serial.print(currentTime.Minute());
  Serial.print(":");
  Serial.println(currentTime.Second());

  delay(500); // Attendre une seconde avant de mettre à jour l'écran LCD
}
void sonnerie() {
  // Déclencher l'alarme en mettant la sortie du buzzer à HIGH
  digitalWrite(Buzzer, HIGH);

  // Attendre jusqu'à ce que le bouton poussoir soit enfoncé pour arrêter l'alarme
  while (digitalRead(Arret) == LOW) {
    delay(100); // Attendre 100 ms avant de vérifier à nouveau l'état du bouton poussoir
  }

  // Arrêter l'alarme en mettant la sortie du buzzer à LOW
  digitalWrite(Buzzer, LOW);
}
void retour() {
  // Effacer l'écran LCD
  lcd.clear();
  Accueil();
}
void Afficher(String tache) {
  // Effacer l'écran LCD
  lcd.clear();
  
  // Afficher la tâche sur l'écran LCD
  lcd.setCursor(0, 0);
  lcd.print(tache);
}
void afficherTacheSuivante() {
  Gestion();
  if (Tache == Tache_1) {
    Afficher(Tache_2);
  } else if (Tache == Tache_2) {
    Afficher(Tache_3);
  } else if (Tache == Tache_3) {
    Afficher(Tache_1);
  } else {
    //
  }
}
void supprimer() {
  // Effacer la tâche actuellement affichée sur l'écran LCD
  lcd.clear();
  afficherTacheSuivante();
}

void loop() {
  afficherHeure();

}
```
# Sources

Pour réaliser ce projet, nous avons dû consulter de nombreux sites et regardé des vidéos entre le 09 mars 2024 et le 23 mars 2023.  
Voici les liens de nos sources : 
- https://youtu.be/tG9jZt7ZrME?si=-BvY9c8qf68NFwxF
- https://youtu.be/1n_KjpMfVT0?si=cqUgA5AprYfO4R6C
- https://youtu.be/8PMEe7VvovM?si=JuN84bVqriODaKHQ
- https://youtu.be/BCvXOPih2zo?si=nwH4i1jCNLBUO8hy
- https://youtu.be/uCCrLPmaa_w?si=lMIUktS_0-ToLvVI
- https://youtu.be/tG9jZt7ZrME?si=ldOMA3Ahjqu5gKYE
-  https://youtu.be/hHIIWpZcYNs?si=tB9dx_kWs098L-zI
-  https://youtu.be/1n_KjpMfVT0?si=P1G5ooKKE-DB9gqf
-  https://youtu.be/1n_KjpMfVT0?si=JuLWSnHzW6YHPFlO
-  https://youtu.be/MnzidiZ_6ok?si=XaeNTNJPcE1X0qT9
-  https://youtu.be/gGXvWD2qPPc?si=HnjCoWSxPj2zBdh9
-  https://youtu.be/AU9dxEcrVQ4?si=BhiTja3u5icZ2jBY
-  https://youtu.be/MfmK55TREuQ?si=Hx29F9dxczJMhF8B
-  https://youtu.be/2iFGNswJxo8?si=I4SY_IUFGSB-KXAu
-  https://youtu.be/Athue7Wkjog?si=zV58WzsB2grrPPpO
-  https://youtu.be/T85CoWZ_Zc8?si=1OjzBssnw8lvuH8N
-  https://youtu.be/MlDi0vO9Evg?si=0nFy7E1L4pnkOr4A
-  https://www.equascience.com/kits-d-experiences/5253-module-haut-parleur-pour-arduino.html
-  https://grabcad.com/library/lcd-display-5
-  https://grabcad.com/library/hw-504-joystick-1
-  https://grabcad.com/library?page=1&time=all_time&sort=recent
-  https://grabcad.com/library/micro-servo-sg-90-2
-  https://grabcad.com/library/lcd-display-1602a-1
-  https://www.moussasoft.com/bouton-poussoir-arduino
-  https://forum.arduino.cc/t/comment-faire-un-bouton-reset-sur-un-projet-resolu/639784/6
-  https://fr.vittascience.com/learn/tutorial.php?id=224#:~:text=sera%20ajout%C3%A9%20prochainement%5D-,Utilisation%20de%20l%27afficheur%20LCD,Attention.
-  https://zestedesavoir.com/tutoriels/686/arduino-premiers-pas-en-informatique-embarquee/748_laffichage-une-autre-maniere-dinteragir/3443_les-ecrans-lcd/
-  https://ledisrupteurdimensionnel.com/arduino/comment-relier-lecran-lcd-a-l-arduino-uno/
-  https://rtmfm.cnrs.fr/wp-content/uploads/2022/01/Tutoriel-10-Arduino-programme-ecran-LCD.pdf
-  https://github.com/TechKrowd/ArduinoLCD/blob/master/LCD_1602A.ino
-  https://forum.arduino.cc/t/lcd-16x2-pcf8574t-black-boxes-problem/241702/2
-  https://exploreembedded.com/wiki/Analog_JoyStick_with_Arduino
-  https://grabcad.com/library/adafruit-perma-proto-full-sized-breadboard-pcb-1
-  https://grabcad.com/library/rtc-ds1302-2
-  https://grabcad.com/library/buzzer-kls3-mt-09-1
-  https://youtu.be/83E3qum343k?si=5HMfTAawIBvblHVd
-  https://youtu.be/lJ4zk4b8dds?si=otElqShIFQyFtLrc

# Remerciements 
Nous tenons à remercier quelques personnes pour nous avoir aidé directement ou non à réaliser S.P.A.R.K. :  
-  [M. OLANLO](https://www.linkedin.com/in/sylvestre-olanlo-9b7229186?miniProfileUrn=urn%3Ali%3Afs_miniProfile%3AACoAACvQ3FsBNHHTQC275Wll1vGHQk_kiTAp59o&lipi=urn%3Ali%3Apage%3Ad_flagship3_search_srp_all%3BRNbL%2F3UYTYuJH7%2FecRM28Q%3D%3D), [M. HANKEM](https://www.linkedin.com/in/justin-hankem-a97491175?miniProfileUrn=urn%3Ali%3Afs_miniProfile%3AACoAACmKJdMBky3_1KcOlS4GcgkNzIFx4lNP15c&lipi=urn%3Ali%3Apage%3Ad_flagship3_search_srp_all%3B%2FdqMAqcaRUaRa7KMyVoOKw%3D%3D), [M. KAMEKPO](https://www.linkedin.com/in/komlan-giovanni-kamekpo-3571b920a/), [M. BAKAI](https://www.linkedin.com/in/josaphat-bakai-0b1261253?miniProfileUrn=urn%3Ali%3Afs_miniProfile%3AACoAAD6B9UUBkkrP2BP6diubeUNhCdbg9BukLYQ&lipi=urn%3Ali%3Apage%3Ad_flagship3_search_srp_all%3Bc%2BinFkysRoWHiJm0Ol6gdw%3D%3D) pour nous avoir encadré par leurs bons conseils et pour nous avoir donné l'opportunité de participer à cet événement
-  [M. LEENAERTS](https://github.com/THE07s/GarderMapBot.git) et [M. ATADEGNON](https://github.com/9Pierrot/Espace_de_travail_phoenix.git) pour leurs conseils au sujet du code arduino, de la modélisation ainsi qu'au niveau de la documentation
-  Toute la communauté Arduino, en particulier vous qui avez mis vos découvertes à disposition de vos pairs

Nous sommes heureux d'appartenir à cette communauté de passionés et espérons fortement que par notre projet, d'autres trouveront la motivation d'en faire autant.








