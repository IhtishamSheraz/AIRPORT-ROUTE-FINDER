Overview

The Airport Route Finder is a C++ graphical application that helps users find the shortest flight path between two cities.
The program uses Dijkstra’s Algorithm to calculate the minimum distance between airports and displays the route on a world map using a graphical interface.

This project demonstrates the practical application of Data Structures and Algorithms (DSA) concepts such as graphs and shortest path algorithms in a real-world scenario.

Features

Find the shortest flight route between two airports.

Interactive graphical interface using SFML.

Visual display of routes on a world map.

Graph-based airport network representation.

Uses Dijkstra’s Algorithm for shortest path calculation.

Displays route distance between selected airports

Technologies Used

C++

SFML (Simple and Fast Multimedia Library)

Graph Data Structure

Dijkstra’s Shortest Path Algorithm

Visual Studio 2022

Project Structure
Airport Route Finder
│
├── main.cpp        # Program entry point
├── graph.cpp       # Graph implementation and Dijkstra algorithm
├── graph.h         # Graph class definition
├── gui.cpp         # GUI implementation
├── gui.h           # GUI class definition
│
├── world_map.png   # Map used for visualization
├── ARIAL.TTF       # Font used in GUI
│
└── ROUTE.vcxproj   # Visual Studio project file
How the System Works

The airport network is represented as a graph.

Airports are treated as nodes (vertices).

Flight connections between airports are edges with distances.

When a user selects a source and destination, the program:

Runs Dijkstra’s Algorithm

Finds the minimum distance path

Displays the route on the GUI.

Installation and Setup
1. Install Requirements

Make sure the following are installed:

Visual Studio 2022

SFML Library

Download SFML:
https://www.sfml-dev.org/download.php

2. Configure SFML in Visual Studio

Open the project in Visual Studio.

Add SFML include directories.

Link the required SFML libraries:

sfml-graphics

sfml-window

sfml-system

3. Run the Project

Open ROUTE.vcxproj in Visual Studio.

Build the project.

Run the application.

The GUI window will open and display the map with available airport routes.

Example Use Case

User Input:

Source Airport: Islamabad
Destination Airport: Dubai

Program Output:

Shortest Route:
Islamabad → Karachi → Dubai
Total Distance: 2340 km

The route will also be visualized on the map.

Algorithm Used
Dijkstra’s Algorithm

Dijkstra’s algorithm is used to compute the shortest path between nodes in a graph.
It works by repeatedly selecting the node with the minimum distance and updating distances to its neighbors.

Time Complexity:

O((V + E) log V)

Where:

V = number of vertices (airports)

E = number of edges (routes)

Educational Purpose

This project was developed as part of a Data Structures and Algorithms course to demonstrate how theoretical algorithms can be implemented in practical applications such as route optimization systems.

Author

Ihtisham Sheraz
BS Computer Science
Bahria University, Islamabad
