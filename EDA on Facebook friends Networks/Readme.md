

# Facebook Network Analysis

This Python script analyzes a social network using the NetworkX library. The network is represented as an edgelist in the 'facebook_combined.txt' file, which contains information about connections between users on a social platform like Facebook.

## Network Visualization

The script starts by loading the network from the edgelist and visualizing it using the Spring Layout algorithm. It creates a network graph and uses the spring layout to position the nodes. The resulting visualization shows the network's structure, with nodes representing users and edges representing connections.

## Basic Network Statistics

The script calculates and prints basic network statistics, including:
- The number of nodes (users) in the network.
- The number of edges (connections) in the network.

## Node Degree Analysis

The script performs node degree analysis, which includes:
- Calculating the degree (number of connections) of each node and storing it in a dictionary.
- Finding the node with the highest degree and printing its degree.
- Finding the node with the lowest degree and printing its degree.
- Creating a subgraph containing the neighbors of a specific node ('11') and visualizing it.
- Creating a subgraph containing the neighbors of another node ('0') and printing the total number of friends for that node.

## Node Centrality Analysis

The script analyzes node centrality using three centrality measures:
- Degree Centrality: Finding the most influential nodes based on degree centrality and printing the top 10.
- Eigenvector Centrality: Finding the most important nodes based on eigenvector centrality and printing the top 10.
- Betweenness Centrality: Finding connector links based on betweenness centrality and printing the top 10.

## Network Metrics

The script calculates and prints various network metrics, including:
- Average Clustering Coefficient: Measures the degree to which nodes tend to cluster together.
- Network Density: Measures the ratio of actual edges to possible edges in the network.
- Network Diameter: Measures the longest shortest path between any two nodes in the network.

## Bridge Detection

The script identifies bridge edges (edges that, when removed, increase network fragmentation) and prints the nodes involved in those bridges.

This script provides an overview of social network analysis using NetworkX and can be customized and expanded for more in-depth analysis of social networks.

