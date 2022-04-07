Data Visualisations Prénoms en France depuis 1900
===
Victor Boby, Anaïs Mazoué, Ariane Menu - Avril 2022

# Objectif : enrichissement d'un dataset de prénoms

## Dataset original (dpt2020)
A partir du Fichier des prénoms de l'INSEE (https://www.insee.fr/fr/statistiques/2540004?sommaire=4767262&q=pr%C3%A9noms), qui contient les prénoms attribués aux enfants nés en France hors Mayotte entre 1900 et 2020 et les effectifs par sexe associés à chaque prénom par département.

Nous avons choisi d'aborder ce dataset du point de vue de la diversité et notamment de croiser ces informations avec les origines des prénoms bretons, occitans, bibliques et anglais, d'après leurs attributions d'origine de Wikipédia.

Deux data visualisations à partir du dataset original ont également été produites :
- les 10 prénoms les plus donnés par année depuis 1900,
- l'évolution du nombre de prénoms par département depuis 1900.

## Données Wikipédia
à compléter

## Données écartées
- Nous avons écarté l'exploitation du fichier Pantheon 2020 Person Dataset, un important dataset de données biographiques, du fait de l'absence de données historiques

## Nettoyage des jeux de données (dpt2020)

### Nettoyage du fichier INSEE
- 803 lignes (sur 3,7 millions) pour lesquelles des données n'étaient pas exploitables ont été supprimées. Il s'agit notamment d'enregistrements dont le champ année de naissance (ANNAIS) prenait la valeur «XXXX» et les départements de naissance (DPT) codés en «XX» pour certains cas de prénoms rares (voir "Conditions portant sur les prénoms retenus" sur le sire de l'INSEE).

- Les valeurs «_PRENOMS_RARES_» du champ prénom (PREUSUEL) ont été conservées pour les visualisations obtenues exclusivement depuis ce dataset, afin de ne pas perdre cette notion du point de vue de la diversité adopté.

- Autres nettoyages faits par Ariane à ajouter

### Traitements

- 10 prénoms les plus donnés par année depuis 1900 : les 10 premiers prénoms par département par année ont été filtrés dans Dataiku (recette TopN)
- Evolution du nombre de prénoms par département depuis 1900 : le nombre de prénoms par département et par année est obtenu directment dans Tableau aves les fonctions de calcul




