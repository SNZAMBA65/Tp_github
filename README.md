# Tp_github

Un dépôt pour apprendre Git et GitHub à travers des exercices pratiques.

## Description

Ce projet contient une petite application Python qui affiche l'heure actuelle. Le but principal est de pratiquer les commandes Git de base : branches, commits, merge et résolution de conflits.

## Installation

Clonez le dépôt :

```bash
git clone https://github.com/SNZAMBA65/Tp_github.git
cd Tp_github
```

Aucune dépendance externe requise, juste Python 3.

## Utilisation

```bash
python code.py
```

Affiche l'heure actuelle au format `HH:MM:SS`.

## Structure

- `code.py` - Script principal
- `module.py` - Module contenant la logique métier
- `README.md` - Documentation

---

## Exercices réalisés

### TP1 : Manipulation des branches, commits, push et fusion

#### Objectifs
- Créer et gérer des branches Git
- Effectuer des commits structurés
- Fusionner des branches avec merge
- Synchroniser avec GitHub

#### Déroulement
1. **Travail initial sur `main`** : Création du fichier `code.py` avec affichage simple de l'heure
2. **Création de la branche `refonte`** : Refactorisation du code avec création d'un module séparé
3. **Développement modulaire** : Ajout de `module.py` contenant la fonction `obtenir_temps()`
4. **Fusion** : Merge de `refonte` dans `main` (fast-forward)
5. **Nettoyage** : Suppression de la branche `refonte` après fusion

#### Commandes clés utilisées
```bash
git checkout -b refonte
git add .
git commit -m "message"
git merge refonte
git push origin main
```

---

### TP2 : Création et résolution d'un conflit de merge

#### Objectifs
- Comprendre l'origine des conflits Git
- Identifier les marqueurs de conflit
- Résoudre manuellement un conflit
- Valider la résolution

#### Déroulement
1. **Création de deux branches divergentes** : `conflit-a` et `conflit-b` modifiant le même fichier différemment
2. **Fusion de `conflit-a`** : Merge réussi dans `main`
3. **Tentative de fusion de `conflit-b`** : Conflit détecté par Git
4. **Résolution manuelle** : Édition du fichier pour choisir la version finale
5. **Validation** : Commit de résolution et push

#### Marqueurs de conflit rencontrés
```
<<<<<<< HEAD
print("Version A du code")
=======
print("Version B du code")
>>>>>>> conflit-b
```

#### Résolution appliquée
Le conflit a été résolu en choisissant une version finale unifiée, puis validé avec :
```bash
git add code.py
git commit -m "Résolution du conflit entre conflit-a et conflit-b"
git push origin main
```

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
```

2. Installer les dépendances si ce n'est pas déjà fait :
```bash
pip install -r requirements.txt
```

3. Ouvrir le notebook `TP4_AB_Testing.ipynb` dans VS Code ou Jupyter Notebook et exécuter les cellules dans l'ordre.

4. Un PDF professionnel est généré automatiquement à la dernière cellule : `TP4_report_pro.pdf`.

### Ce que j'ai appris

- Préparer et filtrer un dataset réel pour un test A/B
- Randomiser correctement par utilisateur
- Calculer un KPI e-commerce et le comparer entre groupes
- Effectuer un test statistique (Z-test) et interpréter la p-value
- Prendre une décision produit basée sur les résultats
- Créer des visualisations claires et un rapport PDF prêt à présenter

### Installation

**Prérequis :**
- Python 3 (>=3.10 recommandé)
- Modules Python : `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `tabulate`

Rien de spécial à installer en dehors de ces modules.

---

## Auteur

Samir NZAMBA (@SNZAMBA65)

## Licence

Projet éducatif sans licence spécifique.