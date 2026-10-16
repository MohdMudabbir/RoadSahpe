# 🛣️ RoadShape

**Advanced Mapping, Skewness & Chi-Square Statistical Analytics for Road Accident Data**

RoadShape is a single-file, browser-based analytics dashboard. Load a road-accident CSV (or use the built-in 800-record demo dataset) and explore it through interactive charts, a map workspace, and statistical labs, with no backend or installation needed.

## ✨ Features

- 📊 **Interactive dashboards**: overview, temporal, spatial, road/junction, environment and severity views
- 🗺️ **Map workspace** (Leaflet) with filters for state, city, severity, road type and weather
- 📈 **Skewness Lab**: distribution shape analysis
- 🧮 **Chi-Square Lab**: test of independence with expected frequencies, Pearson residuals, Cramér's V and Cochran's rule check
- 📁 **CSV upload** (drag & drop) and **CSV export** of datasets and statistical reports
- 🔄 One-click reset to the built-in demo dataset

## 🚀 Getting Started

### Option 1: Open directly
1. Download or clone this repository
2. Open `index.html` in any modern browser

### Option 2: Run a local server (optional)
```bash
python -m http.server 8000
```
Then visit http://localhost:8000

### Option 3: GitHub Pages
Go to **Settings → Pages**, select the `main` branch and root folder, and your app goes live.

> An internet connection is required on first load, since Chart.js, Leaflet, map tiles and Google Fonts load from CDNs.

## 📂 CSV Format

Uploaded files should include these columns (header names are case-insensitive):

| Column | Example |
|---|---|
| accident_id | ACC-0001 |
| date | 2024-03-15 |
| time | 18:45 |
| state | Maharashtra |
| city | Pune |
| road_type | Highway |
| weather_type | Rain |
| severity | Fatal / Serious / Minor |
| casualties | 3 |

Other columns your project expects (e.g. latitude/longitude) should be included too.

## 🛠️ Tech Stack

- HTML5, CSS3, vanilla JavaScript
- [Chart.js 4.4.1](https://www.chartjs.org/)
- [Leaflet 1.9.4](https://leafletjs.com/)
- [Inter font](https://fonts.google.com/specimen/Inter)

## 📁 Project Structure

```
RoadShape/
├── index.html        # Complete application
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

## 📄 License

Released under the MIT License. See [LICENSE](LICENSE).
