# SubwayFlow: Forecasting NYC Subway Delays with Weather Patterns

**SubwayFlow** is a data analytics and forecasting project aimed at understanding and predicting NYC subway delays, particularly those affected by weather conditions. This initiative blends personal commuter frustration with technical problem-solving, resulting in a decision-support tool designed to benefit both riders and MTA operators.

---

## Why SubwayFlow?

As a daily subway rider, I often experienced delays worsened by rain or snow, with no public tool available to anticipate them. SubwayFlow was created to fill that gap by visualizing the underlying weather-delay relationship and offering predictive insights.

- Daily frustration as a commuter  
- Delays worsened by weather  
- No forecasting tools available  

> *"As someone affected by this issue, I wanted to create something that could help others like me."*

---

## Technical Approach

### Data Pipeline Workflow

```
Weather CSV + Delay CSV 
   → Clean & Merge 
   → Feature Engineering 
   → Final Modeling Dataset
```

- Combined NYC MTA delay logs with NOAA weather data  
- Cleaned and joined by date  
- Engineered new features (e.g., temperature range, snow day indicator)

#### Delay Forecasting Flow (Python)

```
Data Preparation 
   → RandomForestRegressor Setup 
   → Model Training & Prediction 
   → Visualization & Post-Processing

---

### Dashboard & Insights

The interactive dashboard (built in Power BI) visualizes:

- Delay trends over time and by line
- Correlation between temperature/rainfall and delay frequency
- Predicted future delay patterns
- Clear, Rainy, and Snow Day impact comparison

This tool helps:
- MTA operators anticipate surge conditions
- Commuters plan smarter routes

---

#### Files

| File | Description |
|------|-------------|
| `SubwayFlow.pbix` | Power BI project file with full visuals |
| `SubwayFlow_Dashboard.png` | Preview image of dashboard layout |
| `SubwayFlow.pdf` | Report summary (presentation export) |

---

#### Future Improvements

- Use real-time MTA + weather API
- Incorporate additional ML models (e.g., XGBoost, LSTM)
- Build a public web dashboard with live data feed
