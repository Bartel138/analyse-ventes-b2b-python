# 📊 Projet d'Analyse Exploratoire des Ventes (Sales EDA)

Ce projet de science des données a pour objectif de réaliser une Analyse Exploratoire des Données (EDA) complète sur un jeu de données de ventes B2B/B2C. Il couvre l'ensemble du cycle de vie du projet : de la structuration initiale du dépôt GitHub et du nettoyage des données jusqu'à la visualisation et l'analyse métier des performances commerciales.

---

## 📂 Structure du Projet

Le projet est organisé de manière modulaire pour garantir la reproductibilité et la clarté du code :
- data/ : Jeux de données bruts et nettoyés
- notebooks/ : Notebooks Jupyter de l'analyse exploratoire
- src/ : Scripts sources (modules de nettoyage et fonctions utilitaires)
- assets/ : Graphiques et exports visuels
- README.md : Documentation du projet
- requirements.txt : Dépendances et bibliothèques Python

---

## 🧹 1. Nettoyage et Mise en Conformité des Données

Avant toute analyse, un travail rigoureux de préparation et de nettoyage des données a été mené :
* Gestion des Dates : Conversion et formatage des variables temporelles pour permettre une indexation et un regroupement temporel précis (analyse de la saisonnalité mensuelle).
* Traitement des Nombres : Vérification, typage rigoureux et contrôle des variables numériques (TotalPrice, UnitPrice, Quantity) pour éviter les erreurs de calcul ou d'agrégation.
* Standardisation des Textes : Uniformisation des variables textuelles et catégorielles (catégories de produits, régions) afin de garantir la fiabilité des regroupements.

---

## 📈 2. Analyse Exploratoire et Visualisations Clés

L'analyse macro-économique des ventes s'appuie sur un Design System cohérent et des graphiques statistiques avancés (réalisés via seaborn et matplotlib) :

### A. Évolution Mensuelle du Chiffre d'Affaires
* Tendances et saisonnalité : La courbe met en évidence une dynamique annuelle irrégulière marquée par des pics de performance majeurs en décembre (mois 12), juin (mois 6) et mars (mois 3).
* Périodes de creux : Des ralentissements notables sont observés au démarrage de l'année, au printemps (mois 4) ainsi qu'une transition plus creuse entre juillet et novembre.

### B. Répartition par Catégories de Produits
* Dominance de l'Électronique : La catégorie Electronics représente 62,3 % du chiffre d'affaires global.
* Complémentarité des Accessoires : La catégorie Accessories pèse pour 37,7 %, portée par des volumes réguliers mais des prix unitaires plus faibles.

### C. Répartition Géographique
* Équilibre territorial : Toutes les régions enregistrent un chiffre d'affaires supérieur à 500 000 €.
* Locomotives : Les régions South et West s'imposent comme les moteurs commerciaux principaux de l'entreprise.

### D. Distributions Statistiques (Panier, Prix et Quantités)
* Montant des commandes (Panier) : Un histogramme combiné à une courbe de densité met en lumière une forte concentration sur les paniers intermédiaires et bas, complétée par une longue traîne de commandes exceptionnelles à forte valeur.
* Prix unitaires et Quantités : L'analyse de la structure du catalogue (UnitPrice) et des volumes par transaction (Quantity) confirme une répartition homogène des tailles de lots et des gammes de prix.

---

## 🚀 Prochaines Étapes
* Approfondissement de la structure des paniers via une analyse de type Loi de Pareto (80/20).
* Segmentation avancée de la clientèle et modélisation prédictive.