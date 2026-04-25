D-SymBIA
Design Support System for Building-Integrated Agriculture
IAT 355 — Information Visualization · Spring 2026
Simon Fraser University · School of Interactive Arts and Technology
Computational Design Lab
 

About
D-SymBIA is an interactive scenario-based dashboard for exploring Building-Integrated Agriculture (BIA) opportunities in architectural design. It operationalizes the Computational Design Lab's BIA scenario framework — helping architects and urban designers compare multiple "what-if" pathways across location, crop type, BIA system, and waste circularity, rather than evaluating a single solution at a time.

Features
TabContent.  HomeBuilding illustration color-coded by DLI suitability · Surface selector · Seasonal DLI panel. Location (LS)Vega-Lite DLI heatmap · Seasonal boxplot · Area by direction · 49 real surfaces.Crop (CS)Radar chart · DLI supply vs. requirement · Crop parameter comparison BIA System (BS)Vega-Lite operational requirements · Compatibility heatmap. Waste (WS)Resource flow diagram · Greywater + HVAC heat recovery⊞ CompareAll four scenarios side by side

Dataset

Location_Database.csv — 49 building surfaces with seasonal DLI, radiation, temperature, humidity, orientation, area
Location_Scenarios.csv — 15 location scenario sets
Crop_Scenarios.csv — 15 crop scenario sets
Building geometry from Rhino model (Computational Design Lab case study)


Tech Stack

Design: Figma (wireframes, design system, color palette)
Frontend: HTML · CSS · JavaScript (single-page app)
Visualizations: Vega-Lite (heatmap, boxplot, bar charts, radar)
Development: AI-assisted translation from Figma to HTML/CSS
Deployment: GitHub Pages


Design System
TokenValuePrimary Green#1E8C5ABlue#3B82D4Amber#DBA830Terracotta#C8684ARed#B83020Peach#F2B89AFont (UI)UrbanistFont (Data)DM Mono
Color encoding is consistent across all visualizations — green = high DLI suitability, amber = medium, red = low.

Running Locally
bash# Clone the repo
git clone https://github.com/aysearyavilgenoglu/dsymbia.git
cd dsymbia

# Serve locally (required for CSV loading)
python3 -m http.server 8080

# Open in browser
open http://localhost:8080/index.html

Project Context
This dashboard is part of the Computational Design Lab's research on scenario-based BIA integration in architectural design, supported by the BC Centre for Agritech Innovation (BC CAI) and Perkins&Will Canada Architects.
