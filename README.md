# Analyse de Données avec AdventureWorks - Microsoft
Ce projet d'analyse de données se concentre sur le nettoyage, la transformation et la visualisation des données de l'entrepôt AdventureWorks, fourni par Microsoft. L'objectif principal était d'extraire et de préparer les données nécessaires à l'analyse des ventes, des clients et des produits, en utilisant SQL pour la manipulation des données et Power BI pour la création de tableaux de bord dynamiques.
## Objectifs du Projet
- Nettoyer les données brutes en sélectionnant les colonnes essentielles pour l'analyse.
- Extraire uniquement les tables nécessaires via des requêtes SQL.
- Créer des visualisations interactives pour l'analyse des ventes, des clients et des produits.

## Nettoyage des Données :
### 1. Table DimDate :
J'ai commencé par nettoyer la table DimDate en sélectionnant uniquement les colonnes essentielles telles que la date complète, le jour de la semaine, le nom du mois et son abréviation, ainsi que les numéros de mois, trimestre et année. Seules les données à partir de 2019 ont été retenues pour une analyse plus récente et pertinente.
### 2. Table DimCustomer :
Ensuite, j'ai nettoyé la table DimCustomer en conservant uniquement les colonnes pertinentes pour l'analyse des clients. Les informations clés incluent : prénom, nom de famille, nom complet (concaténation du prénom et du nom), genre (transformé en 'Male' ou 'Female'), date du premier achat, et la ville de résidence (via une jointure avec DimGeography).
### 3. Table DimProduct :
Pour l'analyse des produits, j'ai sélectionné les colonnes importantes telles que le code produit, le nom en anglais, la couleur, la taille, la ligne de produits et le modèle. J'ai également ajouté les sous-catégories et catégories de produits grâce à des jointures avec les tables DimProductSubcategory et DimProductCategory. Les produits sans statut spécifié ont été marqués comme 'Outdated' par défaut.
### 4. Table FactInternetSales :
Pour l'analyse des ventes en ligne, j'ai retenu des informations essentielles comme le ProductKey, les dates de commande, de livraison et d'échéance, le numéro de commande, et le montant des ventes (SalesAmount). Les colonnes non pertinentes, comme celles liées aux promotions ou aux remises, ont été exclues, et seules les ventes des quatre dernières années ont été incluses pour se concentrer sur les données récentes.

## Visualisations :

Grâce à Power BI, des tableaux de bord dynamiques ont été créés pour fournir des insights clés sur les ventes, les clients et les produits. Ces visualisations permettent de mieux comprendre les tendances des ventes, la répartition des produits, et le comportement des clients.
=======
>>>>>>> 7232b72 (first commit)
