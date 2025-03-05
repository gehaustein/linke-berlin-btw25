# Election Data Analysis and Visualization

This Jupyter Notebook is designed to analyze and visualize election data from the Berlin-Mitte district for the years 2021 and 2025. The analysis focuses on the percentage of votes received by the political party "Die Linke" and visualizes the changes over time using geographic data.

## Table of Contents

1. [Data Import](#data-import)
2. [Data Processing](#data-processing)
3. [Geospatial Analysis](#geospatial-analysis)
4. [Visualization](#visualization)
5. [Results](#results)
6. [Setup and Installation](#setup-and-installation)

## Data Import

The notebook begins by importing necessary libraries such as `pandas`, `geopandas`, `folium`, and `matplotlib`. It then loads election data from CSV and Excel files for the years 2021 and 2025. The data includes voting results and geographic information for the Berlin-Mitte district.

## Data Processing

- **Election Data**: The data is filtered to focus on the Berlin-Mitte district. The percentage of votes for "Die Linke" is calculated for both years.
- **Geographic Data**: Geospatial data is loaded using `geopandas` to represent the voting districts.

## Geospatial Analysis

The notebook performs a geospatial analysis to determine the overlap between voting districts in 2021 and 2025. It calculates the percentage of overlap for each district and creates a mapping between the districts of the two years.

## Visualization

- **Folium Map**: A layered map is created using `folium` to visualize the geographic boundaries of the voting districts for both years.
- **Matplotlib Plots**: Two plots are generated using `matplotlib`:
  - The first plot shows the percentage of votes for "Die Linke" in 2025.
  - The second plot visualizes the percentage gain in votes from 2021 to 2025.

## Results

The analysis results in a CSV file (`uwb_mapping.csv`) that maps the voting districts from 2025 to those in 2021 based on geographic overlap. The visualizations provide insights into the voting patterns and changes in support for "Die Linke" over time.

## Setup and Installation

To run this notebook, you will need to set up a local Python environment and install the required packages. Follow these steps:

1. **Create a Virtual Environment**:
   - Open a terminal or command prompt.
   - Navigate to the directory where your project is located.
   - Run the following command to create a virtual environment:
     ```bash
     python -m venv env
     ```
   - Activate the virtual environment:
     - On Windows:
       ```bash
       .\env\Scripts\activate
       ```
     - On macOS and Linux:
       ```bash
       source env/bin/activate
       ```

2. **Install Required Packages**:
   - Install the packages using pip:
     ```bash
     pip install -r requirements.txt
     ```
