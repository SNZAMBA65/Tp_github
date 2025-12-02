# TP Git - Manipulation des branches et fusion

Ce projet est un exercice pratique sur l'utilisation de Git : gestion des branches, commits, fusion et synchronisation avec GitHub.

## 📋 Objectifs du TP

- Créer et gérer des branches Git
- Effectuer des commits
- Fusionner des branches
- Synchroniser avec un dépôt distant (GitHub)

## 📁 Structure du projet

```
Tp_github/
│
├── code.py       # Fichier principal qui affiche l'heure actuelle
├── module.py     # Module contenant la fonction obtenir_temps()
└── README.md     # Ce fichier
```

## 🚀 Fonctionnalités

### `module.py`
Contient une fonction `obtenir_temps()` qui retourne l'heure actuelle formatée.

### `code.py`
Utilise le module pour afficher un message avec l'heure actuelle.

## 💻 Utilisation

Pour exécuter le programme :

```bash
python code.py
```

Résultat attendu :
```
Hello ! Il est 14:30:25.
```

## 🔄 Workflow Git utilisé

1. Travail initial sur la branche `main`
2. Création d'une branche `refonte` pour la modularisation
3. Développement du module sur la branche `refonte`
4. Fusion de `refonte` dans `main`
5. Nettoyage des branches

## 🛠️ Technologies

- **Langage** : Python 3
- **Versioning** : Git / GitHub
- **Modules** : datetime (bibliothèque standard Python)

## 👤 Auteur

**SNZAMBA65**

## 📝 Notes

Ce projet a été réalisé dans le cadre d'un TP sur Git pour apprendre les bonnes pratiques de versioning et de collaboration.