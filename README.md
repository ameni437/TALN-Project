# Projet TALN

## Titre du Projet : Analyse de la Cohérence Inter-phrastique en langue arabe à travers la similarité des paires de phrases


Ce projet est une étude approfondie de l'analyse de la cohérence inter-phrastique en langue arabe en utilisant des techniques avancées de traitement automatique du langage naturel (TALN). Voici une description détaillée du code et de la méthodologie utilisée :

##Nettoyage et Préparation des Données
Nettoyage du Texte : Le texte est nettoyé pour enlever les chiffres, les crochets et les lettres non-arabes. Cela permet d'obtenir un texte plus propre pour l'analyse.
Extraction des Phrases : Le texte nettoyé est divisé en phrases individuelles à l'aide d'expressions régulières, ce qui est essentiel pour l'analyse de la cohérence entre les phrases.
##Création de Paires de Phrases
Paires Consécutives : Des paires de phrases consécutives sont formées. Ces paires sont destinées à représenter des segments de texte où l'on s'attend à une forte cohérence.
Paires Aléatoires : Des paires de phrases aléatoires sont également créées pour servir de comparaison. Ces paires sont susceptibles de montrer une faible cohérence.
##Analyse de la Similarité avec BERT
Utilisation de BERT : Le modèle BERT multilingue est utilisé pour extraire les caractéristiques de chaque phrase.
Calcul de la Similarité : La similarité entre les phrases de chaque paire est calculée en utilisant la similarité cosinus, une mesure standard pour évaluer la proximité entre deux vecteurs dans un espace vectoriel.
##Annotation Automatique
Annotation en Fonction des Scores : Les scores de similarité sont utilisés pour annoter automatiquement les paires de phrases avec des valeurs indiquant le degré de cohérence (de 1 à 5).
Agrégation et Analyse des Scores
Agrégation des Scores : Les scores de similarité sont agrégés pour évaluer la cohérence à différents niveaux (au niveau du paragraphe, entre les paragraphes, et pour l'ensemble du texte).
Analyse des Résultats : Une analyse détaillée est effectuée pour identifier les zones où la cohérence est perçue différemment, offrant ainsi une compréhension nuancée de la cohérence dans le texte arabe.
##Utilisation de Word2Vec
Entraînement de Word2Vec : Un modèle Word2Vec est entraîné sur les phrases pour obtenir une autre perspective sur la similarité entre elles.
Comparaison avec les Annotations BERT : Les annotations générées par Word2Vec sont comparées à celles de BERT pour examiner les différences dans la perception de la cohérence.
##Visualisation des Données
Graphiques : Des graphiques sont utilisés pour visualiser et comparer les annotations automatiques obtenues par BERT et Word2Vec, facilitant ainsi l'interprétation des résultats.
