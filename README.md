# Analyse de données de mutuelle sur la durée de contrat

Dans ce projet, on analyse des données de mutuelle concernant ses adhérents. La variable d’intérêt est la durée qui s’écoule entre la date de souscription et la rupture du contrat. Cette variable est importante pour la mutuelle car elle a constaté que des adhérents ont tendance à rompre leur contrat pour changer de mutuelle. 

Le but est donc de pouvoir déterminer les raisons qui poussent certains adhérents à rompre leur contrat et éventuellement à pouvoir prédire la durée du contrat d’un adhérent en fonction de certaines de ses caractéristiques. 

Pour cela, la mutuelle a prélevé un échantillon de 953 personnes parmi ses clients et ancien clients et, pour chacun d’entre eux, elle dispose des covariables suivantes :
1. AGE : en années.
2. PROP : est-ce que l’adhérent est propriétaire de son logement ? 1 Oui, 0 Non.
3. HOMME : 1 si l’adhérent est un homme, 0 si c’est une femme.
4. PROF : la catégorie socio-professionnelle qui contient huit modalités, codées de la façon suivante.
    1 agriculteur, 2 artisan, 3 cadre, 4 profession intermédiaire, 5 employé, 6 ouvrier, 7 retraité, 8 autre.

On dispose en outre des variables DEBUT et FINOBS qui permettent de construire les variables de temps observé et d’indicateur de censure.
DEBUT représente la date (en années) où l’adhérent a souscrit à sa mutuelle et FINOBS représente soit la date (en années) où l’adhérent a arrêté sa souscription (si la date est inférieure à 2015.80), soit la date 2015.80, qui correspond à la date d’extraction des données, et qui signifie que la personne est toujours adhérente à la mutuelle.

Les objectifs demandés par la mutuelle, il nous est demandé d’effectuer les analyses suivantes:
Nous devons aborder, et en fin apporter une conclusion, des analyses précises sur:

1. Analyse descriptive des données (statistiques descriptives univariées et bivariées) pour comprendre les profils des adhérents et leurs comportements.
2. Analyses non-paramétriques des données (estimateur de Kaplan-Meier, tests du log-rang etc.) pour analyser les différences de survie entre groupes de profils.
3. Implémentation de deux modèles de régression pour expliquer les raisons associées à la rupture du contrat.


# Outil utilisé : R
