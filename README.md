# Weather Data Analysis

Analysis of 366 days of weather observations — temperature patterns, rainfall, wind, and a machine learning model to predict rain.

## What's Inside

| File | Description |
|---|---|
| `weather_analysis.ipynb` | Main analysis notebook |
| `weather.csv` | Dataset (366 days, 22 features) |
| `requirements.txt` | Python dependencies |

## Analyses Covered

1. **Monthly Temperature Trends** — min/max temperature range with rainfall overlay (interactive Plotly chart)
2. **Seasonal Statistics** — avg temperature, rainy days, total rainfall per season
3. **Correlation Heatmap** — relationships between all numeric weather features
4. **Wind Rose Chart** — rainfall distribution by wind gust direction
5. **Humidity vs Temperature** — scatter plot colored by rain tomorrow
6. **Rain Prediction (ML)** — Random Forest classifier to predict `RainTomorrow` with feature importance

## Key Findings

- Humidity at 3pm is the strongest predictor of rain the next day
- NW wind gusts are associated with the most rainfall
- ML model achieves ~80%+ accuracy predicting rain

## Setup

```bash
pip install -r requirements.txt
jupyter notebook weather_analysis.ipynb
```

## Dataset Features

`MinTemp`, `MaxTemp`, `Rainfall`, `Evaporation`, `Sunshine`, `WindGustDir`, `WindGustSpeed`, `Humidity9am`, `Humidity3pm`, `Pressure9am`, `Pressure3pm`, `Cloud9am`, `Cloud3pm`, `Temp9am`, `Temp3pm`, `RainToday`, `RainTomorrow`
