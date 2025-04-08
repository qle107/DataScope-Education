
# DataScope-Education

**DataScope-Education** is a modular Python-based data analysis project built to explore, clean, and visualize education-related datasets from the World Bank’s EdStats program. Designed to be run in Google Colab with Drive integration, this project supports scalable CSV data ingestion, quality assessment, and insightful analytics.

---

## Features

- **Google Drive Integration** – Mount and retrieve datasets directly from Drive
- **Multi-file CSV Loader** – Automatically locates and loads datasets
- **Data Quality Analysis** – Identify missing values with `missingno`
- **Statistical Summaries** – Explore datasets with descriptive stats and metadata
- **Interactive Visualizations** – Dive into data using `plotly`, `seaborn`, and `matplotlib`

---

## Dataset Structure

All CSV files should be stored in a Google Drive folder and referenced through the `base_path`.

### Expected Files:

| Filename                  | Description                                      |
|---------------------------|--------------------------------------------------|
| `EdStatsData.csv`         | Core time-series data of education indicators    |
| `EdStatsCountry.csv`      | Country metadata                                 |
| `EdStatsCountry-Series.csv` | Mapping of countries to indicator series      |
| `EdStatsFootNote.csv`     | Notes and clarifications for data points         |
| `EdStatsSeries.csv`       | Indicator descriptions                           |

---

## Tech Stack

- Python 3 (Google Colab)
- pandas
- seaborn
- matplotlib
- plotly
- missingno
- os (for file management)

---

## How to Use

1. **Open the notebook in Google Colab**  
2. **Mount Google Drive**
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
3. **Set your `base_path`** to point to the folder containing your CSVs.
4. **Run all cells** to:
   - Load data
   - Analyze structure
   - Visualize missing data
   - Generate statistical summaries

---

## Sample Outputs

- Heatmaps of missing data
- Descriptive statistics for each dataset
- Interactive plots using Plotly
- Country and indicator breakdowns

---

## Future Work

- Correlation and trend analysis between education indicators
- Time series forecasting
- Integration with external socioeconomic datasets
- Deployment as a Streamlit or Dash app

---

## Some Words

Developed by me but since no one know who am i so you can copy pasta it.
