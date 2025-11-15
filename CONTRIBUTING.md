## Contribuer au projet

Tout d'abord, merci de votre intérêt pour `cv-classifier` ! Nous accueillons avec plaisir les contributions qui nous permettent d'améliorer le projet, qu'il s'agisse de nouvelles fonctionnalités, de corrections de bugs, d'améliorations de la documentation ou de tests plus poussés. Vous trouverez ci-dessous nos instructions pour contribuer.

## Structure du dépôt

Notre dépôt est organisé comme un espace de travail python et clairement structuré pour séparer chaque fonctionnalite. Voici un aperçu du dossier principal :

```bash
cv-classifier/
├─ data/
│ ├─ raw/
│ ├─ processed/
├─ notebooks/
├─ src/
│ ├─ data_load.py
│ ├─ preprocess.py
│ ├─ features.py
│ ├─ train_tfidf_svm.py
│ ├─ train_bert.py
│ ├─ extract_skills.py
│ ├─ evaluate.py
│ └─ api.py
├─ models/
├─ experiments/
└─ README.md
```

> _Vous trouverais un fichier README.md dans chaque dossier pour expliquer chaque fichier et dossier_

### Commencer

1. Forkez et clonez le dépôt
    - Forkez le dépôt sur GitHub.
    - Clonez votre fork localement :
        ```bash
        git clone git@github.com:[nom_user]/cv-classifier.git
        cd cv-classifier
        ```

2. Installer les LIBRARYs necessaire
    ```bash
    ```

3. Installer les dépendances
    - Examinez la structure du dépôt.
    - Examinez le code existant dans les `src/dossiers` et autres pour comprendre comment le projet est organisé.

4. Branchement et flux de travail
- Stratégie de branchement
    - Pour les nouvelles fonctionnalités ou les correctifs, veuillez créer une branche à partir de la `main` branche
    - Utilisez des noms de branches descriptifs, par exemple, `feature/new-componentou` `bugfix/fix-issue-123`
- Création d'une branche
    ```bash
    git checkout -b feature/your-feature-name
    ```
- Directives d'engagement
    - Rédigez des messages de commit clairs et concis.
    - Respectez la convention des messages de commit :
    ```bash
    [type]: short description
    ```
    où le **type** pourrait être `feat`(nouvelle fonctionnalité), `fix`(correction de bug), `docs`(documentation [REDME...]), etc.
    - Exemple de commit :
    ```bash
    feat: add support for custom hook in package XYZ
    ```

## Normes de codage et messages de validation

- Style de code
    - Respectez les conventions de codage établies dans le dépôt.
    - Veuillez vérifier la présence de fichiers de configuration de linting ou de style (par exemple, .eslintrc) pour garantir la cohérence.

- Messages de validation
    - Veillez à ce que les messages de commit soient descriptifs.
    - Si nécessaire, ajoutez une description détaillée dans le corps du commit, incluant des références à tous les problèmes que le commit résout.

- Exécution des tests
    - Avant de soumettre votre demande de fusion, assurez-vous que tous les tests réussissent.
    - Exécutez les tests depuis la racine du dépôt

- Tests sur le terrain de jeu
    - Testez vos modifications dans les `/` exemples pour vous assurer qu'elles fonctionnent dans des situations réelles.

## Processus de demande d'extraction

1. Soumettre une demande de fusion
    - Une fois vos modifications terminées et tous les tests réussis, ouvrez une demande de fusion (PR) sur la devbranche (ou comme spécifié).
        ```bash
        git add .
        git commit -m "[type]:message claire"
        git push origin nom_de_ta_branch
        ```
2. Description des relations publiques
    - Veuillez fournir une description claire de vos modifications.
    - Faites un lien vers tout problème connexe et expliquez votre raisonnement.

3. Faites un lien vers tout problème connexe et expliquez votre raisonnement.
    - Votre demande de modification sera examinée par les responsables de la maintenance.
    - Soyez prêt à prendre en compte les commentaires ou à apporter d'autres modifications.

4. Fusion
    - Nous pourrions vous demander de rebaser ou de fusionner vos commits avant la fusion afin de maintenir un historique propre.

5. Code de conduite
    - Nous nous engageons à créer une communauté conviviale, respectueuse et inclusive.
    - Veuillez consulter notre [Code of Conduct](CODE_OF_CONDUCT.md) avant de contribuer.

Merci de contribuer au succès de cv-classifier . Bon codage !