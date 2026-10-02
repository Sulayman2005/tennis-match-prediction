# CLAUDE.md · Projet fil rouge B3 Data & IA

> Ce fichier est lu automatiquement par Claude Code à chaque session. Complétez les sections marquées « à remplir » dès le J1.

## Le projet

- **Nom** : à remplir
- **Groupe** : à remplir (prénoms + qui porte quoi)
- **Question** : voir `docs/brain/fiche-projet.md`
- **Cadre** : module Data & IA, B3 DEV Sup de Vinci Nantes. 4 jalons : J1 cadrage, J2 modèle, J3 application, J4 déploiement + soutenance.

## Le second brain : `docs/brain/`

C'est la mémoire du projet, en Markdown, versionnée avec le code. Tu t'en sers à chaque session.

- **Au début de chaque session** : lis `docs/brain/00-index.md` puis le dernier fichier de `docs/brain/journal/`.
- **Pendant** : une décision (choix de dataset, de feature, de modèle, de métrique) va dans `docs/brain/decisions/` (commande `/decision`) ; un terme nouveau va dans `docs/brain/glossaire.md` ; une question pour le formateur va dans `docs/brain/questions.md` ; ce qu'on apprend du dataset va dans `docs/brain/dataset.md`.
- **À la fin de chaque session** : commande `/journal`.
- Ne réécris jamais un fichier du brain en entier : ajoute ou modifie la partie concernée.

## Méthode de travail

1. **Explore** : lis les fichiers concernés et explique ce que tu comprends avant de proposer un changement.
2. **Plan** : pour toute tâche non triviale, propose un plan et attends la validation.
3. **Implement** : petites étapes, une intention à la fois.
4. **Verify** : exécute, montre le résultat réel. Tant que ce n'est pas vérifié, ce n'est pas fait.

Principes : réfléchir avant de coder et **demander plutôt que deviner** · **la simplicité d'abord**, pas de fonctionnalité spéculative · **changements chirurgicaux**, ne toucher que ce qui est demandé · transformer chaque demande floue en **critère vérifiable**.

Les membres du groupe doivent comprendre chaque ligne : explique ce que tu changes et pourquoi, en français, simplement. Propose des options, ne décide pas à leur place.

## Règles data (non négociables)

- Séparer train et test **avant** tout preprocessing (imputation, normalisation, encodage) ; `random_state=42`.
- Aucune feature qui ne serait pas connue au moment de la prédiction (fuite de données).
- Toujours comparer à une **baseline naïve** (moyenne, classe majoritaire).
- Un chiffre écrit dans le README ou le brain vient d'une exécution réelle, avec le notebook ou le script qui le produit. **Ne jamais inventer un résultat.**
- Les notebooks tournent de haut en bas sans erreur.
- Ne jamais modifier ni supprimer les données brutes (`data/raw/`).

## Stack et commandes

- Python 3.11+ · Pandas · PySpark 3.5 (une étape) · Scikit-learn · puis FastAPI (J3), React (J3), Docker + Hugging Face Spaces (J4)
- Installation : `python -m venv .venv && source .venv/bin/activate && pip install -r requirements.txt`
- Notebooks : `jupyter lab` (ou Google Colab)

## À ne pas faire

- Pas de secret (clé API, mot de passe, token) dans le code ou dans Git : `.env` uniquement, déjà ignoré.
- Pas de `git push --force`, pas de réécriture globale d'un fichier qui marche.
- Pas de nouvelle librairie sans le dire et l'ajouter à `requirements.txt`.
