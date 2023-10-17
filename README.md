# Project Overview

The goal of this project was to organize a weekend food truck trip around Indianapolis. I utilized Google Maps API to fetch details about food trucks, ascertain their operating hours, plan the travel route, and visualize the journey.

## Folder Organization

### 1. List of Trucks:

This folder serves as a central repository for all the food trucks we've considered for the weekend trip. It houses the following files:

- **All Nearby Food Trucks 10km.xlsx**: Contains a list of all food trucks within a 10km radius of "Mile Square, Indianapolis, IN" with details like truck names, operational status, ratings, addresses, website links, and operating hours.

- **Breakfast Food Trucks.xlsx**: A curated list of food trucks ideal for breakfast.
  
- **Lunch Food Trucks.xlsx**: Features food trucks suitable for a midday meal.

- **Dinner Food Trucks.xlsx**: Lists food trucks perfect for an evening meal.

### 2. Saturday Plan:

Dedicated to the Saturday trip, this folder contains:

- **Saturday Food Truck List.xlsx**: Lists food trucks chosen for Saturday in sequence: breakfast, lunch, dinner.
  
- **Saturday Journey Preview.txt**: Detailed journey preview for each trip leg, including start/end points, distance, time, and transportation mode.
  
- **Saturday_Trip.html**: Interactive map visualizing the Saturday journey, showcasing the optimal route from Google Maps with a focus on user interactivity.

### 3. Sunday Plan:

Similar to "Saturday Plan", this directory is dedicated to Sunday's itinerary. It comprises:

- **Sunday Food Truck List.xlsx**
  
- **Sunday Journey Preview.txt**
  
- **Sunday_Trip.html**

---

## Methods and Approach:

- **Initialization**: The Google Maps API was initialized using a private API key (Stored in .gitignore file).
  
- **Finding Nearby Food Trucks**: Identified food trucks within a 10km radius of "Mile Square, Indianapolis, IN", filtering only operational ones.
  
- **Fetching Additional Information**: Gathered detailed information for each truck, like website and specific weekly operating hours.
  
- **Filtering by Operating Hours**: Ensured only trucks with available opening hours were considered.
  
- **Determining Transportation Mode**: Chose between driving, walking, and bicycling based on distances between food truck locations.
  
- **Visualizing the Trip**: Created an interactive map using the `folium` library, displaying the route with randomly selected dark colors and markers for each truck.
  
- **Dynamic Directions**: Displayed the most optimal route recommended by Google Maps, considering real-time factors like traffic.

---

## Results:

The program plots a weekend trip visiting various Indianapolis food trucks. The sequence of visits was proximity-based, and the transportation mode was selected dynamically. Each journey leg has been distinctly color-coded for differentiation.

Both Saturday and Sunday trips begin and end at "Mile Square, Indianapolis, IN". The day-wise food trucks are plotted in order, with annotations for the truck's name, distance, estimated time, and transportation mode. The routes for both days are saved as separate HTML files ("Saturday_Trip.html" and "Sunday_Trip.html") for an interactive browsing experience.
