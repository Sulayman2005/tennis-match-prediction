# Nom du projet

> Projet fil rouge · Data & IA · B3 DEV Sup de Vinci Nantes · 2026-2027. Remplacez chaque bloc. **Jalon J1** : sections 1 à 4 remplies.

**Groupe** : Prénom NOM · Prénom NOM · Prénom NOM
**Qui porte quoi** : données · modèle · API · interface · déploiement

## 1 · La question

Une phrase : « Prédire **X** à partir de **Y**, pour aider **Z** à décider **W**. » (détail : [fiche projet](docs/brain/fiche-projet.md))

## 2 · Le dataset

| | |
|---|---|
| Source | lien + producteur |
| Licence | ex. Licence Ouverte Etalab, CC BY 4.0 |
| Taille | lignes × colonnes |
| Une ligne représente | ex. un match, une transaction, un patient |
| Période couverte | |
| Deuxième source (optionnel) | lien + pourquoi |

Dictionnaire des colonnes : [docs/brain/dataset.md](docs/brain/dataset.md)

## 3 · La fiche projet

| Rubrique | Votre réponse |
|---|---|
| **Cible y** | la colonne à prédire |
| **Type de problème** | régression / classification (+ clustering en bonus) |
| **Features X** | 5 à 10 variables, connues AVANT le moment de la prédiction |
| **Métrique** | MAE, RMSE, R², accuracy, F1… et pourquoi |
| **Baseline naïve** | le score à battre |
| **Risques** | fuite de données, biais, taille, manquants, et votre parade |

## 4 · Premiers constats

3 à 5 constats tirés de `notebooks/01-exploration.ipynb`.

## 5 · Lancer le projet

```
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

## 6 · Architecture

À compléter au J3 (schéma mermaid bienvenu).

## 7 · Résultats et limites

À compléter au J2 puis au J4.

## Mémoire du projet

Le second brain est dans [`docs/brain/`](docs/brain/00-index.md) : état du projet, décisions, journal des séances, glossaire, questions. Règles pour l'agent de code : [`CLAUDE.md`](CLAUDE.md).
