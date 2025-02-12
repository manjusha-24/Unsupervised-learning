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

1.Import Libraries

2.Read Data

3.Exploratory Data Analysis

3.1 - Understand the Dataset

3.2 - Data Type

3.3 - Distribution of Variables

3.4 - Analysis of Outliers

3.5 - Summary Statistics

3.6 - Missing Values

3.7 - Prepare the Data

4.K-means Clustering

4.1 - Identify the Optimal Number of Clusters

4.2 - Build the Model

4.3 - Analyze the Clusters

5.Hierarchical Clustering

5.1 - Identify the Optimal Number of Clusters

5.2 - Build the Model

5.3 - Analyze the Clusters

6.DBSCAN

6.1 - Build the Model

6.2 - Analyze the Clusters

7.Visualize the Clusters

The subplots above represent clusters formed by different algorithms. We can see that the K-means and hierarchical clustering have created 3 clusters, while the DBSCAN algorithm has grouped the data into 4 clusters.

The plots for K-means and hierarchical clustering show similarity in cluster formation. The DBSCAN algorithm has clustered houses based on the power consumption of the other appliances in the house. Also, the blue points in the DBSCAN plot represent the outliers identified by the algorithm.

We can see that some points overlap in the subplots, this is because we have projected a 7-D dataset to 2-D which is explaining only 65 percent of total variance in the original data.
