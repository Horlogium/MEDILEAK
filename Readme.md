# Medileak CTF
Write Up de la team dodo pizza

# La victime
## Il était une fois…
On lit l'énoncé et:

*flag: C’est parti*

## Le travail
```
Vous allez tout d’abord essayer de dresser le portrait de la victime. Quel est son emploi actuel, et depuis quand l’occupe t-elle ?

Format de flag : assistante de direction - 2010
```


Dans le mail donné dans le premier challenge, on trouve le nom de la victime: Christine Daguerran

On trouve son facebook: https://www.facebook.com/profile.php?id=61557910274434

*flag : chargée de mission - 1996*

## La maladie
```
Elle se plaint de souffrir de ses traitements, sans doute une des raisons de son abandon de soin.

Quelle maladie a-telle l’impression d’avoir après son traitement ?

Format de flag : choléra
```
[maladie]: ./images/lamaladie.png
![maladie]

*flag: grippe*

## La détente
```
Elle aime se promener parfois pour estomper ses symptomes. A quelle adresse a t-elle pris une photo près de chez elle ?

Format de flag : 123 rue du Lac, Feytiat
```
On retrouve le lieu de la photo sur google maps:

[detente]: ./images/ladetente.png
![detente]

*flag: 585 route des Chaverneaux, Ambazac*

## Le médicament
```
Quel est le numéro CAS du traitement qui cause ces symptômes chez Christine ?

Format de flag : 123456-12-1
```
Dans un commentaire sur Facebook, elle parle de Rebif. On trouve son numéro CAS sur wikipédia:

*flag: 145258-61-3*

# Le coach
## Un homme bien sous tous rapports
```
Christine a trouvé un « soutien » dans son parcours qui semble lui apporter des conseils en privé. Quel est son nom ?

Format de flag : Raymond Redington
```

Dans ses amis facebook, on trouve:

*flag : Mathias Haztinger*

## Joli village 
```
Dans quelle commune dit-il résider ?

Format de flag : Madrid
```
Sur le Facebook de Mathias, on trouve:

[village]: ./images/village.png
![village]

*flag : Rochechouart*

## Des tarifs raisonnables ?
```
Vous essayez d’en apprendre plus sur ce coach. Combien coûte 1h de consultation avec lui ?

Format de flag : 99
```
Depuis le profil Facebook de Mathias, on trouve le site de osain.eu
En passant par la wayback machine, on retrouve l'url de leur réseau social: social.osain[.]eu
On se crée un compte, on va sur le profil de mathias. En banniere, on trouve l'url de son site perso avec la réponse: https://mathias-coach-bien-etre.e-monsite.com/

*flag: 95*

## Un lieu bien trouvé
```
A quel endroit s'est tenu le stage organisé par Mathias ?

Format de Flag (parcelle Cadastrale) : SECTION PARCELLE
```

On utilise le cadastre inversé avec les informations trouvées sur le site: https://trinv.fr/carte-parcelles?inseeid=87126&commune=ROCHECHOUART&surface=2161 

*flag: B 1089*


# Anonymous
## Le Chef
```
Mathias est en lien avec une association pour organiser ses stages. Quel est le pseudo du chef de l'association sur leur réseau social ?

Format de flag : michel boss
```

Sur le réseau social, on trouve le nom.

*flag: Edgard Admin*

## Un simple oubli…
```
Edgard, le chef de l'association, semble avoir perdu quelque chose. Mais dans quel endroit ?

Format de flag : Bordeaux, Aéroport Bordeaux Mérignac
```

Sur le réséau social.osain[.]eu, on trouve le message suivant:

![oubli](./images/oubli.png)

*flag : Limoges, Gare de Limoges-Bénédictins*

## ...mais un oubli compromettant
```
Cette perte vous donne une information inattendue !

Quelle est la véritable identité d’Edgard ?

Format : Georges Clooney
```

Sur le message précédent, Edgard mentionne qu'il a publié une annonce pour retrouver les documents qu'il a perdu.
En cherchant, on trouve cette annonce: https://les-objets-perdus.fr/objets/single/R8EiHDgK3

![oubli2](./images/oubli2.png)


*flag: Isaac Decheev*

## Reconversion
```
Quelle était l’entreprise pour laquelle Isaac a travaillé pendant plus de 21 ans ?

Format de Flag : Renault France SA
```

On trouve un profil LinkedIn au nom d'Isaac:

![reconversion](./images/reconversion.png)

*Flag : Ricoh Canada Inc.*

## Nos meilleures années
```
Dans quelle établissement Isaac et Raoul ont fait leur études en commun ?

Format : Collège Privé Louis Arago
```

L'information est disponible sur le LinkedIn, et aussi sur le CV de Raoul:

![lycee](./images/lycee.png)

*flag : Lycée Professionnel Francois d'Assise*


# Localisation
## Un nouveau départ
```
Rien ne semble se passer comme prévu, et Isaac préfère prendre des distances avec ses activités actuelles.

Quelle est sa nouvelle destination ?

Format de Flag : Barcelone - Espagne
```

Voir post linkedin avec le numéro de vol : ACA871
Grâce à flight radar 24 on trouve que c’est un vol Paris Montreal.

*flag: Montréal - Canada*

## Retour aux sources
```
Kalliopée n’est plus en France actuellement… Trouvez l’endroit où elle a résidé en dernier.

Format de Flag : Nice Rock Grandhotel
```

Avec la photo qu'a posté Kalliopee sur son reseau, on peut rechercher un endroit qui correspond aux lettres qu'on peut voir en bas à gauche. Sur la page TripAdvisor, on trouve son commentaire et son profil: 
https://www.tripadvisor.com/Profile/kalliopee_hadrianos?fid=1a9db9cf-d3df-41c6-9349-99c8df896793

*flag: Pier Beach Aparthotel*

## Jolie ville
```
Mathias a laissé un message sur le téléphone de Christine...

Pourrez vous retrouver la ville où il se cache ?

Format de flag : Limoges
```

On nous donne un enregistrement MP3. En fond, on peut entendre un grand nombre de cloches. Un peu par hasard, on tombe sur la page de la cathédrale de Strasbourg: https://fr.wikipedia.org/wiki/Sonnerie_de_la_cath%C3%A9drale_de_Strasbourg
Vers la fin, on peut entendre deux femmes parler, ce qui nous confirme que c'est le même audio.

*flag: Strasbourg*

## Le monde du silence
```
A quel endroit est localisée la dernière trace numérique laissée par Henri ?

format de flag : 12° 34′ 00″ sud, 5° 67′ 00″ est
```

On utilise la dernière photo publiée par Henri:

![marin](./images/marin.png)

On retrouve le lieu grâce à un reverse search, et on trouve les coordonnées sur la page wikipédia du sous marin.

*flag : 47° 39′ 00″ nord, 3° 34′ 00″ ouest*

## Mon petit village
```
Gizem également semble avoir quitté le territoire. Pourrez vous retrouver dans quel village elle est partie ?

format de flag : New York
```

Le post mastodon du Sysadmin nous apprend que Gizem aime chanter: 

![soundcloud](./images/soundcloud.png)

On trouve le lien de son Soundcloud: https://soundcloud.com/gizem-469913696 

Il contient 4 chansons en grec. On utilise un service de speech2text et de traduction pour obtenir les paroles en français. On cherche:
* Un village à Chypre
* Au bord de la mer
* Avec 2 églises 
* Une place décorée
* Des carrés

Grâce à la magnifique recherche google suivante, on trouve la ville concernée :
```
chyprus "two churches" village sea
```

*flag: Kato Pyrgos*

# Le docteur
## Questions indiscrètes
```
Selon vos renseignements, Christine n’a pas beaucoup d’argent. Elle aura peut-être négocié un prêt ou autre financement. Quelle est le deuxième groupe de mot en gras dans le questionnaire qu’elle a rempli (hors titres) ?

Format de flag : liste de courses à faire
```

Sur le site d'osain, on trouve le formulaire en cherchant dans le stage annulé.

*flag: état de santé actuel*

## Poussez vous je suis medecin
```
Avant d’intégrer le stage, un avis médical d’un médecin partenaire est indispensable. Comment s’appelle le médecin avec qui Christine semble être en contact ?

Format de Flag : Louis Pasteur
```

Toujours sur le site:

*flag: Raoul Reidid*

## Doctor Lib’
```
Il faudrait confirmer qu’il s’agit bien de ce médecin qui a eu rendez-vous avez Christine. Quel jour à quelle heure devait-elle consulter ?

Format de Flag : JJ/MM/YYYY HH:MM
```

On trouve le mot de passe sur le post-it du message précédent: r4ou71STH3b3S7
Dans les fichiers, un calendrier .ics avec un rendes-vous concernant un patient ayant le SEP.

*flag : 19/04/2024 17:30*

## Belle expérience 
```
Afin de parfaire votre profil du medecin, essayez de trouver quel est le premier diplôme qu’il a obtenu dans le domaine médical. Quel établissement lui a délivré son diplôme en 2022 ?

Format de Flag : Faculté Mondiale du Portugal
``` 

Dans le drive, on trouve l'information sur le CV de Raoul: 

*Flag : Université Internationale de Chypre*

## Adieu le foie
```
Le Docteur Reidid ne semble pas médecin… mais est-il seulement pharmacien ?

Dans sa thèse de fin d’étude, il semble qu’une erreur terrible a été commise, pouvant conduire à la destruction du foie des patients !

Quelle dose totale de la molécule étudiée était administrée par 24h aux participants ?

Quelle est la dose maximale recommandée par les médecins en automédication ?

Format de Flag (dose administrée / dose recommandée) : 4302mg / 1000mg
```

Sur le drive, dans sa thèse, on trouve l'information concernant la posologie du paracetamol, et on la compare avec ce qui est recommandé: 

![paracetamol](./images/paracetamol.png)

*Flag : 8000mg / 3000mg*

## Expérience cachée
```
Il semble que le bon Docteur essaie de dissimuler une de ses expériences professionnelles…

Quel est le nom de l’entreprise qu’il a fondée et qui ne figure pas sur son CV officiel ?

Format de Flag : Mc Donald’s Healthy Food
```

Sur le forum social.osain[.]eu, on voit qu'une marque est sponsorisée : Dr. Revel's Marvel Oils. En commentaire des posts, un certain Johnny propose de nous en apprendre plus en le contactant par mail. Il signe un de ses messages par un pseudo: johnny-b9bb. Maigret nous donne un lien correspondant à ce pseudo: https://calendly.com/johnny-b9bb, sur lequel on peut trouver son adresse mail: johnny@ozmail.eu 


Une suite de mail avec lui nous permet d'obtenir un lien vers la boutique de cette marque: 

![boutique](./images/boutique.png)

Sur ce site, on voit dans l'histoire qu'elle a été créée par un certain Raoul R. Cela confirme notre hypothèse:

*flag: Dr. Revel's Marvel Oils*

# La Clinique

## Le lien
```
Au delà du médecin, qui a été désavoué par Edgard, il existe peut-être un lien entre les 2 structures. Mais il faut le prouver !

A quelle date et heure des fichiers ont-ils été transmis pour la dernière fois à la clinique par Osaïn ?

Format de flag : AAAA-MM-JJ HH:MM
```

En regardant le robots.txt du site d'osain, on trouve: https://osain.eu/ftp/log.txt

La date est présente au début du ficher: 

*flag: 2024-04-20 23:34*

## Trust me I am a developper
```
Quelle est la version du logiciel utilisé pour récupérer les questionnaires par la clinique ?

Format de flag : v4.9.8
```

Dans le fichier précédent, on trouve le lien de destination. Sur le site de la clinique, un fichier php est présent, contenant la version: 

*flag: v1.4.2*

# Start with a K
