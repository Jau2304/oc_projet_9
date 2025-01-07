# Traitement Big Data sur le Cloud pour "Fruits!"

## Contexte du Projet

"Fruits!" est une start-up innovante dans le secteur de l'AgriTech, ayant pour mission de préserver la biodiversité des fruits grâce au développement de robots cueilleurs intelligents. La société cherche à sensibiliser le grand public à cette biodiversité en mettant à disposition une application mobile permettant aux utilisateurs de prendre des photos de fruits et d’obtenir des informations sur ces fruits. Cette application mobile sera également le point de départ pour la mise en place d'une architecture Big Data capable de gérer une croissance rapide du volume de données.
Objectifs du Projet

L'objectif de cette mission est de compléter une chaîne de traitement de données dans un environnement Big Data sur le Cloud (AWS EMR ou Databricks), en vue de créer une infrastructure évolutive pour traiter les données de l’application mobile et préparer le passage à l’échelle. Il ne s'agit pas d’entraîner un modèle pour le moment, mais de créer les premières briques de traitement qui seront nécessaires pour gérer un grand volume de données à l'avenir.

Les objectifs spécifiques incluent :

1. Compléter et améliorer la chaîne de traitement existante :
- Prendre en main le travail de l'alternant et étendre les scripts en PySpark pour intégrer des traitements Big Data évolutifs.
- Compléter le script avec le traitement de diffusion des poids du modèle TensorFlow (broadcast des “weights” du modèle).
- Ajouter une étape de réduction de dimension avec PCA en PySpark.

2. Mise en place d’une instance EMR sur AWS :
- Créer une instance EMR sur AWS et démontrer sa mise en place opérationnelle.
- Expliquer et détailler chaque étape du script PySpark que vous aurez complété.

3. Respect des contraintes du RGPD :
- Paramétrer l’installation afin que les serveurs utilisés soient situés sur le territoire européen.

4. Gestion des coûts :
- S’assurer que les coûts restent inférieurs à 10 euros en optimisant l’utilisation de l’instance EMR et en utilisant un serveur local pour le développement du script PySpark.

## Données

Le projet utilise un jeu de données constitué d'images de fruits, avec les labels associés. Ce jeu de données est disponible en téléchargement et servira à tester les traitements que vous mettez en place. L'objectif n'est pas d’entraîner un modèle complet, mais de préparer les étapes nécessaires à un traitement à grande échelle.

## Méthodologie

1. Appropriation des travaux de l'alternant
- Analyser et comprendre le travail réalisé par l’alternant dans l’environnement Big Data AWS EMR.
- Identifier les points manquants et les compléments nécessaires pour finaliser la chaîne de traitement.

2. Traitement de diffusion des poids du modèle TensorFlow
- Utiliser PySpark pour diffuser les poids d'un modèle TensorFlow à travers les clusters (technique du broadcast).
- S’appuyer sur des ressources disponibles (comme l’article “Model inference using TensorFlow Keras API”) pour comprendre et implémenter cette fonctionnalité.

3. Réduction de dimension avec PCA en PySpark
- Implémenter une étape de réduction de dimension à l’aide de la méthode PCA (Principal Component Analysis) en utilisant PySpark.
- Assurer une bonne gestion des données à grande échelle et une exécution efficace des calculs.

4. Mise en place d’une instance EMR sur AWS
- Créer une instance EMR sur AWS et configurer l'environnement pour effectuer des traitements de données à grande échelle.
- Tester et démontrer le fonctionnement de cette instance dans le cadre des traitements mis en place (en veillant à respecter les contraintes de coût).

5. Respect du RGPD et gestion des coûts
- Configurer les instances et les traitements afin que les données soient traitées dans des serveurs localisés sur le territoire européen pour être en conformité avec le RGPD.
- Optimiser l'utilisation de l'instance EMR en la maintenant opérationnelle uniquement pour les tests et les démonstrations, tout en limitant les coûts liés à son fonctionnement (moins de 10 euros).

## Outils et Technologies

Les outils et technologies utilisés pour ce projet incluent :
- PySpark : pour le traitement des données à grande échelle, l’utilisation de Spark permet de manipuler de gros volumes de données efficacement.
- AWS EMR : pour l'hébergement et le traitement des données dans un environnement Big Data.
- TensorFlow / Keras : pour la gestion du modèle de machine learning, ainsi que pour la diffusion des poids sur les clusters.
- PCA : pour la réduction de dimension des données.
- AWS S3 : pour le stockage des données et des modèles.
- AWS IAM : pour gérer les permissions et la sécurité des accès.
- Docker : pour compartimenter le projet avant déploiement.

## Résultats Attendus

À la fin de cette mission, l’objectif est d’avoir mis en place une chaîne de traitement Big Data complète pour l’application mobile de "Fruits!", avec les étapes suivantes :
- Script PySpark opérationnel : Traitement des données d’images de fruits et diffusion des poids du modèle TensorFlow sur les clusters.
- Réduction de dimension avec PCA : Application de la réduction de dimension à l’échelle des données.
- Instance EMR fonctionnelle : Mise en place et démonstration d'une instance EMR opérationnelle sur AWS, en respectant les coûts et les contraintes RGPD.
- Documentation et démonstration : Fourniture d’une explication détaillée des étapes mises en place, et d'une démonstration de l’instance EMR avec le script PySpark.

Cette architecture Big Data pourra être ensuite utilisée à l'échelle lorsque le volume des données augmentera avec le développement de l’application mobile. Les solutions mises en place seront une base solide pour le futur traitement des données et l’entraînement de modèles de machine learning.
