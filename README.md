# Data Visualization

A comprehensive, interactive data visualization dashboard built with **Dash** and **Plotly**, analyzing Hollywood and Indian movies datasets.

## Overview

This project provides an interactive dashboard for exploring movie data across industries, decades, and genres. It combines data from Hollywood and Indian film industries into a unified, filterable visualization interface.

## Features

- **Interactive Dashboards** powered by Plotly and Dash
- **Multiple Visualization Types**: Trend charts, scatter plots, box plots, genre explorers, and histograms
- **Dynamic Filtering**: Filter by industry and year range
- **Key Performance Indicators (KPIs)**: Real-time statistics based on filtered data
- **Responsive Web Interface** with Bootstrap components
- **Efficient Data Processing** with Pandas and NumPy

## Requirements

- dash
- dash-bootstrap-components
- pandas
- numpy
- plotly

## Installation

```bash
pip install -r requirements.txt
```

## Running the Application

```bash
python data_visuvalizaion.py
```

The dashboard will be accessible at `http://0.0.0.0:8050` (or `http://localhost:8050`)

## Project Structure

### Source Files
- `data_visuvalizaion.py` - Main Dash application with all interactive components and callbacks
- `requirements.txt` - Python dependencies

### Data Files
- `final_movies_dataset.csv` - Merged dataset combining Hollywood and Indian movies
- `hollywood_movies.csv` - Raw Hollywood movies dataset
- `indian_movies.csv` - Raw Indian movies dataset
- `modified_hollywood_movies.csv` - Processed Hollywood movies data
- `modified_indian_movies.csv` - Processed Indian movies data

### Jupyter Notebooks
- `hollywood_movies.ipynb` - Exploratory data analysis and preprocessing for Hollywood movies
- `indian_movies.ipynb` - Exploratory data analysis and preprocessing for Indian movies
- `movies_merging.ipynb` - Data merging and integration workflow

## Dashboard Components

### Filters
- **Industry Selection**: Choose one or multiple film industries (Hollywood, Indian, etc.)
- **Year Range Slider**: Select movies from specific decades

### Key Metrics
- Number of movies in current selection
- Median rating
- Median budget
- Top genre

### Visualization Tabs

1. **Budget vs Year** - Trend analysis showing average or total budget over years by industry
2. **Budget vs Runtime** - Scatter plot with bubble sizing based on ratings, log scale options available
3. **Rating Distributions** - Box plots showing rating distributions by industry or genre
4. **Genre Explorer** - Top genres visualization with bar chart or treemap options
5. **Histograms** - Genre and year-wise distribution patterns

## Data Processing Workflow

1. Raw data from `hollywood_movies.csv` and `indian_movies.csv`
2. Processing via `hollywood_movies.ipynb` and `indian_movies.ipynb`
3. Modified datasets: `modified_hollywood_movies.csv` and `modified_indian_movies.csv`
4. Integration via `movies_merging.ipynb`
5. Final merged dataset: `final_movies_dataset.csv`
6. Visualization through interactive Dash dashboard

## Features Highlights

- **Genre Handling**: Automatically processes movies with multiple genres
- **Multi-language Support**: Visualizations account for different movie languages
- **Smart Currency Formatting**: Budget displays with appropriate units (B, M, K)
- **Interactive Tooltips**: Hover information shows movie details
- **Responsive Design**: Adapts to different screen sizes using Bootstrap grid system
