# Medileak CTF


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
En passant par la wayback machine, on retrouve l'url de leur réseau social: social.osain.eu
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



# Le docteur
## Questions indiscrètes
```
Selon vos renseignements, Christine n’a pas beaucoup d’argent. Elle aura peut-être négocié un prêt ou autre financement. Quelle est le deuxième groupe de mot en gras dans le questionnaire qu’elle a rempli (hors titres) ?

Format de flag : liste de courses à faire
```

Sur le site d'osain, on trouve le formulaire en cherchant dans le stage annulé.

flag: état de santé actuel

## Poussez vous je suis medecin
```
Avant d’intégrer le stage, un avis médical d’un médecin partenaire est indispensable. Comment s’appelle le médecin avec qui Christine semble être en contact ?

Format de Flag : Louis Pasteur
```

Toujours sur le site:

flag: Raoul Reidid

## Doctor Lib’
```
Il faudrait confirmer qu’il s’agit bien de ce médecin qui a eu rendez-vous avez Christine. Quel jour à quelle heure devait-elle consulter ?

Format de Flag : JJ/MM/YYYY HH:MM
```

On trouve le mot de passe sur le post-it du message précédent: r4ou71STH3b3S7
Dans les fichiers, un calendrier .ict avec un rendes-vous concernant un patient ayant le SEP.

flag : 19/04/2024 17:30