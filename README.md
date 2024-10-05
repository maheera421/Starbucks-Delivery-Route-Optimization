# ☕ Starbucks Delivery Route Optimization

This project focuses on optimizing delivery routes for Starbucks stores within a city. Using advanced data filtering, graph theory, and machine learning techniques, it aims to minimize the travel time and distance for deliveries between stores, enhancing efficiency and reducing operational costs.

## 📊 Project Overview
The goal of this project is to create an optimized delivery route within a city by leveraging data related to store locations, travel times, and road networks. This solution is designed to help delivery drivers follow the most efficient route, minimizing fuel consumption and travel distance.

## 🧠 Machine Learning & Graph Theory Workflow
The workflow in this project includes the following steps:

- **Data Preprocessing:** Filtering store location data based on the selected city.
- **Map Visualization:** Using geospatial tools to plot store locations on a city map.
- **Graph Creation:** Generating a road network graph from the selected city and calculating travel times between nodes.
- **Route Optimization:** Applying the OR-Tools library to calculate the shortest and most efficient route for the delivery driver.
- **Evaluation:** Visualizing the optimized route and calculating the total travel distance.

## 📂 Dataset
The dataset consists of Starbucks store locations in London, including features such as the city, street address, latitude, and longitude. The filtered dataset is used to create a distance matrix that feeds into the route optimization algorithm.

## 🚀 Getting Started
To run this project on your local machine:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/maheera421/starbucks-delivery-optimization.git
   ```

2. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## ⚙️ Requirements
The main libraries used in this project are:

- **pandas:** For data manipulation.
- **numpy:** For numerical computations.
- **matplotlib & seaborn:** For data visualization.
- **folium & plotly:** For map visualization.
- **osmnx & networkx:** For road network and graph analysis.
- **OR-Tools:** For route optimization.

For a complete list of dependencies, refer to the `requirements.txt` file.

## 📈 Optimization Process

The project uses the following steps to optimize the delivery routes:

1. **Data Filtering:** Filter store data by city (e.g., London).
2. **Graph Creation:** Generate a road network graph and calculate travel times using OSMnx.
3. **Shortest Path Calculation:** Use Dijkstra’s algorithm to find the shortest path between store locations.
4. **Route Optimization:** Apply Google OR-Tools to generate an optimal route based on the calculated distance matrix.
5. **Visualization:** Visualize the optimized route on a map using Folium and Plotly.

## ✨ Features

- **City-based Filtering:** Allows selecting a specific city and generating a route within it.
- **Graph Theory Implementation:** Uses road networks to calculate real-world travel times and distances.
- **Optimal Route Calculation:** Generates the shortest possible delivery route using state-of-the-art algorithms.
- **Map Visualizations:** Displays the route dynamically using interactive maps.

## 📊 Performance Metrics

- **Total Distance:** The total distance covered by the delivery driver is displayed after route optimization.
- **Nodes Visited:** The number of nodes (locations) visited during the route.

## 🗺️ Visualizations

The project includes interactive map visualizations that display the starting point (in red), the stores to visit (in black), and the optimized path (in blue). You can view the optimized route and its animation on the map.
