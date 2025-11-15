## Tous les scripts du projet

C’est le cœur technique du projet.

`src/data_load.py` il est charger les données.

Ce fichier contient du code pour :
- charger le CSV depuis `data/raw/`
- vérifier les colonnes
- supprimer les doublons
- renvoyer un DataFrame propre

`src/preprocess.py` il sert a nettoyer le texte

Contient :
- suppression des emails, URLs, numéros
- lemmatisation
- normalisation
- transformation en texte prêt pour ML

`src/features.py` sert a transformer le texte en features

Contient :
- TF-IDF Vectorizer
- Bag-of-Words
- embeddings (optionnel)

`src/train_tfidf_svm.py` sert a entraînement du modèle baseline TF-IDF + SVM

Script qui :
- charge les données
- applique preprocess
- vectorise
- entraîne un SVM
- évalue
- sauvegarde le modèle dans `models/`
 _Baseline simple et efficace._

`src/train_bert.py` fine-tuning BERT / CamemBERT

Ce fichier :
- prépare le dataset HF
- tokenise les textes
- paramètre l'entraînement
- entraîne un modèle BERT
- sauvegarde le modèle dans `/models`

`src/extract_skills.py` extraction automatique des compétences

Contient :
- extraction par dictionnaire
- match fuzzy
- ou pipeline NER

`src/evaluate.py` évaluer les modèles

Mesure :
- précision, rappel, F1-score
- matrice de confusion
- comparaison TF-IDF vs BERT
- rapport complet

``