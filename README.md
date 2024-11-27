# Analyse de données de mutuelle sur la durée de contrat

Ce projet vise à analyser les données d’une mutuelle afin de mieux comprendre les comportements de ses adhérents en matière de durée de contrat. La variable principale étudiée est la durée entre la souscription et la rupture du contrat, un indicateur clé pour la mutuelle, car une tendance à la résiliation a été observée, souvent au profit d’autres mutuelles.

L’objectif est double :

1. Identifier les facteurs qui influencent la rupture de contrat en fonction des caractéristiques des adhérents (âge, statut de propriétaire, catégorie socio-professionnelle, etc.).
2. Prédire la durée d’un contrat à partir de ces variables explicatives, en s’appuyant sur des approches statistiques et de modélisation.

La mutuelle a prélevé un échantillon de 953 clients, comprenant à la fois des adhérents actuels et des anciens clients, qui nous a été mis à disposition. Ce jeu de données inclut des variables descriptives et des informations temporelles (date de souscription et de fin d’observation).

Le projet se déroule en trois étapes principales :

1. Analyse descriptive des données (statistiques descriptives univariées et bivariées) pour comprendre les profils des adhérents et leurs comportements.
2. Une analyse non-paramétrique à l’aide de l’estimateur de Kaplan-Meier et des tests de log-rank pour étudier les différences de survie entre groupes de profils.
3. La mise en œuvre de modèle de régression pour expliquer les raisons associées à la rupture du contrat et d’améliorer la compréhension des dynamiques sous-jacentes.


# Outil utilisé : R
