# 2022 AI project
#### Predict whether a compound can be approved by FDA

## Datasets
#####[DrugBank](https://go.drugbank.com) 
The DrugBank database is a comprehensive, freely accessible, online database containing information on drugs and drug targets.
The database contains 9591 drug entries(11280 in the latest version) including 2037 FDA-approved small molecule drugs, 241 FDA-approved biotech (protein/peptide) drugs, 96 nutraceuticals and over 6000 experimental drugs.
>Ref: [Wikipedia](https://en.wikipedia.org/wiki/DrugBank)

## Features
We use molecular fingerprints to featurize compounds. Each compound might be constructed by several different substructures(we call it moiety), and we use one-hot representation to describe it. We also use several different systems of moieties to increase diversity. For instance Checkmol, Pubchem, Rings in drugs, MACCS etc. , and there are totally 1744 features.

## Models
Since it is a classification problem, we decide to use tree-based machine learning models to implement our classifier. 
We use Random Forest, SVM, XGBoost as our models.