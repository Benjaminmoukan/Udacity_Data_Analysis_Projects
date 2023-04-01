# Projets techniques pour le nanodegree ALX-DATA ANALYSIS de Udacity

## Sommaire :
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#noshow">Projet 1 : No-Show Appointments 2016</a></li>
<li><a href="#wrangle">Projet 2 : WeRateDogs - Préparation et Analyse</a></li>
<li><a href="#bike_sharing">Projet 3 : Analyse des données d'un système de partage de bicyclettes</a></li>
</ul>


<a id='intro'></a>
## Introduction :

Ce dépôt contient les projets sur lesquels j'ai eu à travailler dans le cadre du Nanodegree ALX Data Analysis que j'ai suivi pendant trois mois environ sur Udacity. Ces derniers ont été soumis et approuvés. Il contient d'autres projets également sur lesquels j'ai pu travailler par la suite.

<a id='noshow'></a>
## Projet 1: No-Show Appointments 2016

### Description du jeu de données
Ce premier projet a consisté au nettoyage et à l'analyse du jeu de données Show Appointments. Il provient de la plateforme [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments?page=3). Il contient plusieurs colonnes; en voici quelques-unes :

   * PatientId : le numéro d'identification unique du patient 
   * AppointmentID : numéro d'identification unique de chaque patient pour chaque rendez-vous programmé.
   * Sexe : Femme (F) ou homme (M)
   * ScheduledDay : La date et l'heure auxquelles chaque rendez-vous a été programmé.
   * AppointmentDay : La date réelle de chaque rendez-vous programmé.
   * Age : L'âge des patients.
   * Neighbourhood : où vit chaque patient.
   * Scholarship : inscription ou non du patient à la [Bolsa Família](https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia), un programme d'aide sociale mis en place par le gouvernement du Brésil, entre 2003 et 2021.
   * Hipertension : enregistrements permettant de savoir si chaque patient souffre ou non d'hypertension.
   * Diabetes : dossiers indiquant si chaque patient est diabétique ou non.
   * Alcoholism : indique si chaque patient souffre d'alcoolisme chronique ou non.
   * Handcap : enregistrements indiquant si chaque patient souffre ou non d'une forme de handicap.
   * SMS_received : indique si chaque patient a reçu un ou plusieurs SMS de rappel pour son rendez-vous programmé, ou pas non.
   * No-Show : indique si le patient s'est présenté à son rendez-vous ou non. Ici, 'No' signifie que le patient ne s'est pas présenté, c'est-à-dire qu'il a respecté son rendez-vous.


### Questions auxquelles j'ai répondu
Après avoir collecté et nettoyé les données, les questions qui ont guidé mon analyse ont été les suivantes : 

   1. Les personnes en général ont-ils tendance à respecter leur rendez-vous ?
   2. Est-ce que le genre d'un patient influence le fait qu'il respecte son rendez-vous ?
   3. Les rendez-vous sont-ils mieux respectés par les personnes d'une certaine tranche d'âge ?
   4. Avoir un handicap est-il un facteur qui pousse ou non à respecter le rendez-vous ?
   5. Les gens qui n'ont pas reçu de SMS ont-ils eu tendance à ne pas respecter leur rendez-vous ?


<a id='wrangle'></a>
## Projet 2 : WeRateDogs - Préparation et Analyse 

Pour ce second projet principalement axé sur les compétences en préparation des données (collecte, évaluation et nettoyage), il m'a été demandé de "gratter" (web scraping) des tweets de l'archive du compte WeRateDogs (@dog_rates), en utilisant l'API Tweepy. Une analyse visuelle et à l'aide de Python via pandas s'en est suivie; ensuite j'ai nettoyé le jeu de données sur la base de l'évaluation que j'avais faite. Pour enfin l'analyser.

### Description du jeu de données

Il comprend les colonnes suivantes : 

   * tweet_id : La dernière partie de l'URL du tweet après "status/".
   * date_created : La date et l'heure auxquelles chaque tweet a été posté.
   * source : Le type d'appareil à partir duquel le tweet a été fait.
   * text : Le contenu complet du tweet.
   * expanded_url : Le lien vers chaque tweet.
   * rating_numerator : La note attribuée à chaque chien sur une échelle de (presque) 10.
   * name : Le nom de chaque chien évalué.
   * dog_stage : Si chaque chien est un doggo, un floofer, un pupper, un puppo ou aucun.
   * favorite_count : Nombre de likes que chaque tweet a recueilli.
   * retweet_count : Nombre de "retweets" obtenus par chaque tweet.
   * jpg_url : Lien vers chaque image contenue dans chaque tweet.
   * p1 : la prédiction n°1 de l'algorithme pour l'image contenue dans le tweet.
   * p1_conf : le degré de confiance de l'algorithme dans sa prédiction n°1. 
   * p1_dog : si la prédiction n°1 est une race de chien ou non. 
   * p2 : la deuxième prédiction la plus probable de l'algorithme
   * p2_conf : confiance de l'algorithme dans sa prédiction n°2
   * p2_dog : la prédiction n°2 est une race de chien ou non.
   * p3 : la troisième prédiction la plus probable de l'algorithme
   * p3_conf : confiance de l'algorithme dans sa prédiction n°3
   * p3_dog : si la prédiction n°3 est une race de chien ou non


### Questions auxquelles j'ai répondu :

Après avoir collecté et nettoyé les données, les questions qui ont guidé mon analyse ont été les suivantes : 

1. D'où (de quel type de téléphone) proviennent la plupart des tweets ?
2. Quelles sont les deux races de chien les plus identifiées sur les photos ?
3. Quelles sont les deux stades de chien les plus répertoriés ?
4. De tous les stades de chien répertoriés, quel est celui qui a le plus apprécié (qui a le plus de likes) ?


<a id='bike_sharing'></a>
## Projet 3 : Analyse des données d'un système de partage de bicyclettes

Ce dernier projet était axé sur la visualisation des données. L'ensemble de données comprend des informations sur les trajets individuels effectués dans un système de partage de vélos couvrant la grande région de la baie de San Francisco. Ces données s'étendent sur un mois entier (février 2019). 

### Dataset Description.
Les colonnes qui nous intéressent principalement sont les suivantes :

   * duration_sec : durée de l'emprunt de la bicyclette
   * user_type : type d'utilisateur de l'emprunteur ('Subscriber' ou 'Customer')
   * member_age : âge de l'emprunteur
   * member_gender : genre de l'emprunteur ('Male', 'Female' ou 'Other')

D'autres colonnes ont été créées à partir d'une colonne du jeu de données dans le but de nous permettre de mieux mener notre analyse :

   * day_of_week : jour de la semaine
   * starting_hour : heure du début de l'emprunt
   * day_of_month : jour du mois de l'emprunt

### Questions for Analysis.
Suivant que l'analyse exploratoire était univariée, bivariée ou multivariée, nous avions les questions suivantes : 

##### Univariée 
- Quelle est la durée à vélo la plupart du temps ?
- Quelle est la catégorie d'âge de ceux qui empruntent le plus de bicyclettes ? 
- La majorité des trajets sont-ils effectués par les hommes ou les femmes ?
- Quel pourcentage des trajets recensés est effectué par les utilisateurs de type Subscriber ?
- Y a-t-il une ou des périodes de la journée où l'affluence pour l'emprunt est plus importante ?
- Y a-t-il un jour, des jours ou une période de la semaine où les gens empruntent le plus les bicyclettes ?
- Y a-t-il un jour, des jours ou une période du mois où les gens ont le plus emprunté les bicyclettes ?


##### Bivariée
- Comment la durée du trajet, qui constitue notre première variable d'intérêt, varie en fonction de l'heure à laquelle la bicyclette a été empruntée et de l'âge de l'emprunteur ?
- Quelle est l'influence que les variables catégorielles peuvent avoir sur la durée d'un trajet ?
- Quelle est la relation entre l'âge d'un emprunteur et l'heure à laquelle le vélo est emprunté ?
- Quelle est l'influence que les variables catégorielles (genre, type d'utilisateur et jour de la semaine) peuvent avoir sur l'heure d'emprunt d'une bicyclette ?
- La répartition des trajets effectués par les hommes ou les femmes varie-t-elle en fonction des jours de la semaine ?
- Comment varient les répartitions des Subcriber et Customer chaque jour de la semaine ? Qu'en est-il des proportions ?


##### Multivariée
- Nous avons pu observer qu'en général les trajets de bicyclette féminins avaient tendance à mettre plus longs que les masculins. Peut-on faire la même observation pour chaque jour de la semaine ou alors certains jours seulement ?
- Qu'en est-il de la variation du temps de trajet par jour de semaine et par genre d'utilisateur ?
- Enfin, quelle est la relation entre la durée d'un trajet et les trois variables suivantes : l'heure d'emprunt, le genre et le type d'un utilisateur ?

