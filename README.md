# 🗺️ Selecting Ideal Hotels in the DC Area

A geospatial application that helps travelers find the **top 5 hotels in Washington, D.C.** based on personalized preferences like **price**, **rating**, and **distance to metro stations**. This project uses **raster and vector-based spatial analysis** to recommend optimal hotels and identify nearby landmarks.

## Problem Statement

Washington, D.C. has a large number of hotels, and selecting one can be overwhelming—especially for visitors with varying preferences for:

- Proximity to metro stations
- Price range
- Traveler ratings
- Landmarks nearby

## Goals

- Identify **top 5 hotel options** based on user input.
- Evaluate hotels using **multi-criteria evaluation (MCE)**.
- Provide nearby **landmarks** for each recommended hotel.
- Focus on accessibility from **selected metro stations**.

## Technologies & Geospatial Techniques Used

- **Python + ArcPy**
- **Raster Analysis**
- **Euclidean & Manhattan Distance**
- **Multi-Criteria Evaluation (MCE)**
- **Landmark Proximity with Scaled Distance**
- **Interactive user inputs**

## Core Logic

### Step-by-step Workflow:

1. **Load and clean datasets** (hotels, metro, landmarks).
2. **User inputs**: price, rating range, metro station, max distance.
3. Filter hotels using a **raster-based metro distance layer** (`select_hotels_raster_method`).
4. Compute **exact Manhattan distance** and apply **MCE scoring**.
5. Use scaled **Euclidean distance** to find landmarks near selected hotels.
6. Display the **top 5 hotels** with the highest MCE scores along with nearby points of interest.

## Sample Functions

- `select_hotels_raster_method()`: Filters hotels within user-defined distance to a metro station.
- `find_nearby_landmarks()`: Computes scaled distance to nearby landmarks.
- `display_results()`: Shows final ranked hotel list and associated nearby landmarks.

## Applications

- 🧳 Tourists exploring D.C.
- 💼 Business travelers needing convenience
- 🗺️ Visitors planning around metro proximity and landmark access

## Future Improvements

- Add **neighborhood-level selection** (not just metro station)
- Factor **landmarks into MCE score**
- Include **traffic/travel time** in distance calculations
- Balance price with rating more intelligently

## Conclusion

This tool helps visitors:

- Quickly narrow down ideal hotel options
- Visualize how hotels compare by location and access
- Get contextual information via nearby landmarks

It combines core **geospatial techniques** with **practical use cases**, and can be adapted for other cities or types of lodging.
