SALES PREDICTION AI - MODEL RESULTS UPGRADE

Purpose:
This app.py is a drop-in replacement for your existing four-tab Rossmann Streamlit dashboard.
Added to the Model Results tab:
 - MAE / RMSE / R2 / number of test predictions
 - Actual-vs-predicted scatter chart
 - Daily actual vs predicted trend
 - Store-wise MAE bar chart
 - Per-store prediction table, error columns, CSV download

HOW TO INSTALL
1. In VS Code, open the folder that contains your existing app.py.
2. Keep YOUR existing model.pkl, stores.csv, weekly_forecast.csv (do not overwrite them).
3. Replace app.py with the updated app.py from this ZIP.
4. Copy included test_predictions.csv to this same folder.
5. Confirm requirements.txt includes:
   streamlit>=1.40,<2
   pandas
   numpy
   matplotlib
   scikit-learn
   joblib
6. Run in VS Code terminal: streamlit run app.py
7. Open the Model Results tab and verify charts + cards.

NOTE
- The CSV here is the held-out results file YOU uploaded (9,450 rows).
- The ZIP intentionally DOES NOT include a trained model: use your own real trained model.pkl.
- Metrics reflect the data in test_predictions.csv, not a new training run.
- Original Rossmann dataset is historical; 12-week scenarios are not live forecasts.
