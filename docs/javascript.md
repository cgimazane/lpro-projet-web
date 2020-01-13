Editeur en ligne

[stackblitz](https://stackblitz.com/)

# 1 Introduction

[Ré-introduction à Javascript](https://developer.mozilla.org/fr/docs/Web/JavaScript/Une_r%C3%A9introduction_%C3%A0_JavaScript)

Certificat de naissance :
* Parent : Brendan Eich
* Date de naissance : 1995
* Lieu de naissance : NetScape 2
* Premier moteur JS écrit en C : SpiderMonkey

Caractéristiques :
* Interprété
* Léger
* Orienté Prototype
* Multiparadigme
* Dynamique
* Impératif
* Fonctionnel

Différent de JAVA
* D'abord appelé LiveScript.
* Renommé JavaScript pour "profiter" de la popularité du langage JAVA (Sun Microsystem).
* Reprend les structures de contrôle, les éléments de langage du Java et C++ pour faciliter l'apprentissage

Le langage est normalisé en 1997 avec ECMAScript :
* V2 - 1999
* V3 - 
* V4 - abandoné
* V5 - 2009
* V6 - 2015

Implémentations de JavaScript :
* SpiderMonkey moteur de Firefox / Thunderbird
* V8 - Google / Opera / NodeJs
* JavaScriptCore - Safari
* Chakra - I.E.

Les moteurs Javascript expose des APIs (interface de programmation) à partir desquelles les objets JavaScript pour manipuler le DOM ont été crées.

JS n'a pas de concept d'entrée / sortie (vs java / c++ / shell)

Execution du script dans un environnement hôte qui fournit les mécanismes de communication.

On retrouve JS dans : 
* les navigateurs
* Adobe / photoshop
* NodeJs
* Apache Couche DB
* GNOME (interface graphique Ubuntu)

# Evolution d'Internet

[Evolution du web](http://www.evolutionoftheweb.com/)

# Les types

## Les Nombres

64 bits / ```NaN``` / ```Infinity``` / ```-Infinity```

## Les String

Séquence de caractères unicode de 16bits

## Null et undefined

Type particuliers
* ```null``` : absence délibéré de valeurs
* ```undefined``` : pas encore affecté

## Boolean

Deux valeurs : true / false
Tout peut être interprété en booléen
* ```false, 0, "", NaN, null, undefined```
  * false
* toute autre valeur
  * true

## Déclaration et portée

```var``` déclare une variable qui peut être utilisée dans tout le bloc

```let``` déclare une variable qui n'est utilisée que dans le bloc où elle est déclarée

```const``` déclare une variable qui ne pourra pas être ré-affectée

## Opérateur

## Structure de contrôle

## Objet

Collection de clé (chaine de caratère) valeur (peut être n'importe quoi)

## Array

Objet particulier présentant la méthode length ou les clé suive une séquence numérique

## Fonctions

Ce sont des objets particuliers
* ```arguments```
* ```apply()``` method
* fonctions anonymes

