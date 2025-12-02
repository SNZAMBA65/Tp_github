# TP Git - Apprendre les branches

Un petit projet pour s'entraîner sur Git. Le but est d'apprendre à créer des branches, faire des commits, fusionner le tout et pousser ça sur GitHub.

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

## Ce qu'il faut retenir
Au début, j'ai fait un fichier simple sur la branche `main`. Ensuite j'ai créé une branche `refonte` pour réorganiser le code et créer un module séparé. Une fois que c'était bon, j'ai fusionné tout ça dans `main` et nettoyé la branche `refonte`.

Pas très compliqué finalement, mais c'est cool de voir comment Git gère tout ça !

## Installation

Rien de spécial à installer, juste Python 3. Le module `datetime` est déjà inclus dans Python.

---

Fait par Samir dans le cadre d'un TP sur Git