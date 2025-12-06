# Analyse des Ventes et Comportement Clients - Librairie en Ligne

## 📌 Contexte

Notre librairie en ligne existe depuis deux ans.  
Sylvain, le nouveau responsable commercial, souhaite faire un point global sur les indicateurs et chiffres clés de l’entreprise afin de décider de la stratégie à suivre : offres à créer, adaptation des prix, ciblage de clients, etc.

Cette analyse est réalisée à partir des fichiers clients, produits et transactions fournis.

---

## 🗂 Contenu du projet

Le projet contient les fichiers suivants :  

- **`products.csv`** : informations sur les produits (ID, catégorie, prix, etc.)  
- **`transactions.csv`** : détails des transactions en ligne (session, client, produit, date, prix)  
- **`customers.csv`** : informations clients (ID, sexe, date de naissance, etc.)  
- **`analyse_ventes.ipynb`** : notebook Jupyter pour VS Code contenant toutes les analyses et visualisations  

---

## 📈 Objectifs de l’analyse

### 1. Analyse des ventes
- Chiffre d’affaires journalier, hebdomadaire et mensuel  
- Évolution du chiffre d’affaires par catégorie de produit  
- Identification des produits et clients les plus performants (**Top/Flop 20**)  
- Analyse des inégalités dans le CA (courbe de Lorenz, indice de Gini)  

### 2. Analyse du comportement clients
- Nombre de clients uniques et fréquence d’achat  
- Répartition du CA et des achats selon le sexe et l’âge  
- Taille moyenne du panier selon l’âge  
- Associations entre âge, sexe et catégories de produits  

### 3. Tests statistiques / Hypothèses
- Test **Chi²** pour la relation sexe/catégories  
- Corrélations (**Spearman / Pearson**) entre âge et CA ou fréquence  
- Régressions linéaires pour étudier l’effet de l’âge sur la taille du panier  

---

## 🛠 Instructions pour lancer le projet

1. Installer **Python** (>=3.10 recommandé) et **VS Code**  
2. Installer l’extension **Jupyter** pour VS Code  
3. Installer les librairies nécessaires :  
```bash
pip install numpy pandas matplotlib seaborn scipy statsmodels pingouin
