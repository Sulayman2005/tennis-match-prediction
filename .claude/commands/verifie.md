Vérifie l'état du projet sans rien corriger, puis fais-moi un rapport.

1. Chaque notebook de `notebooks/` s'exécute-t-il de haut en bas ? (`jupyter nbconvert --to notebook --execute --output /tmp/check.ipynb <notebook>`)
2. Les chiffres cités dans `README.md` et `docs/brain/` correspondent-ils aux sorties des notebooks ?
3. Le split train/test est-il fait avant tout preprocessing ? Une feature pourrait-elle contenir la réponse ou venir du futur ?
4. Y a-t-il un secret dans le code ou l'historique Git (`git log -p | grep -i -E "api_key|token|password|secret"`) ?
5. Liste les écarts par gravité. Propose les corrections, n'applique rien sans mon accord.
