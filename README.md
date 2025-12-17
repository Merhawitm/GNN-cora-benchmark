# GNN-cora-benchmark
Benchmarking GCN, GraphSAGE, and GATv2 on the Cora dataset

What this project is

In this task, I trained and compared 4 models on the Cora citation dataset using the Spektral library.

Goal: predict the class (topic) of each paper (node).

     Dataset (Cora)

Nodes: papers

Edges: citations between papers

Features: words in each paper

Labels: paper category (class)

Task type: Node classification


             Models I implemented

MLP (baseline)

Uses only node features

Ignores the graph (edges)

GCN

Uses neighbors to update each node’s features

GraphSAGE

Samples and combines neighbor information (works well for bigger graphs)

GATv2

Uses attention to give more weight to important neighbors

What I did (steps)

Loaded Cora from Spektral

Built each model (MLP, GCN, GraphSAGE, GATv2)

Trained each model

Evaluated test accuracy

Plotted training/validation accuracy and loss (optional)

Expected outcome

MLP usually performs worst because it ignores edges

GNN models perform better because they use graph connections

GATv2 can perform best because it learns which neighbors matter most

Author

Merhawit Tesfay Kassa
