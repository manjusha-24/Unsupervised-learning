# Unsupervised-learning
Unsupervised learning is a type of machine learning where the model learns patterns and relationships in the data without labeled outputs. Unlike supervised learning, where the model is trained on labeled data, unsupervised learning identifies hidden structures, clusters, or associations within the dataset. Common techniques in unsupervised learning include:

Clustering: Grouping similar data points together (e.g., K-means, DBSCAN, Hierarchical Clustering).

Dimensionality Reduction: Reducing the number of variables in the dataset (e.g., PCA, t-SNE).

Anomaly Detection: Identifying unusual data points (e.g., Isolation Forest, One-Class SVM).

In this project, clustering algorithms are used to classify houses based on their energy consumption patterns, helping to derive meaningful insights for energy management and optimization.

Energy Consumption Clustering

Problem Statement

Typically, a house in Manhattan comprises various electrical appliances. Each of these appliances partly contributes to the total energy consumption of the house. Grouping these houses based on their power usage helps analyze electricity demand in different parts of the city. These insights can also be useful in identifying appliances with high and low electricity consumption.

In this case study, we consider the power consumption due to various appliances in the house and try to group the houses based on their power consumption.

Data Definition

The dataset represents the electric power consumption in the house. The data attributes are defined as follows:

Global_active_power: The global minute-averaged active power of the house (in KW).

Global_reactive_power: The global minute-averaged reactive power of the house (in KW).

Voltage: The minute-averaged voltage of the house (in volt).

Global_intensity: The global minute-averaged current intensity of the house (in ampere).

Kitchen_consumption: The power consumption of the appliances in the kitchen (in watt-hour).

Laundry_consumption: The power consumption of the appliances in the laundry room (in watt-hour).

Other_appliances_consumption: The power consumption of the appliances other than in the kitchen and laundry room (in watt-hour).

Table of Content

Import Libraries

Read Data

Exploratory Data Analysis

3.1 - Understand the Dataset

3.2 - Data Type

3.3 - Distribution of Variables

3.4 - Analysis of Outliers

3.5 - Summary Statistics

3.6 - Missing Values

3.7 - Prepare the Data

K-means Clustering

4.1 - Identify the Optimal Number of Clusters

4.2 - Build the Model

4.3 - Analyze the Clusters

Hierarchical Clustering

5.1 - Identify the Optimal Number of Clusters

5.2 - Build the Model

5.3 - Analyze the Clusters

DBSCAN

6.1 - Build the Model

6.2 - Analyze the Clusters

Visualize the Clusters

Cluster Analysis

The subplots represent clusters formed by different algorithms:

K-means and hierarchical clustering created 3 clusters.

The DBSCAN algorithm grouped the data into 4 clusters.

The cluster formations of K-means and hierarchical clustering are quite similar.

The DBSCAN algorithm categorized houses based on the power consumption of appliances other than the kitchen and laundry.

The blue points in the DBSCAN plot represent outliers detected by the algorithm.

Some points overlap due to the projection of a 7-D dataset into 2-D, which explains only 65% of the total variance in the original data.
