<h1 align="center">🎵 Spotify Tracks Analysis (EDA)</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Analysis-EDA-blue.svg" />
  <img src="https://img.shields.io/badge/Python-3.8+-green.svg" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange.svg" />
  <img src="https://img.shields.io/badge/Status-Complete-success.svg" />
  <img src="https://img.shields.io/github/license/rohan911438/Spotify-Tracks-Analysis" />
</p>

<p align="center">
  <b>Author:</b> Rohan Kumar (<a href="https://github.com/rohan911438">@rohan911438</a>)
</p>

---

## 📊 Overview

This repository contains an Exploratory Data Analysis (EDA) of Spotify tracks to uncover patterns and trends across audio features like danceability, energy, valence, loudness, and tempo. The goal is to understand what drives popularity and how musical characteristics have evolved over time.

The analysis is implemented in a single Jupyter notebook: `Spotify_Tracks_Analysis.ipynb`.

---

## 🎯 What you’ll learn

- Clean and preprocess Spotify track-level data
- Explore popularity distribution and outliers
- Identify top artists and recurring hit-makers
- Visualize feature relationships (correlations, pairwise plots)
- Analyze temporal trends (feature evolution across years)
- Build intuition for future ML tasks (recommendation, hit prediction)

---

## � Dataset

- Provided as: `spotify_dataset.zip`
- Expected files inside the zip (used by the notebook):
  - `spotify_tracks.csv` – main dataset with track-level audio features and metadata
  - `spotify_data_description.csv` – column descriptions/metadata

After cloning/downloading this repository, extract the zip so the CSV files are available to the notebook. The notebook reads these files from the project root by default:

```text
data = pd.read_csv('spotify_data_description.csv')
track = pd.read_csv('spotify_tracks.csv')
```

If you keep the CSVs in a subfolder, update the paths in the notebook accordingly.

---

## 🛠️ Tech stack

- Python 3.8+
- Jupyter Notebook
- pandas, numpy — data wrangling
- seaborn, matplotlib — visualization

Dependencies are listed in `requirements.txt` for convenience.

---

## ⚙️ Setup (Windows, cmd)

1) Optional: create and activate a virtual environment

```bat
py -3 -m venv .venv
.venv\Scripts\activate
```

2) Install dependencies

```bat
pip install -r requirements.txt
```

3) Extract the dataset

Unzip `spotify_dataset.zip` so that `spotify_tracks.csv` and `spotify_data_description.csv` are available in the project folder. If you extract to a subfolder, update the paths used in the notebook.

4) Open the notebook

```bat
jupyter notebook Spotify_Tracks_Analysis.ipynb
```

Run all cells. If you encounter a FileNotFoundError, verify the CSV file paths.

---

## 🔍 Notebook roadmap (high level)

1) Imports and warnings configuration
2) Data loading (tracks + data dictionary)
3) Quick data audit (shape, dtypes, missing values)
4) Cleaning and preprocessing (duplicates, basic fixes)
5) Descriptive statistics and distributions (popularity, tempo, loudness, danceability, etc.)
6) Correlation heatmap and feature relationships
7) Artist and track-level insights (top artists, recurring patterns)
8) Time-based trends (feature evolution by year)
9) Takeaways and next steps for modeling

Note: The exact names of sections/plots are implemented directly in the notebook.

---

## 📈 Example insights (from this dataset)

- Energy and loudness are strongly correlated
- Popular tracks tend to show higher danceability and tempo
- Pop dominates by volume, but other genres show strong niche patterns
- A handful of artists repeatedly appear among top-popularity tracks

Your exact results may vary depending on filtering choices and timeframe in the dataset.

---

## 📂 Repository structure

```text
Spotify-Tracks-Analysis/
├─ Spotify_Tracks_Analysis.ipynb   # Main notebook with EDA
├─ spotify_dataset.zip             # Dataset archive (extract before running)
├─ requirements.txt                # Python dependencies
├─ LICENSE                         # Project license (MIT)
└─ README.md                       # You are here
```

---

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repo
2. Create a new branch (feature/fix/docs)
3. Commit with clear messages
4. Open a Pull Request describing your change and rationale

---

## 📜 License

This project is licensed under the MIT License — see the `LICENSE` file for details.

---

## � Acknowledgements

- The open-source Python ecosystem (pandas, seaborn, matplotlib)
- Spotify datasets used for educational, non-commercial analysis

If this repository helped you, please ⭐ star it on GitHub!



