PMIST Waste Collection Optimization

This repository contains the Python implementation of a Hybrid Optimization Algorithm (Sweep Clustering + 2-Opt Heuristic) designed to solve the Capacitated Vehicle Routing Problem (CVRP).

The project focuses on optimizing waste collection routes within the Periyar Maniammai Institute of Science & Technology (PMIST) campus road network, aiming to reduce total travel distance and improve operational efficiency.
Project Structure

    Waste_Collection_Optimization.ipynb: The main Jupyter Notebook containing the full implementation of the Greedy, 2-Opt, and Hybrid algorithms, along with performance comparisons.

    data/: Directory containing the VRP benchmark datasets (A-n32-k5, B-n31-k5, E-n22-k4, and E-n51-k5) used for validation.

    pmist_map.pdf: A visualization of the optimized waste collection routes generated using real-world road network data from OpenStreetMap.

Methodology

    Sweep Clustering: Organizes waste bins into manageable zones based on angular coordinates relative to the depot.

    2-Opt Optimization: Refines the routing sequence within each zone to eliminate path crossings and minimize total distance.

    Road Network Integration: Utilizes the OSMnx and NetworkX libraries to calculate actual road distances rather than simple Euclidean paths for real-world campus scenarios.

Prerequisites

To run the code, you will need the following Python libraries:
Bash

pip install osmnx networkx matplotlib

Guide to Reproduce Results

    Ensure all dataset files (A-n32-k5.vrp, etc.) are in the data/ folder.

    Open Waste_Collection_Optimization.ipynb in Google Colab.

    Go to 'Runtime' -> 'Run all' to execute all algorithms and generate the performance table.

    The final visualization map will be saved as pmist_map.pdf.

Data and Code Availability

The datasets and source code provided in this repository are intended for academic research purposes. If you use this implementation in your own work, please cite this repository.

Developed for research on waste management optimization at PMIST.
