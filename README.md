# 🧠 Learning Word Vectors for Sentiment Analysis

Ce projet implémente en Python le modèle proposé dans le papier de recherche :
**"Learning Word Vectors for Sentiment Analysis"** par Maas et al. (Stanford University, 2011).

L'objectif est de générer des représentations vectorielles de mots (word embeddings) intégrant à la fois la **sémantique** et la **polarité sentimentale**, afin de les utiliser pour des tâches de classification d'opinions.

## 📚 Référence

> Maas, A. L., Daly, R. E., Pham, P. T., Huang, D., Ng, A. Y., & Potts, C. (2011).  
> Learning Word Vectors for Sentiment Analysis. *ACL 2011*.  
> [PDF original](https://aclanthology.org/P11-1015.pdf)

## 📦 Dataset utilisé

Nous utilisons le **Large Movie Review Dataset (IMDB)**, disponible publiquement ici :  
📎 https://ai.stanford.edu/~amaas/data/sentiment/

Le dataset contient :
- 25 000 critiques de films **annotées** (positives/négatives) pour l’entraînement
- 25 000 critiques pour le **test**
- + 50 000 critiques **non annotées** pour l’apprentissage semi-supervisé

## 🛠️ Technologies

- Python 3.10+
- NumPy, Pandas, Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

## 🚀 Objectifs du projet

- Implémenter le modèle proposé : combinaison d'un modèle probabiliste non supervisé (type LDA/log-bilinear) et d’un composant supervisé (régression logistique sur les vecteurs).
- Appliquer l’apprentissage supervisé et semi-supervisé sur les critiques IMDB.
- Comparer les performances du modèle avec d’autres approches classiques : tf-idf, LSA, LDA.
