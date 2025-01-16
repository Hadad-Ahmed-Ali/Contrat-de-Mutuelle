# NOTE:
Le fichier HTML ci-joint contient le rapport du projet. Pour l'ouvrir, veuillez cliquer dessus. Vous verrez alors un code source. Cliquez sur l'icône en forme de flèche pour le télécharger. Une fois téléchargé, vous pourrez consulter le rapport en l'ouvrant dans votre navigateur.

# Analyse de données de mutuelle sur la durée de contrat

Ce projet vise à analyser les données d’une mutuelle afin de mieux comprendre les comportements de ses adhérents en matière de durée de contrat. La variable principale étudiée est la durée entre la souscription et la rupture du contrat, un indicateur clé pour la mutuelle, car une tendance à la résiliation a été observée, souvent au profit d’autres mutuelles.

### L’objectif est double :

1. Identifier les facteurs qui influencent la rupture de contrat en fonction des caractéristiques des adhérents (âge, statut de propriétaire, catégorie socio-professionnelle, etc.).
2. Prédire la durée d’un contrat à partir de ces variables explicatives, en s’appuyant sur des approches statistiques et de modélisation.

Une base des doonnées clients, comprenant à la fois des adhérents actuels et des anciens clients, nous a été mis à disposition. Ce jeu de données inclut des variables descriptives et des informations temporelles (date de souscription et de fin d’observation).

### Le projet se déroule en trois étapes principales :

1. Analyse descriptive des données (statistiques descriptives univariées et bivariées) pour comprendre les profils des adhérents et leurs comportements.
2. Une analyse non-paramétrique à l’aide de l’estimateur de Kaplan-Meier et des tests de log-rank pour étudier les différences de survie entre groupes de profils.
3. La mise en œuvre de modèle de régression pour expliquer les raisons associées à la rupture du contrat et d’améliorer la compréhension des dynamiques sous-jacentes.

# Conclusion de l'analyse : 

Grâce à une combinaison d’approches descriptives, non-paramétriques et de modélisation, plusieurs enseignements majeurs ont été dégagés:

**Analyse descriptive:**

L’analyse univariée et bivariée des données a mis en évidence que des facteurs tels que le sexe, l’âge, et la catégorie socio-professionnelle ont une influence notable sur la durée des contrats. Les adhérents masculins, les cadres, et les retraités présentent des durées de contrat plus longues, tandis que les femmes et certaines catégories socio-professionnelles comme les agriculteurs affichent une tendance à résilier plus rapidement. La durée moyenne des contrats est de 10,77 ans, avec une médiane de 11 ans, illustrant une certaine stabilité pour une grande partie des adhérents.

**Estimateur de Kaplan-Meier et tests log-rank:**

Les analyses non-paramétriques ont confirmé que des variables comme le sexe et la catégorie professionnelle impactent significativement la durée des contrats, tandis que le statut de propriétaire ne présente pas d’effet significatif. Les courbes de survie montrent que les **cadres** et les **hommes** ont une probabilité de résiliation plus faible sur la durée. Ces résultats offrent une base solide pour orienter les stratégies de fidélisation vers les segments les plus à risque.

**Modèles de régression (Cox et AFT):**

Les modèles de régression ont affiné la compréhension des dynamiques sous-jacentes :

- Le modèle de **COX** a montré un effet significatif de l’âge (HR = 1,015) : les adhérents plus âgés sont initialement plus à risque de résiliation, mais cet effet diminue avec le temps. Les **cadres** (HR = 0,533) sont également moins susceptibles de résilier leurs contrats.

- Le modèle **AFT** a révélé que les adhérents plus âgés, les hommes, et les cadres ont des durées de contrat plus longues. En revanche, les propriétaires de leurs logements présentent une durée de contrat plus courte, ce qui suggère un comportement spécifique à cette catégorie.


**Implications stratégiques:**

Ces résultats offrent des pistes concrètes pour la mutuelle :

- **Stratégies de fidélisation ciblées :** Mettre en place des offres spécifiques pour les segments les plus à risque, comme les femmes et certaines catégories professionnelles (agriculteurs, employés).

- **Optimisation des campagnes :** Renforcer la fidélisation des profils stables (hommes, cadres, retraités) par des avantages durables, tout en étudiant les besoins spécifiques des propriétaires pour comprendre leur plus grande propension à résilier.


# Outil utilisé : R ( outil demandé par mon prof ), sinon je pourrais le faire avec Python
