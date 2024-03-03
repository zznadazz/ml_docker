L'électroencéphalogramme (EEG) est un modèle de signal obtenu en amplifiant et en enregistrant le potentiel biologique spontané du cerveau sur le cuir chevelu. Il a été démontré que ce potentiel reflète l'activité macroscopique de la surface du cerveau et est généralement acquis à l'aide d'électrodes non invasives appliquées sur le cuir chevelu.

Le but du projet est d'entraîner deux modèles : un réseau de neurones (perceptron multicouche) ainsi qu'une Analyse Discriminante Linéaire (LDA) pour classifier les données.

Le script `train.py` est un script Python qui ingère et normalise les données EEG dans un fichier CSV (`train.csv`) et entraîne les deux modèles pour classer les données à l'aide de la bibliothèque scikit-learn. Le script enregistre deux modèles : l'Analyse Discriminante Linéaire (`clf_lda`) et le perceptron multicouche des réseaux de neurones (`clf_NN`).

Le script `inference.py` est appelé pour effectuer une inférence par lots en chargeant les deux modèles précédemment créés. L'application normalise les nouvelles données EEG provenant d'un fichier CSV (`test.csv`), effectue des inférences sur l'ensemble de données et affiche l’accuracy de la classification ainsi que les prédictions.

Enfin, le projet est dockernisé pour faciliter son déploiement et son exécution dans différents environnements.
