# MyComps Project

## Présentation

MyComps Project est un projet pour la gestion de compétences dans une equipe. Il a pour but de gamifier le suivit de l'évlotion des niveaux de compétences pour les personnes d'une équipe.

## Tesorus
* Compétence: Une compétence est un connaissance sur une technologie, un concepte ou autre.
* Niveau de compétence: Représente sur 20 le niveau de connaissance d'une compétence.
    |Niveau| Nom du niveau | materiel | description                  |
    |------|---------------|----------|------------------------------|
    |     0| Non Initié    | chocolat | Ne connait pas la compétence |
    |     1| Non Initié    | chocolat | A deja entendu parler de la compétence mais ne sais pas ce qu'elle fait. |
    |     2| Non Initié    | chocolat | A deja entendu parler de la compétence mais son utilité est encore flou |
    |     3| Non Initié    | chocolat | A deja entendu parler de la compétence et connais son principe dans les grande lignes |
    |     4| Non Initié    | chocolat | A deja entendu parler de la compétence et connait son but mais n'a jamais vu comment elle marche |
    |     5| Débutant      | Bronze   | Connait la compétence mais na jamais essayé |
    |     6| Débutant      | Bronze   | Connait la compétence mais na vu que les bases que rapidement |
    |     7| Débutant      | Bronze   | Connait la compétence mais et connait un peu les bases |
    |     8| Débutant      | Bronze   | Connait la compétence mais n'ai pas encore alaise avec les bases|
    |     9| Débutant      | Bronze   | Connait la compétence et ses bases mais n'est pas alaise |
    |    10| Connaisseur   | Silver   | Connait la compétence et ses bases |
    |    11| Connaisseur   | Silver   | Connait la compétence et est capable de faire les bases en autonomie |
    |    12| Connaisseur   | Silver   | Connait la compétence et est capable d'aller un peu plus loin |
    |    13| Connaisseur   | Silver   | Connait la compétence et est autonome sur son utilisation |
    |    14| Connaisseur   | Silver   | Connait bien la technologie |
    |    15| Expert        | Gold     | Peut utiliser la compétence pour des élements avancé |
    |    16| Expert        | Gold     | Peut utiliser la compétence pour des élements expert |
    |    17| Expert        | Gold     | Connait les cencepts les plus avancé de la technologie |
    |    18| Maitre        | Diaman   | Maitrise la technologie. Est alaise avec tout ses concepts |
    |    19| Maitre        | Diaman   | Serait capable d'expliquer comment la compétence a pu etre créer... Maitrise Total |
    |    20| Créateur      | Diaman   | A créer la technologie. |
* Famille de compétence: Représentate une famille regroupant des compétences et autre famille.
    - Par exemple La famille Langage Java regroupe: Java algorithmie, Java POO, Java Avancé, Java Expert.
    - Par exemple La famille Environement Java regroupe: Famille Langage Java, Framework Spring, Maven, Gradle, Configuration JVM
* Niveau de famille de compétence: Correspond a la somme des niveaux de compétences de ses enfants.
* Classe : Regroupement de compétence et famille représentant une Classe. Un Classe definie des régles pour son niveau. Par exemple le Classe développeur backend débutant demande de connaitre 2 langages de programmations au niveau 10, un framework backend au niveau 10, la compétence git au niveau 10 ...
* Tag: permet d'identifier une compétence, faille ou Classe. 
    - Par exemple Java posséde les tags: Langages, Backend, POO, JVM
* Médaille: Une médaille récompense les personnes ayant le plus haut niveau de compétence sur une compétence précise:
    - Or : premier
    - Argent: deuxieme
    - Bronze: troisieme
* Journal d'évolution: permet de voir l"evolution du niveau d'une personne.
* Régles de connaissance: Les compétences ne peuvent pas etre apprise dans n'importe qu'elle ordre. Il est possible d'y mettre des régles:
    * Régle débloqué Si: Débloque la compétence si vous répondez a la régle enfant.
    * Régle Niveau possible Si: Autorise le niveau si vous répondez a la régle enfant.
    * Régle Au moins une parmit: Est réspecter si vous répondez a l'une des sous régles.
    * Régle Tous: Est réspecter si vous respécter l'ensemble des sous régles.
    * Régle niveau minimum: Est réspecter si votre niveau est au minimum.
    * Régle validation par les pair: Est réspecter si un validateur valide le niveau de compétence.
    * Régle débloque Validation: Permet au joueur de devenir Validateur pour cette compétence.

* Mentor: Utilisateur pouvant definir le niveau de compétence et le niveau de compétence cible d'une personne.
* Validateur: utilisateur possédant pouvant valider la monté en niveaud e compétence d'une personne.
* Objectif: definie un niveau de compétence acquerir avant une certaine echehance.
* Selectionneur: Utilisateur n'ayant pas de competence mais voyant les compétences de l'ensemble (Lindsay)
* Joueur: Utilisateur avec des niveau de compétence.
* Marqueurs: permet de notifier aux utilisateur q'une compétence a un quelque chose de plus.
    * Marqueurs d'interet: Permet a un joueur de definir une compétence comme interessante pour lui.
    * Marqueurs d'utilité: permet a un mentor de definir une compétence comme interessante pour un joueur.
    * Marqueurs de manque: La compétence est sous représenté dans l'équipe par rapport aux besoins.
    * Marqueurs d'objectif: La compétence fait partie d'un objectif.

## Personna et roles:
* Joueur: Utilisateur ayant des compétences et pouvant suivre son évolution. Pour lui l'outil permet de suivre son évolution, de connaitre le niveau de ses mates (autres joueur), de definir des compétence comme intéressante, de voir les compétences qu'il peut apprendre, voir les besoins
* Selectionneur: joueur ou non, il peut voir l'ensemble des compétences des joueurs.
* Mentor : Peut suivre l'evolution d'un ou plusieurs autre joueurs. Il peut aussi definir des compétence comme objectif.
* Validateur: Peut valider l'evolution d'une personne sur une compétence.
* Game Master : Peut créer des compétences, famille et role et peut configurer les régles.

## Les besoins

### Pour les joueurs
* Un joueur PEUT definir (up, down) son niveau sur les compétences qui lui son disponible en fonction des regles.
* Un joueur PEUT voir les autre joueurs et leurs niveau sur une compétence.
* Un joueur PEUT definir une compétence comme interessante.
* Un joueur commence avec un niveau de 0 sur toutes ses compétence.
* Un joueur PEUT choisir un ou plusieurs role a suivre.
* Un joueur PEUT voir son classement sur une technologie.
* Un joueur PEUT rechercher une compétence.
* Un joueur PEUT voir les régles necessaire pour asquerir un niveau de role ou de compétence.
* Un joueur PEUT voir le récapitulatif de l'équipe.
* Un joueur PEUT voir son journal d'evolution.
* Un joueur NE PEUT PAS voir le journal d"volution des autres joueurs s'il n'est pas Selectionneur ou Mentor.
* Un joueur PEUT voir l'etat de ses demande de validation en attente.
* Un joueur PEUT voir l'ensemble des compétence ou il est validateur.

### Pour les Selectionneur
* Un Selectionneur PEUT voir le niveau de compétence, famille et role de tout les joueurs.
* Un Selectionneur PEUT rechercher une compétence et voir qui sont les personnes ayyant le plus haut niveau.
* Un Selectionneur PEUT definir une compétence comme en manque grace a un marqueur.
* Un Selectionneur a acces au journal d'évolution de l'ensemble des joueurs.

### Pour les Mentors
* Un Mentor PEUT definir une compétence comme d'utilité pour un des joueurs qu'il mentor.
* Un Mentor a acces au journal d'évolution des joueurs qu'il mentor.
* Un Mentor PEUT changer le niveau d'un joueur qu'il mentor.
* Un Mentor PEUT voir la liste des joueurs qu'il mentor.
* Un Mentor PEUT definir les objectif d'un de ses joueurs.

### Validateur:
* Un Validateur PEUT voir l'ensemble des validations des joueurs en attente q'uil peut valider.
* Un validateur PEUT valider ou non une demande de validation s'il est validateur dessus.
* Un Validateur PEUT avoir les informations de contact d'une personne qui demande une validation.

### Game Master
* Un GM PEUT créer, mettre a jour ou supprimer une compétence, famille ou role.
* Un GM PEUT créer, mettre a jour ou supprimer une régle sur une compétence.
* Un GM PEUT créer un nouvelle utilisateur et lui affecter un role.

## Choix des technologies:

### Front: 
* Framework: React
* Langage: TS
* Structure: Classique, MonoProject
* Tests: Jest
* Provider HTTP: Nginx

### Back:
* Framework: SpringBoot
* Language: Java
* Structure: Microservice Clean Archi
* Tests : JUnit TDD 100% Service
* BDD: MongoDB

### GateWay:
* SpringGateway

### Sécurité:
* A definir...

## UseCase

### Premiére connsion pour un simple joueur.
1. Login
2. Choisie son niveau pour les compétences sans regles.
3. Choisie son niveau pour les compétences avec régles qu'il a pue débloqué jusqu'a ne plus avoir de compétences a remplir.
4. Arrive sur sa page d'acceuil et peut voir ses informations.
5. il peut alors:
    - Changer le niveau d'une de ses compétences.
    - Naviguer a travers les compétences pour voir le niveau des autres joueurs.
    - Marquer une compétences comme interessante.
    - voir ses objectifs.
### Mentor peut choisir un objectif:
1. Clique sur objectif.
2. Navigue a travers les technologies.
3. Clique sur un bouton (invisible pour les simple joueur) et peut choisir d'affecter un objectif a un joueur dont il est mentor.

### Validateur
1. Sur sa page d'acceuil il voit les validations qu'il peut valider
2. Peut vailider une demande de validation
3. Peut refuser en indiquant pourquoi.
4. Peut avoir les informations de contact du joueur faisant la demande.

### Selectionneur
1. Peut naviguer a travers les compétences.
2. Sur la page d'une compétence, peut cliquer sur un bouton pour la definir en manque.

### GM
1. A acces a une page permettant de créer une nouvelle compétence.

## Prio des features:
| Nom de la feature                | Prio | desscription |
|----------------------------------|------| ------------ |
| Systeme de compétence            | F1   | Page pour voir les informations d'une compétence |
| Systeme de profile joueur        | F2   | ... |
| Systeme de role                  | F3   | ... |
| Systeme de selectioneur          | F4   | ... |
| Systeme de mentor                | F5   | ... |
| Systeme de médaille              | F6   | ... |
| Systeme de régles                | F7   | ... |
| Systeme de validation            | F8   | ... |