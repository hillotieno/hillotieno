# Fieldnotes Studio

A small, static, browser-based data science workspace. Upload a CSV to get an automated exploratory analysis without sending your data to a server.

## Features

- CSV upload with drag-and-drop and a built-in retail sample dataset
- Automatic row/column and missing-value summaries
- Numeric-variable detection and target selection
- Descriptive statistics, histograms, strongest Pearson correlations, and scatter plots with a simple linear fit
- A one-feature correlation-squared score as an in-sample fit indicator
- Downloadable analysis report in CSV format
- Responsive layout; no build step or external dependencies

## Run locally

Open `index.html` in a modern browser, or serve this directory with any static web server. Select **Load sample data** to try the dashboard.

## Publish with GitHub Pages

In the repository's **Settings → Pages**, choose the `main` branch and `/ (root)` as the publishing source, then save. Once Pages finishes deploying, the website will be available at `https://hillotieno.github.io/hillotieno/`.

## Important notes

All dataset processing happens in the browser. The simple model score is the square of the Pearson correlation for the strongest single numeric feature, calculated on the same rows used to fit it. It is an exploratory in-sample indicator—not cross-validation, causal evidence, or a reliable measure of future predictive performance. Validate important findings with appropriate methods and domain expertise.
