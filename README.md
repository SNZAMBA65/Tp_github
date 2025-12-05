# TP Git - Apprendre les branches

Un petit projet pour s'entraîner sur Git. J'ai appris à créer des branches, faire des commits, fusionner le tout et pousser ça sur GitHub.

## Ce qu'il y a dans le projet

Le projet contient deux fichiers Python :

**code.py** : Le fichier principal qui affiche l'heure qu'il est en ce moment

**module.py** : Un module que j'ai créé pour organiser le code proprement avec une fonction `obtenir_temps()`

## Comment ça marche

C'est simple, il suffit de lancer :

```bash
python code.py
```

Et ça affiche quelque chose comme :
```
Hello ! Il est 14:30:25.
```

## Ce que j'ai appris

Au début, j'ai fait un fichier simple sur la branche `main`. Ensuite j'ai créé une branche `refonte` pour réorganiser le code et créer un module séparé. Une fois que c'était bon, j'ai fusionné tout ça dans `main` et nettoyé la branche `refonte`.

Pas très compliqué finalement, mais c'est cool de voir comment Git gère tout ça !

## Installation

Rien de spécial à installer, juste Python 3. Le module `datetime` est déjà inclus dans Python.

---

## TP2 - Gestion des conflits

Dans un deuxième temps, j'ai géré les conflits Git. J'ai créé deux branches (`conflit-a` et `conflit-b`) qui modifiaient le même fichier différemment. Quand j'ai essayé de les fusionner, Git m'a dit "je sais pas laquelle choisir, débrouille-toi".

Du coup j'ai dû :
- Ouvrir le fichier qui posait problème
- Voir les marqueurs de conflit (`<<<<<<<`, `=======`, `>>>>>>>`)
- Choisir la version finale que je voulais garder
- Valider le tout

---

## TP4 – A/B Testing avec RetailRocket

Ce projet est un TP sur l'A/B Testing pour un site e-commerce. L'objectif était d'analyser un dataset réel, simuler un test A/B et prendre une décision produit basée sur des résultats statistiques.

### Ce qu'il y a dans le projet

Le projet contient un notebook principal :

**TP4_AB_Testing.ipynb** : Notebook complet pour le TP4, incluant :

- Nettoyage et exploration des données
- Simulation d'un test A/B par utilisateur
- Calcul du KPI Add-to-Cart Rate pour chaque groupe
- Test statistique de comparaison de proportions (Z-test)
- Analyse business pour recommander un design
- Visualisations professionnelles (barplots, tableau résumé)
- Export PDF final avec graphiques et tableau

Le fichier **events.csv** est également inclus (ou doit être placé dans le même dossier) pour l'analyse.

### Comment ça marche

1. Activer l'environnement virtuel :

```bash
source venv/Scripts/activate  # Windows Git Bash / Linux / MacOS


Fin

---

Fait par Samir dans le cadre d'un TP sur Git