# ExercicesAPI_REST - FastAPI – API de personnages

## Réalisé par : Ilias

Ce projet est composé de 3 exercices réalisés avec FastAPI.

---

## Exercice 1 : Créer une API REST

- Création d'une API avec FastAPI
- Endpoint `/personnages` qui retourne une liste statique de personnages
- Fichier `personnages.json` ajouté pour documenter les données

Testé via : http://127.0.0.1:8000/docs

---

## Exercice 2 : Sécuriser l’accès avec un token

- Ajout d'un token dans les headers HTTP (`token`)
- Vérification du token dans l’endpoint `/personnages`
- Retourne une erreur 401 si le token est incorrect

Token utilisé pour les tests :  
```
token: super_token_123
```

---

## Exercice 3 : Ajouter CORS

- Activation du CORS avec `CORSMiddleware`
- Permet à des sites web (ex : HTML ou React) d'accéder à l’API
- Testé avec un fichier `index.html` qui affiche la liste des personnages

---

## Fichiers fournis

- `main.py` : Code FastAPI
- `personnages.json` : Données JSON
- `index.html` : Test via JavaScript
- `README.md` : Ce fichier de documentation

---

## Lancer le projet

```bash
uvicorn main:app --reload
```

Ouvrir ensuite :
- Swagger : http://127.0.0.1:8000/docs
- HTML local : double-cliquer sur `index.html`
