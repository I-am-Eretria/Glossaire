

# GLOSSAIRE 🔍


## - Sommaire - ##

- [Général](#général)  -  001 à 017
  
- [Front-end](#front-end) -  018 à 034
 
- [UX / UI](#ux-ui) - 035 à 042
 
- [Programmation orientée objet](#programmation-orientée-objet-poo) - 043 à 059 
  
- [Architecture](#architecture) - 060 à 066 
 
- [Modélisation / Base de données](#modélisation---base-de-données) - 067 à 083 
  
- [Symfony](#symfony) - 084 à 093 
  
- [Sécurité](#sécurité) - 094 à 103 
  
- [RGPD](#rgpd) - 104 à 113 
  
- [SEO](#seo) - 114 à 126 
  
- [Gestion de projets / DevOps](#gestion-de-projets---devops) - 127 à 142 
  
- [English](#english) - ??? à ??? 

<br>
<br>

## Général

<br>

### 1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte.

Pour exécuter un script PHP, il est nécessaire d'avoir un serveur HTTP (par exemple Apache) associé à un interpréteur PHP. Dans le cas contraire,  le code de toute la page sera affiché tel quel tout simplement car un navigateur n’est pas capable de comprendre ni d’exécuter du code PHP sans l'environnement adéquat.

Logiciels (gratuits) pouvant être utilisés :
- Laragon : Un environnement regroupant les serveurs Apache HTTP Server, PHP et MySQL.
- XAMPP : Une distribution Apache comprenant MySQL, PHP, et Perl.

<br>
<br>

### 2.	Qu’est-ce qu’un algorithme ?  

Algorithme: suite finie et ordonnée d'instructions qui, une fois exécutée correctement, conduit à la résolution d'un problème initial.

<br>
<br>

### 3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?

Variable: boîte identifiée par le programme via son étiquette (nom unique) pour stocker une valeur ou un ensemble de données. Pour accéder à cette boîte, il nous faudra donc la désigner par son étiquette.

En PHP, une variable est préfixée par le symbole $. 
    
<ins>Exem</ins><ins>ple</ins>: $etiquette = "valeur";    } Variable   

<br>
<br>

4.	Qu’est-ce que la portée d’une variable ?

<br>
<br>

### 5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?

Constante : Les constantes sont des variables spécifiques dans le sens où leurs contenus resteront inchangés tout au long du traitement, à l'inverse d'une variable qui verra son contenu être modifié. 

Elles sont définis avec le mot Const précédent leur nom.

Différence : Une variable peut changer de valeur pendant l'exécution du script contrairement à une constante qui elle reste identique.

<br>
<br>

6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation 
7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)
8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?
9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles
10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?
11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP
12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP
13.	Quelle est la différence entre les instructions « require » et « include » en PHP
14.	Comment effectuer une redirection en PHP ?
15.	Définir la partie « front-end » et « back-end » d’une application
16.	Définir le contrôle de version ? Qu’est-ce que Git ?
17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples

<br>
<br>

## Front-end

<br>

### 18.	Définir HTML

HyperText Markup Language ou HTML est un langage de balisage (ou marquage pour Markup) pour structurer et organiser le contenu d'une page web.

Le HTML se définit par des caractéristiques très claires :
- la syntaxe : elle commence toujours par une balise d’ouverture et est clôturée par une balise de fermeture (toutes deux entourées de chevrons)
- l'utilisation de balises : elles décrivent et structurent les éléments d’une page.

Enfin l'HyperText désigne les liens qui relient les pages web entre elles, que ce soit au sein d'un même site ou entre différents sites web. Les liens sont un aspect fondamental du Web. 

<br>
<br>

### 19.	Définir CSS

Cascading Style Sheets ou CSS est un langage de styles utilisé pour décrire l'apparence et le design des éléments HTML d'une page web.

Il permet de définir des règles de style (couleurs, marges, alignements, polices, etc) et de les appliquer à des éléments spécifiques (#id) ou à des ensembles d'éléments (.class) d'une page.

CSS utilise une structure en cascade, ce qui signifie que les styles peuvent se superposer et être hérités, donnant ainsi une grande flexibilité de personnalisation.

> [!IMPORTANT]
> Pour lier un fichier CSS à un fichier HTML, il faut systématiquement ajouter dans la balise `<head>` du fichier HTML une balise `<link>` :
> 
> `<link rel="stylesheet" href="ajouter ici le chemin de l'emplacement du fichier CSS">`
    

<br>
<br>

### 20.	Définir Javascript

JavaScript (JS) est un langage de programmation, orienté objet, principalement utilisé pour ajouter des fonctionnalités interactives et dynamiques aux pages web.

> [!NOTE]
> JavaScript est un langage côté client, mais il peut aussi être exécuté côté serveur, par exemple avec Node.js.

JavaScript permet de : 
- manipuler le navigateur et le DOM (Document Object Model)
- de réagir aux événements déclenchés par l'utilisateur (les clics, la saisie d'un formulaire, les actions de navigation, etc)
- de valider des formulaires
- et d’effectuer des requêtes asynchrones (il envoie la demande et continue son exécution en attendant la réponse).

> [!IMPORTANT]
> Pour lier un fichier JS à un fichier HTML, il faut systématiquement ajouter dans la balise `<body>` du fichier HTML une balise `<script>` :
> 
> `<script src="ajouter ici le chemin de l'emplacement du fichier JS"></script>`

<br>
<br>

### 21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 

JavaScript Object Notation ou JSON est un format de texte léger et facile à lire utilisé pour représenter des données structurées, similaire aux objets JavaScript (paire clé/valeur).
        
JSON est habituellement utilisé pour échanger des données sur des sites web.
     
<ins>Exem</ins><ins>ple</ins>: _envoyer des données depuis un serveur vers un client afin de les afficher sur une page web ou vice versa._

<br>
<br>

22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
23.	Qu’est-ce qu’un sélecteur CSS ?
24.	Quelle balise HTML permet de créer un lien hypertexte ?
25.	Qu’est-ce qu’une requête AJAX ?
26.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?
27.	Définir le responsive design
28.	Qu’est-ce que le templating ?
29.	Qu’est-ce qu’une fonction anonyme en Javascript ?
30.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?
31.	Qu’est-ce qu’un « media query » ?
32.	Qu’est-ce qu’un pseudo élément en CSS ?
33.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent
34.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes

<br>
<br>

## UX UI

<br>

### 35.	Quelle est la différence entre UX Design et UI Design ?

UX Design (User Experience Design) : Se concentre sur l’expérience globale de l’utilisateur lorsqu’il interagit avec un produit ou un service. Il englobe des aspects comme l’utilisabilité, l’ergonomie, l’accessibilité et la fluidité de navigation.
concevoir une interface accessible et facile à prendre en main pour tout type de support


UI Design (User Interface Design) : Se concentre sur l’aspect visuel et interactif de l’interface, comme les couleurs, les typographies, les boutons et les animations.

En résumé : l’UX concerne comment ça fonctionne, tandis que l’UI concerne à quoi ça ressemble.

> [!NOTE]
> UX Design est basé sur les besoins des utilisateurs.
> UI Design est basé sur la demande du client.

mettre un schéma pour illustrer différences

<br>
<br>

### 36.	Qu’est-ce qu’un wireframe ? 

Wireframe: signifie littéralement structure, cadre, ou modèle en fil de fer, souvent traduit par « maquette fonctionnelle ». C’est le squelette de la future interface des applications mobiles, sites web et logiciels. Quelle qu’en soit la définition, le Wireframe est toujours une maquette au graphisme simplifié.


Avantages :
- optimiser la conception d’une interface avec les fonctionnalités, sans être distrait par les éléments visuels/graphiques (couleurs, logos, etc)
- montrer la future interface de l’outil, à l’échelle réelle, aux parties prenantes et s’accorder ainsi sur le projet web ou mobile avant le développement
- repérer les erreurs ou les problèmes – UX Design et ergonomie – pour faire des itérations rapides, sans code ni programmation
- gagner du temps et de l’argent: le Wireframe est rapide à réaliser, peu coûteux en ressources, flexible, et permet de réduire les révisions en phase de développement.

<br>

image pour illustrer 

<br>
<br>

### 37.	Qu’est-ce qu’un prototype ? 

À l’inverse, le prototype en haute-fidélité est censé être une première version du produit final. Les idées essentielles ont été validées et il peut y avoir eu implémentation. On veut désormais tester l’efficacité et l’utilisabilité avant la sortie finale de l’application web / mobile. 

<br>

image pour illustrer 

<br>
<br>

### 38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?

La hiérarchie visuelle définit l’ordre d’importance des éléments d’une interface grâce à des repères visuels pour guider l’attention de l’utilisateur de manière intuitive.


Exemples de repères visuels : 
- tailles (titres plus grands que le texte courant)
- couleurs (éléments contrastants pour les actions principales)
- positionnement (éléments importants placés en haut ou au centre)
- échelle (taille relative des éléments)
- espacement (créer des groupements logiques d’éléments)
- typographie (utilisatiion de polices de différentes tailles et épaisseurs).

<br>
<br>


### 39.	Qu’est-ce que l’accessibilité en UX Design ? 

L'accessibilité est la pratique consistant à rendre les produits ou services disponibles et utilisables par le plus grand nombre d'utilisateurs possible, y compris ceux ayant des handicaps (visuels, auditifs, moteurs ou cognitifs).

Exemples d'accessibilité possibles :
- utiliser des contrastes suffisants pour le texte
- rendre les interfaces accessibles via clavier et lecteurs d’écran
- offrir des alternatives textuelles pour les images et vidéos
- garantir une navigation simplifiée.

> [!NOTE]
> Technologies utiles :
> ARIA (HTML), WAVE, LIGHTHOUSE.

> [!TIP]
> RGGA : Référentiel Général d'Amélioration de l'Accessibilité.
> Guide français des bonnes pratiques handi-friendly.
>
> WCAG : Règles pour l'Accessibilité des Contenus Web.
> Guide niveau international ayant pour but de fournir un standard unique commun handi-friendly.

<br>
<br>

### 40.	Qu’est-ce qu’une grille de mise en page ?

Une grille de mise en page (ou grid en anglais) est une structure composée de lignes verticales et horizontales invisibles qui organise et aligne les éléments visuels d’une interface. 

Avantages :
- assurer une cohérence visuelle
- faciliter la collaboration entre designers et développeurs
- améliorer l’esthétique et la lisibilité.

<br>
<br>

### 41.	Qu’est-ce que la notion d’affordance en UX Design ?

L’affordance désigne la capacité d’un élément à suggérer son usage. 

Exemples :
- un bouton avec une forme et une couleur spécifiques indique qu’il est cliquable
- une icône de poubelle dans un panier évoque l’action de suppression (d'un article par exemple).

Une affordance efficace rend l’interface intuitive, car les utilisateurs comprennent naturellement ce qu’ils peuvent faire.

> [!NOTE]
> Snapchat est une exception rare dans les applications mobiles qui fonctionnent, car son UX est de prime abord très déroutante : au départ on ne sait pas bien comment l'utiliser (= manque d'affordance).
> Snapchat s'ouvre directement sur la fonction appareil photo, quasiment rien n'est indiqué (peu de signifiant) et cela demande du temps pour comprendre comment l'utiliser :
> - action swipe dans un certain sens pour accéder à fonctionalité en particulier
> - appliquer plusieurs filtres à une même photo en gardant un doigt appuyé sur l'image et en swipant avec l'autre 
> - faire apparaître les masques animés en maintenant le doigt appuyé sur son visage.

<br>
<br>

### 42.	Qu’est-ce qu’un « mobile first design » ?

Le mobile first design est une approche de conception qui commence par le design pour les appareils mobiles avant de s’adapter aux écrans plus grands (tablettes, ordinateurs). 

Les principes clés :
- prioriser les fonctionnalités essentielles
- concevoir une interface simple et optimisée pour les petits écrans 
- utiliser des techniques comme le responsive design pour une adaptation fluide
- chargement rapide notamment même avec un réseau de mauvaise qualité 
- ne pas consommer trop d'énergie et donc de batterie.

> [!NOTE]
> Le moteur de recherche Google "punit" les sites non "responsives", c'est-à-dire qu'il pénalise en termes de référencement les sites non compatibles avec le mobile : ils ne remontent pas dans les résultats de recherche.

<br>
<br>

## Programmation orientée objet (POO)
43.	Donner une définition de la programmation orientée objet 
44.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?
45.	Qu’est-ce qu’un objet ?
46.	Définir la notion de propriété / attribut / méthode
47.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité
48.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?
49.	Qu’est-ce que l’encapsulation ?
50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple
51.	Définir l’opérateur de résolution de portée
52.	Définir une méthode / propriété statique
53.	Définir le polymorphisme en POO
54.	Définir une méthode / classe abstraite ?
55.	Définir le chaînage de méthodes
56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »
57.	Qu’est-ce qu’un « autoload » ?
58.	Comment appelle-t-on en français les « getters » et les « setters » ?
59.	Qu’est-ce que la sérialisation en PHP ? 

## Architecture 
60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence
61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
62.	Qu’est-ce que l’architecture MVC ?
63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
64.	Quels sont les avantages de l’architecture MVC ?
65.	Existe-t-il des variantes à l’architecture MVC ?
66.	Qu’est-ce qu’une API ? Définir l’architecture REST

## Modélisation - Base de données
67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise
68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
a.	Analyse, conception et réalisation
b.	Planification, exécution et contrôle
c.	Création, modification et suppression
69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?
71.	Donner la définition des mots suivants :
a.	Entité
b.	Relation
c.	Cardinalité
d.	Clé primaire / clé étrangère
72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?
73.	Qu’est-ce qu’une base de données ?
74.	Définir les notions suivantes : 
a.	SQL
b.	MySQL
c.	SGBD (donner 2 exemples de SGBD)
75.	Dans une base de données, les données sont stockées dans des ___. Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___
76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?
77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?
78.	A quoi sert une vue dans une base de données ?
79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?
80.	Quelles sont les fonctions d’agrégation en SQL ?
81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
82.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table
b.	Modifier un enregistrement dans une table
c.	Supprimer un enregistrement dans une table
d.	Supprimer la base de données
e.	Filtrer les résultats d’une requête SQL
f.	Trier les résultats d’une requête SELECT
g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
h.	Concaténer 2 chaînes de caractères 
83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

## Symfony
84.	Qu’est-ce que Symfony ?
85.	Sur quel langage de programmation et design pattern repose Symfony ? 
86.	Quelle est la dernière version en date de Symfony ?
87.	Qu’est-ce qu’un bundle ? 
88.	Quel est le moteur de template utilisé par défaut dans Symfony ?
89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91.	Que permet le bundle Maker au sein de Symfony ? 
92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

## Sécurité
94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?
95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
97.	Définir l’attaque par force brute et l’attaque par dictionnaire
98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
100.	Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
101.	Qu’est-ce qu’une politique de mots de passe forts ?
102.	Qu’est-ce que l’hameçonnage ?
103.	Définir la « validation des entrées »

<br>
<br>

## RGPD

<br>

### 104.	Qu’est-ce que le RGPD ?

RGPD : Règlement Général sur la Protection des Données, il encadre le traitement des données personnelles des citoyens de l’Union européenne (UE).

> [!NOTE]
> Règlement : voté par le parlement européen et a donc une force obligatoire.

<br>
<br>

### 105.	Quel est son objectif principal ?

Définition RGPD:
- concerne traitement et circulation des données à caractère personnel
- fixe les conditions dans lesquelles les données peuvent êtres collectées, conservées et exploitées
- doit aussi s'y conformer : tous les organismes dans l'UE & celles qui collectent et traitent données des personnes situées sur le territoire de l'UE.

Son objectif principal est donc de protéger la vie privée des individus en garantissant un cadre juridique clair et homogène pour le traitement des données personnelles au sein de l’UE, tout en responsabilisant les organisations et les utilisateurs.

POURQUOI ?
- Harmonier la législation entre tous les pays européens.
- Responsabiliser les acteurs.
- Renforcer la confiance des citoyens européens qui confient leurs données en améliorant leur protection et leur confidentialité.

<br>
<br>

### 106.	Quelle est la date d’entrée en vigueur du RGPD ?

> [!IMPORTANT]
> Le RGPD est entré en vigueur le 25 mai 2018.

<br>
<br>

### 107.	Quelles sont les sanctions possibles en cas de non-respect du RGPD ?

Lorsque des manquements au RGPD ou à la loi sont portés à sa connaissance, la formation restreinte de la CNIL peut :
- faire un rappel à l'ordre par la présidente ou la formation restreinte
- injonction sous astreinte
- ordre de satisfaire aux demandes d'exercice des droits des personnes, y compris sous astreinte
- prononcer une amende administrative.

Ces sanctions peuvent être rendues publiques (si mise en demeure publique, sur cnil.fr & legifrance.fr).

En cas d'amende administrative, la sanction pécuniaire peut s'élever jusqu'à 20 millions € ou dans le cas d’une entreprise jusqu’à 4% du CA mondial.

<br>
<br>

### 108.	En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?

La CNIL (Commission Nationale de l’Informatique et des Libertés) s’occupe de faire appliquer le RGPD en France.

MISSIONS DE LA CNIL :
- informer et protéger les droits
- accompagner la conformité et conseiller
- anticiper et innover
- contrôler et sanctionner.

<br>
<br>

### 109.	Quel est le consentement valide selon le RPGD ?

Quatre critères cumulatifs doivent être remplis pour que le consentement soit valablement recueilli. Le consentement doit être :
- Libre : donné sans pression / influence ou sous la contrainte (la personne doit se voir offrir un choix réel, sans avoir à subir de conséquences négatives en cas de refus)
- Spécifique : applicable à une finalité précise et correspondre à un seul traitement
- Éclairé : accompagné d’un certain nombre d’informations communiquées à la personne avant qu’elle ne consente.
- Univoque : exprimé par une action positive claire, comme cocher une case (aucune ambiguïté quant à l’expression du consentement ne peut demeurer).

<br>
<br>

### 110.	Qu’est-ce qu’une politique de confidentialité ?

La politique de confidentialité est un document ou une déclaration publique qui informe les utilisateurs :
- des données personnelles collectées les concernant
- de la finalité des traitements qui sera fait de leurs données
- des droits des utilisateurs et comment les exercer (pour assurer la maîtrise de leurs données)
- des mesures de protection mises en place par l’entreprise.

<br>
<br>

### 111.	Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?

Les données personnelles ne peuvent être conservées indéfiniment : une durée de conservation doit être déterminée par le responsable de traitement en fonction de l’objectif ayant conduit à la collecte de ces données. 

Pour un même traitement, les données personnelles poursuivent des phases successives. On parle de « cycle de vie » de la donnée personnelle. 

Ce cycle connaît trois phases :

- Conservation en base active : durée nécessaire à la réalisation de l’objectif (finalité du traitement) ayant justifié la collecte/enregistrement des données. 
Exemple: dans une entreprise, les données d’un candidat non retenu seront conservées pendant 2 ans maximum (sauf s’il en demande l’effacement) par le service des ressources humaines.

- Archivage intermédiaire : Les données personnelles ne sont plus utilisées pour atteindre l’objectif fixé (« dossiers clos ») mais présentent encore un intérêt administratif pour l'organisme (ex : gestion d’un éventuel contentieux, etc.) ou doivent être conservées pour répondre à une obligation légale (par exemple, les données de facturation doivent être conservées dix ans en application du Code de commerce, même si la personne concernée n’est plus cliente). Les données peuvent alors être consultées de manière ponctuelle et motivée par des personnes spécifiquement habilitées.

- Archivage définitif: En raison de leur « valeur » et intérêt, certaines informations sont archivées de manière définitive et pérenne.

<br>
<br>

### 112.	Quels sont les droits des utilisateurs selon le RGPD ?

DROITS DES PERSONNES

Les droits renforcés:
- droit d'information -> être informé du traitement et des finalités (politique de confidentialité par ex)
- droit d'accès -> consulter les données personnelles collectées (formulaire de contact / nous contacter par ex)
- droit de rectification -> corriger des données inexactes (bouton éditer le profil / contact)
- droit d'opposition -> s’opposer à certains traitements, notamment marketing
- droit à l'effacement ("à l'oubli") -> demander la suppression des données (peut être anonymisé par ex).

Nouveaux droits:
- droit à la portabilité (si le traitement est automatisé) -> récupérer leurs données dans un format réutilisable
- droit à la limitation -> restreindre le traitement de leurs données
- droit lié à la prise de décision automatisée -> ne pas faire l’objet d’une décision automatisée.

<br>
<br>

### 113.	Qu’est-ce que le principe de minimisation des données selon le RGPD ?

Le principe de minimisation impose que seules les données (à caractère personnel) strictement nécessaires à la réalisation des finalités du traitement soient collectées et utilisées. Cela limite la collecte excessive ou non pertinente.

Exemple : Collecter et conserver le statut marital d’un salarié n’apparaît pas nécessaire à l’activité RH.

<br>
<br>

## SEO
114.	Qu’est-ce que le SEO ? 
115.	Quel est l’objectif principal du SEO ?
116.	Existe-t-il plusieurs types de référencement ? Lesquels ?
117.	Qu’est-ce que la densité de mots-clés en SEO ?
118.	Qu’est-ce que l'attribut « alt » ?
119.	Qu’est-ce que la balise « meta description » ?
120.	Qu’est-ce que le « nofollow » en SEO ?
121.	Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
122.	Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
123.	Quelle est la recommandation pour les URL d'un site web bien référencé ?
124.	Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
125.	Qu'est-ce que l'optimisation des images pour le référencement ?
126.	Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps
127.	Qu’est-ce que la gestion de projet ?	
128.	Qu’est-ce qu’une méthode Agile de gestion de projet ? 
129.	Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
130.	A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131.	Qu’est-ce que la planification itérative ?
132.	Citer 3 méthodes Agiles dans le cadre d’un projet informatique
133.	Qu’est-ce qu’une réunion de revue de projet ?
134.	Qu’est-ce qu’un livrable dans un projet ? 
135.	Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
136.	Qu’est-ce que le DevOps et quel est son objectif principal ?
137.	Qu’est-ce que l’intégration continue ? 
138.	Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
139.	Qu’est-ce qu’un test unitaire ? 
140.	Quelle est l'unité de code testée lors d'un test unitaire ?
141.	Quelles sont les caractéristiques d'un bon test unitaire ?
142.	Qu'est-ce qu'une assertion dans un test unitaire ?
 
## English
1)	What does JavaScript enable you to do on a website ?
a.	Add interactive behavior and dynamic content
b.	Define the layout and design of web pages
c.	Handle server-side operations
2)	Which programming language is primarily used for server-side web development ?
a.	PHP
b.	JavaScript
c.	HTML
3)	What is the purpose of a web browser ?
a.	To render and display web pages
b.	To execute serve-side code
c.	To manage databases
4)	What is the difference between GET and POST methods in HTTP ?
a.	GET retrieves data from a server, while POST submits data to a server
b.	GET submits data to a server, while POST retrieves data from a server
c.	GET and POST methods are interchangeable
5)	What is the purpose of version control systems (e.g., Git) in web development ?
a.	To track changes and manage collaborative development
b.	To optimize website loading speed
c.	To handle server-side scripting
6)	What is the purpose of a framework in web development ?
a.	To provide a structured environment for building web applications
b.	To handle network protocols and data transfer
c.	To create visual designs and layouts for websites
7)	What does NoSQL stand for ?
a.	Not Only SQL
b.	Non-Structured Query Language
c.	New Object-Oriented Language
8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models