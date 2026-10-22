# CS-340 Project Two – Grazioso Salvare Dashboard  
**Student:** Trista Jacobs

## Overview
This dashboard was created to support Grazioso Salvare in identifying dogs suitable for specialized rescue training. It connects to a MongoDB database through a custom CRUD module and displays animal data in an interactive dashboard. The table, chart, and map all update automatically based on the selected rescue filter.

## Features
- **Interactive Filters**
  - Water Rescue
  - Mountain or Wilderness Rescue
  - Disaster or Individual Tracking
  - Reset (full dataset)
- **Dynamic Components**
  - Data table with full animal details
  - Pie chart showing breed distribution
  - Map showing the selected animal’s location
- **Branding**
  - Grazioso Salvare logo
  - “Dashboard by Trista Jacobs” header

## Screenshot Summary
Screenshots demonstrate dashboard functionality and rubric alignment. Each screenshot shows a different filter state and confirms that the dashboard updates correctly.

1. **Reset Filter**  
   - Full dataset displayed  
   - Breed distribution chart shows all breeds  
   - Map centered  
   - Filename: `Reset.png`

2. **Water Rescue Filter**  
   - Displays water‑rescue‑qualified breeds  
   - Chart shows 100% Labrador Retriever Mix  
   - Filename: `Water Rescue.png`

3. **Mountain Rescue Filter**  
   - Displays Husky, Rottweiler, Malamute, etc.  
   - Chart and map update accordingly  
   - Filename: `Mountain or Wilderness Rescue.png`

4. **Disaster Tracking Filter**  
   - Displays Bloodhound, German Shepherd, Golden Retriever, etc.  
   - Chart and map reflect filtered results  
   - Filename: `Disaster or Individual Tracking.png`

5. **Branding Screenshot**  
   - Logo and student name visible  
   - Included in one or more screenshots

## How to Run
1. Open `ProjectTwoDashboard.ipynb` in JupyterLab.
2. Ensure MongoDB is running (no authentication required).
3. Run all cells from top to bottom.
4. The dashboard will launch in a new tab with full interactivity.

## Challenges
A key challenge was ensuring that all dashboard components updated together when filters were applied. Initially, the table, chart, and map did not stay synchronized. This was resolved by linking the radio input to each callback function so all components shared the same filtered dataset.

## Notes
- The CRUD module (`CRUD_Python_Module.py`) handles all database operations.
- MongoDB access is open in this environment; no login is required.
- All filters and visuals were validated using the screenshots listed above.
