# Trading-ML-Project

Projekt: trenowanie i predykcja modeli LightGBM na danych z Binance (REST + WebSocket).
Cechy projektu:
- Rolling-window training z checkpointingiem (co 1000 wierszy).
- Sygnały tradingowe (z `sygnaly.py`) wyliczane i dołączane jako cechy (0–100%).
- Predykcja real-time (RT) z warunkiem zgodności `features_hash` między treningiem a inferencją.
- GUI: Dash (zakładki: Models, Training, Prediction, Validation, Logs).
- Modele: zapisywane lokalnie jako `.joblib` + `.meta.json` (nie commitujemy do Git).

## Szybki start (dev)
1. Sklonuj repo:
   ```bash
   git clone <repo_url>
   cd trading-ml-project
