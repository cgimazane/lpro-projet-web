# Projet Web

Licence Pro, parcours Environnement et Géomatique
======================

## Sujet

Il s'agit de créer un site web utilisant toutes les technologies vues en cours : `html`, `css`, `JavaScript`, `PHP` et `SQL`.

Vous avez carte blanche pour le design du site, le but étant, entre autres, d'utiliser le maximum de propriétés CSS
vues en cours.

Toutes les pages devront avoir :
* une bannière avec au moins un logo de l’ENSG et un lien vers la page d’accueil
* un menu horizontal placé sous la bannière
* un pied de page

## Données

Les données localisant les sites retenus pour les JO 2024.

### Descritpion des données

Pour commencer :

- un fichier GeoJSON
- un fichier CSV

Contenant une liste de sites sportifs sélectionnés pour accueillir des épreuves olympiques.

Pour chaque site, on a :

- un nom _name_
- une description des sports accueillis _description_
- une représentation du lieu _img_
- une capacité _capacite_
- une latitude _latitude_
- une longitude _longitude_
- une représentation géométrique

### Création de la base de données

* Créer une nouvelle base de données et une table avec les champs corrects (avec des noms clairs)
* Importer le fichier CSV
```sql
COPY nom_de_table(champ1,champ2,champ3)
FROM 'chemin/vers/fichier' DELIMITER ',' CSV HEADER;
```
  - Le séparateur de colonnes est la virgule
  - La première ligne du fichier contient le nom des colonnes
* Renommer la table créée.
```sql
ALTER TABLE ancien_nom RENAME AS nouveau_nom;
```

## Fonctionnalités du site

Le site sera composé de trois pages
1. Une page d’accueil donnant quelques informations sur vous, le master, le module, le projet, le sujet, etc...
2. Une page de visualisation
  - avec une carte qui affiche nos données
  - centrée au chargement de la page sur ces données
  - dans laquelle s’ouvre un popup d’informations quand on clique sur un lieu
  - avec un tableau avec les données chargées en PHP depuis la base de données. Chaque ligne correspond à un lieu avec son nom, sa capacité, les sports accueillis et possède un bouton qui centre la carte sur le site sélectionné
3. Une page de requête avec :
  - une carte du Géoportail affichant nos données
  - un formulaire de recherche, permettant d'afficher les 10 sites les plus proches d’un des points de logement (sélectionné par l’utilisateur dans un menu déroulant)

## Conseils

La troisième page est plus délicate et devra être abordée en dernier

Piste : On pourra vérifier au chargement de la page l'existence des paramètres `$_GET['start']`. S’il existe, c'est nécessairement qu'une requête a été effectuée précédemment et on l'exécute.

Sinon, on affiche simplement la carte et le formulaire.

Le formulaire renvoie sur la même page avec (par exemple) dans l'url le paramètre start éventuellement saisi.


## Notation

- Compréhension du sujet
- Atteinte et dépassement du sujet.
- Qualité des pages proposées
- Mise en valeur de l'information géographique utilisée
- Qualité et technicité du développement
- Prestation orale
