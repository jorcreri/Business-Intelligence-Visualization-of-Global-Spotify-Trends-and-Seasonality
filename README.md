# Business-Intelligence-Visualization-of-Global-Spotify-Trends-and-Seasonality
This project focuses on analyzing Spotify music consumption data, exploring global trends and seasonal patterns, as well as investigating the acoustic "DNA" of different music genres. The project employs both Tableau and Power BI to create interactive dashboards showcasing geographic, temporal, and genre-based analyses.

**IMPORTANT:** Data files are **NOT** included in the `data/` folder. Instead, a `data/links.txt` file contains references to the external datasets used (links to Kaggle). See the "Data links" section below for details.

## Main Contents
- `notebooks/`  
  - `EDA_Estacionalidad_PowerBI.ipynb` — analysis of seasonal streaming patterns across years and months.  
  - `EDA_Atb_Tableau.ipynb` — technical feature analysis and popularity correlations.  
  - `EDA_Charts_Tableau.ipynb` — analysis of chart trends and groupings.

- `twb/`  
  - `Mapa_TopArtistas.twb` — Tableau workbook for visualizing the geographic distribution of top artists.  
  - `Análisis_Atributos.twb` — Tableau workbook analyzing technical attributes and their relationship with popularity.

- `pbix/`  
  - `Estacionalidad_Streams.pbix` — Power BI file for analyzing seasonal patterns in streams over the years.

- `reports/`  
  - `Reporte_Visualización.pdf` — final report detailing methodology and findings.

- `data/`  
  - `links.txt` — references to the external datasets used (the actual datasets are **not** included due to size / licensing). See "Data links" below for the contents of this file.

## Technologies
- **Python (Jupyter Notebooks)**: pandas, numpy, matplotlib, seaborn for data preprocessing and analysis.  
- **Tableau**: Interactive dashboards for global music consumption and acoustic analysis of genres.  
- **Power BI**: Seasonality analysis and artist popularity trends.  
- **CSV Datasets**: Preprocessed for Tableau and Power BI integration (download externally via links provided).

## Key Insights and Visualizations
- **Global Consumption Dashboard (Tableau)**: Interactive map highlighting top countries and regions by streaming volume, with dynamic artist rankings by month.
- **Genre Analysis Dashboard (Tableau)**: In-depth analysis of music genre characteristics (e.g., energy, tempo, positivity), and comparison of popular genres.
- **Seasonality Dashboard (Power BI)**: Time series analysis showing monthly trends and seasonal peaks in Spotify streams, broken down by genre and artist.
- **Artist Popularity (Power BI)**: Comparative analysis of artists’ streaming activity, helping to identify patterns of global consumption.

## Quick Start
1. Clone or download the repository.  
2. Open the notebooks in Jupyter Lab/Notebook.  
3. Install basic dependencies:  
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```  
4. Open Tableau workbooks with Tableau Desktop/Public and Power BI files with Power BI Desktop.  
5. Download the datasets listed in `data/links.txt` and place them in the `data/` folder (see below).  
6. Consult `reports/Reporte_Visualización.pdf` for methodology and detailed findings.

## Data links
The repository does **not** include the raw datasets. Please download the datasets from the following links and save them into the `data/` folder (filenames used in the project are indicated in the README `data/` section):

Links:

charts -> https://www.kaggle.com/datasets/dhruvildave/spotify-charts

dna -> https://www.kaggle.com/datasets/melissamonfared/spotify-tracks-attributes-and-popularity

seasonality -> https://www.kaggle.com/datasets/ivannatarov/spotify-daily-top-200-songs-with-genres-20172021

**Suggested local filenames (place inside `data/`):**
- `charts_grouped.csv` — processed grouped chart data (or the source CSV you generate after aggregation)  
- `spotify_mensual_limpio.csv` — cleaned monthly Spotify dataset (built from the seasonality dataset)  
- `atb_pop_limpio.csv` / `attributes_popularity.csv` — cleaned attributes & popularity datasets  

> Tip: keep original downloaded filenames and add a note in `data/links.txt` if you rename them.

## Repository Structure
```
Spotify_Analytics/
├─ data/
│  └─ links.txt
├─ notebooks/
│  ├─ EDA_Estacionalidad_PowerBI.ipynb
│  ├─ EDA_Atb_Tableau.ipynb
│  └─ EDA_Charts_Tableau.ipynb
├─ twb/
│  ├─ Mapa_TopArtistas.twb
│  └─ Análisis_Atributos.twb
├─ pbix/
│  └─ Estacionalidad_Streams.pbix
└─ reports/
   └─ Reporte_Visualización.pdf
```

## Impact / Use Cases
The project provides valuable insights for marketing, music analysts, and product teams to understand global music consumption patterns, artist popularity, and the impact of seasonal trends on Spotify’s audience. It helps in planning album releases, marketing strategies, and playlist curation.

## Authors
Developed by **Jorge Crespo Rivas**, **Clara Pérez Alonso** and **Lucía Hevia González**.  
Universidade da Coruña — Bachelor’s Degree in Data Science and Engineering (2025).
