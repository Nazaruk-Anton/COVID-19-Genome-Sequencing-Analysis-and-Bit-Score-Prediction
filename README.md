# COVID-19-Genome-Sequencing-Analysis-and-Bit-Score-Prediction
This repository contains a Jupyter Notebook that demonstrates an analysis of COVID-19 genome sequences. The goal of this project is to identify mutations and potential targets for drugs based on the given dataset.

# Introduction
The dataset consists of 428 mutated versions of the COVID-19 virus genome sequences. The analysis aims to predict bit scores and relationships between these sequences by analyzing the mutations and their development.

# Dataset
The dataset used in this project includes COVID-19 genome sequences and associated features. Each sequence is composed of four nucleotide bases: Adenine (A), Guanine (G), Thymine (T), and Cytosine (C). The sequences follow patterns using these bases, represented as letters A, T, C, and G. Genome sequencing is the process of analyzing an individual's DNA to gain insights into its properties.
The dataset files 'SARS_CORONAVIRUS_NC_045512_sequence.fasta' and 'Alignment-HitTable.csv' are required to run the code. Please download the dataset files and place them in the same directory as the corresponding notebooks.

# Part 1: COVID-19 Genome Sequencing Analysis
The first part of the project focuses on analyzing the COVID-19 genome sequences dataset. The following tasks are performed:

Sequence Length: Calculate the length of each genome sequence and find the median length.
Substring Matching: Identify whether each sequence contains a specific sub genome sequence.
Differences Matrix: Calculate the number of differences between sequences and create a differences matrix.
Finding Similar Sequences: Identify the two most similar genome sequences.
To run the notebook successfully, ensure you have the required packages installed (pandas, numpy). Download the dataset file 'SARS_CORONAVIRUS_NC_045512_sequence.fasta' and place it in the same directory as the notebook.

# Part 2: Feature Analysis using K-Means Clustering
The second part of the project focuses on feature analysis using K-Means clustering. The following tasks are performed:

K-Means Clustering: Apply K-Means clustering to the numeric columns of the dataset.
Silhouette Scores: Calculate silhouette scores for different numbers of clusters.
K-Means Clustering on Normalized Data: Normalize the numeric data and apply K-Means clustering.
The analysis helps identify patterns and similarities among genome sequences. The notebook requires pandas, numpy, scikit-learn, and seaborn packages.

# Part 3: PCA Analysis of Genome Sequences
The third part of the project focuses on performing Principal Component Analysis (PCA) on genome sequence data. The notebook showcases the following steps:

Data Description: Analyze the dataset using the .describe() method.
Correlation Analysis: Calculate the correlation matrix and visualize it as a heatmap.
PCA Transformation: Perform PCA on the numeric columns of the dataset.
PCA Components: Analyze and visualize the components of the PCA transformation.
K-Means Clustering: Apply K-Means clustering to the transformed data and visualize the clusters.
The notebook uses the 'Alignment-HitTable.csv' dataset and requires the installation of pandas, numpy, scikit-learn, matplotlib, and seaborn packages.

 
# Part 4: Predicting Bit Scores of Sequences
In the final part of the project, different models are used to predict the bit scores of sequences. The following steps are performed:

Feature Preparation: Create a feature dataframe and define the target variable.
Data Normalization: Normalize the feature data using StandardScaler.
Linear Regression: Fit a linear regression model to predict bit scores.
Neural Network Regression: Train a multi-layer perceptron regression model to predict bit scores.
Both linear regression and neural network models are used for feature prediction. The notebook requires pandas, numpy, scikit-learn, and tensorflow packages.

# Conclusion 
In conclusion, the analysis of the provided bit scores allowed us to determine the similarity between various sequences and the reference genome (NC_045512.2 Wuhan seafood market pneumonia virus isolate Wuhan-Hu-1). Higher bit scores indicated a stronger similarity, while negative scores suggested low alignment or similarity. By focusing on sequences with high bit scores, we can identify genome sequences closely related to the reference genome, which could be potential targets for further analysis and drug targeting.

The K-means algorithm was chosen for this project as it is a simple and effective clustering algorithm that can partition gene expression data into groups with similar expression profiles. This information can provide insights into gene regulatory mechanisms, biomarker identification, and disease mechanisms. However, the selection of the K-means algorithm depends on various factors, such as the data characteristics, desired number of clusters, and project objectives. Other clustering algorithms or dimensionality reduction techniques could also be considered based on specific requirements as was demonstratred in the Part 3 of the project.

It's important to note that while the bit scores and K-means analysis provide valuable insights, further analysis, such as phylogenetic studies and experimental validation, would be necessary to confirm the findings and assess the suitability of specific sequences as drug targets.
