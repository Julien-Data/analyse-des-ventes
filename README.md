# Analyse des Ventes et du Comportement Clients – Librairie en Ligne

## 📌 Contexte

La librairie en ligne de l’entreprise Lapage existe depuis deux ans.  
Le nouveau responsable commercial souhaite faire un point global sur les indicateurs et chiffres clés de l’entreprise afin d’orienter la stratégie à suivre : création d’offres, adaptation des prix, ciblage de la clientèle, etc.

Cette analyse est réalisée à partir des fichiers clients, produits et transactions fournis.

---

## 🗂 Contenu du projet

Ce projet a été réalisé dans le cadre d’une formation en analyse de données.

Le dépôt contient :

- **`analyse-des-ventes.ipynb`** : notebook Jupyter regroupant l’ensemble du travail de préparation des données, d’analyse exploratoire, de visualisation et de tests statistiques

Les fichiers de données utilisés dans ce projet ne sont pas inclus dans le dépôt.

Ils correspondent à trois tables structurées comme suit :

- **Produits** : identifiant produit, catégorie, prix
- **Transactions** : identifiant de session, client, produit, date, montant
- **Clients** : identifiant client, sexe, année de naissance

---

## 📈 Objectifs de l’analyse

### 1. Analyse des ventes
- Chiffre d’affaires journalier, hebdomadaire et mensuel
- Évolution du chiffre d’affaires par catégorie de produit
- Identification des produits et clients les plus performants (**Top/Flop 20**)
- Analyse des inégalités dans le chiffre d’affaires (courbe de Lorenz, indice de Gini)

### 2. Analyse du comportement clients
- Nombre de clients uniques et fréquence d’achat
- Répartition du chiffre d’affaires et des achats selon le sexe et l’âge
- Taille moyenne du panier selon l’âge
- Associations entre âge, sexe et catégories de produits

### 3. Tests statistiques et hypothèses
- Test **Chi²** pour l’étude de la relation sexe / catégories de produits
- Corrélations (**Spearman / Pearson**) entre l’âge et le chiffre d’affaires ou la fréquence d’achat
- Régressions linéaires pour analyser l’effet de l’âge sur la taille du panier

---

## ⚙️ Méthodologie technique (Python)

- Nettoyage des données : gestion des valeurs manquantes, des doublons et des types
- Fusion des tables avec contrôle d’intégrité (`merge` avec validation)
- Détection et traitement des valeurs aberrantes (méthode de Tukey)
- Analyses exploratoires et statistiques
- Visualisations avec **Matplotlib** et **Seaborn**

---

## 🛠 Instructions pour lancer le projet

1. Installer **Python** (>= 3.10 recommandé)
2. Installer l’extension **Jupyter** pour VS Code
3. Installer les librairies nécessaires :

```bash
pip install numpy pandas matplotlib seaborn scipy statsmodels pingouin

