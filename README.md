# Belly Button Biodiversity Dashboard

## Project Overview

This interactive dashboard explores the Belly Button Biodiversity dataset, which catalogs the microbes colonizing human navels. The project visualizes the microbial species (operational taxonomic units, or OTUs) present in more than 70% of individuals and investigates the diversity of rarer microbes. The aim is to offer insights into the microbial ecosystem of the human navel and its potential implications for human health and science.

## Purpose

The purpose of this dashboard is to make the data from the Belly Button Biodiversity study accessible and understandable through interactive visualizations. By examining the presence and frequency of OTUs in individuals, this project contributes to the broader understanding of human microbiomes.

## Technologies and Tools Used

- **D3.js:** For reading the `samples.json` dataset and manipulating the DOM.
- **Plotly.js:** To create interactive visualizations, including a bar chart, bubble chart, and an optional gauge chart.
- **HTML/CSS:** For structuring and styling the dashboard's webpage.
- **JavaScript:** The primary programming language used for the web application's functionality.

## Repository Navigation

- `index.html`: The main HTML document for the dashboard.
- `samples.json`: The dataset containing microbial species (OTUs) data.
- `static/js/app.js`: Contains the JavaScript code for fetching the data, and generating and updating the visualizations.
- `static/css/style.css`: Custom CSS styles for the dashboard.

## Key Features and Findings

- **Horizontal Bar Chart:** Displays the top 10 OTUs found in a selected individual. It uses `sample_values` as the values, `otu_ids` as the labels, and `otu_labels` as the hovertext.
- **Bubble Chart:** Represents each sample, with `otu_ids` for the x values, `sample_values` for the y values and marker size, and `otu_labels` for the text values. The colors of the markers are also determined by `otu_ids`.
- **Sample Metadata Display:** Shows demographic information and other relevant metadata for the selected individual.
- **Dynamic Updates:** All visualizations and metadata information update automatically when a new sample is selected, providing a seamless user experience.

## Conclusions

- A significant portion of the microbial species found in human navels are common across a majority of the population.
- The diversity of rare microbes varies significantly between individuals, suggesting personalized microbial ecosystems.
- The dashboard effectively demonstrates the potential of interactive web visualizations in engaging users with complex datasets.
