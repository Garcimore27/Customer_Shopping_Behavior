🛒 Customer Shopping Behavior Analysis

📌 Description du projet

Ce projet vise à analyser le comportement d'achat des clients à partir de données transactionnelles afin d’identifier des tendances clés, des segments de clientèle et des leviers d’optimisation business.

L’analyse repose sur 3 900 transactions clients couvrant plusieurs catégories de produits et intègre :

Python pour la préparation et l’analyse exploratoire,

SQL (PostgreSQL) pour l’analyse métier,

Power BI pour la visualisation des résultats.

🎯 Objectifs

Comprendre les habitudes de dépenses des clients

Identifier des segments de clientèle pertinents

Analyser l’impact des remises et abonnements

Mettre en évidence les produits les plus performants

Fournir des recommandations stratégiques basées sur les données

📊 Dataset

Nombre de lignes : 3 900

Nombre de colonnes : 18

Principales variables
🧍 Démographie client

Âge

Sexe

Localisation

Statut d’abonnement

🛍️ Détails des achats

Produit acheté

Catégorie

Montant de l’achat

Saison

Taille

Couleur

🔁 Comportement d’achat

Remise appliquée

Code promotionnel utilisé

Nombre d’achats précédents

Fréquence d’achat

Note d’avis

Type d’expédition

⚠️ Données manquantes

37 valeurs manquantes dans la colonne note des avis

🐍 Analyse exploratoire des données (Python)
Étapes réalisées

Chargement des données

Import du dataset avec pandas

Exploration initiale

Analyse de la structure avec df.info()

Statistiques descriptives via df.describe()

Gestion des données manquantes

Détection des valeurs nulles

Imputation des notes manquantes par la médiane de la catégorie produit

Nettoyage et standardisation

Renommage des colonnes en snake_case

Vérification de la cohérence des données

Feature Engineering

Création de la variable age_group

Création de la variable purchase_frequency_days

Optimisation des variables

Détection de la redondance entre discount_applied et promo_code_used

Suppression de promo_code_used

Stockage des données

Connexion à une base PostgreSQL

Chargement du DataFrame nettoyé pour analyse SQL

🗄️ Analyse des données (SQL – MySQL)

Les analyses suivantes ont été réalisées pour répondre aux questions métier :

💰 Revenus par genre

🏷️ Clients utilisant des remises avec dépenses élevées

⭐ Top 5 des produits par note moyenne

🚚 Comparaison des montants d'achat par type d’expédition

🔄 Abonnés vs non-abonnés

📉 Produits les plus dépendants des remises

👥 Segmentation client :

Nouveau

Retour

Fidèle

🥇 Top 3 des produits par catégorie

🔔 Lien entre achats fréquents et abonnement

🎂 Revenus par groupe d’âge

📈 Data Visualization – Power BI

Un tableau de bord interactif Power BI a été conçu pour :

Explorer les indicateurs clés

Comparer les segments clients

Faciliter la prise de décision business

![Example Power BI](Capture d'écran 2025-12-17 142455.png)

💡 Recommandations business

🚀 Développer les abonnements

Offrir des avantages exclusifs aux abonnés

❤️ Renforcer la fidélisation

Mettre en place des programmes de récompense pour les clients réguliers

📊 Optimiser les politiques de remise

Trouver un équilibre entre augmentation des ventes et marges

🛍️ Valoriser les produits performants

Mettre en avant les produits les mieux notés et les plus vendus

🎯 Marketing ciblé

Prioriser les groupes d’âge à forte croissance

Cibler les utilisateurs de l’expédition express

🛠️ Technologies utilisées

Python (pandas, numpy)

PostgreSQL

SQL

Power BI

Git / GitHub

📌 Résultats clés chiffrés
💰 Chiffre d’affaires par genre

Hommes : 157 890

Femmes : 75 191

➡️ Les clients masculins génèrent plus du double du chiffre d’affaires par rapport aux clientes, indiquant un potentiel de croissance côté clientèle féminine.

🏷️ Impact des remises sur les dépenses

839 clients ont utilisé une remise tout en dépensant au-dessus du montant moyen

Certains achats avec remise atteignent des montants compris entre 80 et 97

➡️ Les remises ne réduisent pas systématiquement la valeur des paniers et peuvent stimuler des achats plus élevés.

⭐ Top 5 des produits par note moyenne
Produit	Note moyenne
Gloves	3.86
Sandals	3.84
Boots	3.82
Hat	3.80
Skirt	3.78

➡️ Ces produits constituent des candidats prioritaires pour les campagnes marketing et la mise en avant commerciale.

🚚 Comparaison des types d’expédition
Type d’expédition	Montant moyen
Standard	58.46
Express	60.48

➡️ Les clients utilisant l’expédition Express dépensent en moyenne davantage, suggérant un lien entre rapidité et valeur du panier.

🔔 Abonnés vs Non-abonnés
Statut	Clients	Dépense moyenne	Chiffre d’affaires
Abonnés	1 053	59.49	62 645
Non-abonnés	2 847	59.87	170 436

➡️ Bien que la dépense moyenne soit similaire, les non-abonnés génèrent l’essentiel du chiffre d’affaires en raison de leur volume.
➡️ Fort potentiel de conversion vers l’abonnement.

📉 Produits les plus dépendants des remises
Produit	% d’achats avec remise
Hat	50.00 %
Sneakers	49.66 %
Coat	49.07 %
Sweater	48.17 %
Pants	47.37 %

➡️ Ces produits sont fortement sensibles aux promotions, ce qui nécessite un arbitrage entre volume et marge.

👥 Segmentation client
Segment	Nombre de clients
Fidèle	3 116
Retour	701
Nouveau	83

➡️ La base client est majoritairement composée de clients fidèles, indiquant une bonne rétention globale.

🥇 Top produits par catégorie (extraits)

Accessories : Jewelry (171), Sunglasses (161), Belt (161)

Clothing : Blouse (171), Pants (171), Shirt (169)

Footwear : Sandals (160), Shoes (150), Sneakers (145)

Outerwear : Jacket (163), Coat (161)

➡️ Ces produits dominent leurs catégories respectives en volume de commandes.

🔁 Acheteurs réguliers et abonnements

Clients non abonnés (>5 achats) : 2 518

Clients abonnés (>5 achats) : 958

➡️ Les acheteurs fréquents sont plus susceptibles de s’abonner, confirmant la pertinence d’une stratégie de fidélisation ciblée.

🎂 Chiffre d’affaires par groupe d’âge
Groupe d’âge	Chiffre d’affaires
Young Adult	62 143
Middle-aged	59 197
Adult	55 978
Senior	55 763

➡️ Les jeunes adultes constituent le segment le plus contributeur au chiffre d’affaires.
