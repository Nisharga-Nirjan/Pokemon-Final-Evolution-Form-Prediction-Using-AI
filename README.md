# Pokémon Final Evolution Form Prediction

Pokémon games are regarded as one of the most successful video game adaptations of all time and go way back to when the idea of video games were still afresh. Nintendo, on the other hand, is a major player in the video game industry and has a large team of developers working on creating new games for their consoles for decades. Therefore, working with this dataset can provide insights and opportunities for research, game development, and other renown fields. The core objective of our project is to carefully observe specific input features namely `Base hit points stats`, `Base attack stats`, `Base defense stats` etc. of each pokémon and predict their `final evolution`. In this case, the final evolution would work as our output label which holds binary values referring to `yes` or `no`. Since the output label contains categorical variables, this would stand as a `classification problem`. By using classification models such as `K-Nearest Neighbor (KNN)`, `Decision Tree` and `Support Vector Machine (SVM)`, we plan on recovering the best model and drawing a brief analysis on the rest of the models. For the ease of understanding, we would also demonstrate our findings through `heatmaps`, `bar charts` and other visual stances.

# Dataset Description

Our project uses the “All Pokemon Dataset” that contains all the information for 1032 instances of different pokemons, with a total of 44 features in the dataset such as: Name, HP, Mean, Generation, etc. Out of the 44 features, 5 of them are categorical features, namely: Name, Type 1, Type 2, Abilities, Experience type and the rest 39 features are quantitative. So we have a total of 1032x44 data points. Our Project is a classification problem since the solution we’re trying to predict is whether a pokémon is in its final evolution form or not. As our output feature ‘Final Evolution’ has two unique classes, 1 and 0, this means that our project is trying to predict whether a pokémon is a legendary pokémon, so 1, or not, so 0. So, this indicates that our proposed model is attempting to classify the problem. For our particular problem we only need to select a few features which are:

+ Input Features: `HP (Base HitPoints)`, `Att (Base Attack)`, `Def (Base Defense)`, `Spa (Base Special Attack)`,
  `Spd (Base Special Defense)`, `Spe (Base Speed)`, `BST (Sum of all base stats)` and `Standard Deviation (Standard Deviation of all Base Stats)`

+ Output Feature: `Final Evolution`

-[Dataset](https://www.kaggle.com/datasets/maca11/all-pokemon-dataset)

# Base Models

+ KNN (K-Nearest Neighbours)
+ Decision Tree
+ SVM (Support Vector Machine)

# Dataset Splitting and Feature Scaling Methods

+ Splitting Methods: `Random` and `Stratified`
+ Scaling Methods: `MinMax` and `Standard`

# Model Variants

12 variants have been utilized which are:

+ KNN-MinMax-Random
+ KNN-Standard_Random
+ KNN-MinMax-Stratified
+ KNN-Standard-Stratified
+ DecisionTree-MinMax-Random
+ DecisionTree-Standard_Random
+ DecisionTree-MinMax-Stratified
+ DecisionTree-Standard-Stratified
+ SVM-MinMax-Random
+ SVM-Standard_Random
+ SVM-MinMax-Stratified
+ SVM-Standard-Stratified
