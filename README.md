# Real-world Graphs
## wiki-Talk Graph 

![edges GiB-hours vs Nodes](plots/wiki-Talk/gbhrs_nodes_wiki_talk.pdf)
* cost Graph
* GiB-hours = allocated memory in GiB * runtime (per executor)
* beschreibt die Fläche unter dem memory-runtime Graphen 


![Nodes vs minimal memory](plots/wiki-Talk/memory_vs_runtime_wiki_talk.pdf)
* zeigt memory allocted per executor vs runtime
* Kreuze sind runs mit out of memory Fehler
* Dreiecke sind runs mit timeout (30 Minuten)

  
![Nodes vs minimal memory](plots/wiki-Talk/accuracy_plots_wiki_talk.pdf)



# Synthetische Graphen: Erdős–Rényi
* Hier habe ich ER Graphen verschiedener Größen erstellt
* die Experimente laufen immer auf Graphen mit einer fixen Anzahl von ausgehenden Kanten pro Knoten und steigenden Knotenanzahlen

## ER Graph mit 2 out edges pro Knoten

Zu den folgenden Graphen hatte ich zwei Optionen:

Option 1:

![Runtime and Memory vs Nodes (MC)](plots/ER_2edg/combined_runtime_memory_vs_nodes_2edges_mc.pdf)
* Runtime mit dem allocated Minimal Memory für die Monte Carlo Methode
* Bei verschiedenen Graph Größen  

![Runtime and Memory vs Nodes (GX)](plots/ER_2edg/combined_runtime_memory_vs_nodes_2edges_gx.pdf)
* gleicher Graph nur für die GrapX Methode

Option 2:

Quasi die gleichen Metriken aber jeweils Runtime und Minimal Memory beider Methoden zusammen in einem Graph

![runtime vs nodes](plots/ER_2edg/runtime_vs_nodes_er_graph_2_edges.pdf)

![Minimal Memory vs Nodes](plots/ER_2edg/nodes_vs_mvm_2edges.pdf)


Es folgen die gleichen Experimente mit ausgehenden Kantenanzahlen 3,4,5

## ER Graph mit 3 out edges pro Knoten

Hier nur Option 1

![edges GiB-hours vs Nodes](plots/ER_3edg/combined_runtime_memory_vs_nodes_3edges_mc.pdf)


![Nodes vs minimal memory](plots/ER_3edg/combined_runtime_memory_vs_nodes_3edges_gx.pdf)


![runtime vs nodes](plots/ER_3edg/gbhrs_nodes_er_graph_3edges.pdf)



## ER Graph mit 4 out edges pro Knoten
Hier bisher nur Option 2

![edges GiB-hours vs Nodes](plots/ER_4edg/gbhrs_nodes_er_graph_4edges.pdf)


![Nodes vs minimal memory](plots/ER_4edg/nodes_vs_mvm_4edges.pdf)


![runtime vs nodes](plots/ER_4edg/runtime_vs_nodes_er_graph_4_edges.pdf)



## ER Graph mit 5 out edges pro Knoten
Hier bisher auch nur Option 2

![edges GiB-hours vs Nodes](plots/ER_5edg/gbhrs_nodes_er_graph_5edges.pdf)


![Nodes vs minimal memory](plots/ER_5edg/nodes_vs_mvm_5edges.pdf)


![runtime vs nodes](plots/ER_5edg/runtime_vs_nodes_er_graph_5_edges.pdf)
