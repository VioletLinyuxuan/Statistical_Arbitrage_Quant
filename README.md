# Statistical Arbitrage Quant

Quant research project exploring statistical arbitrage strategies on crypto
markets (Binance 4h candles, 2016 – 2025). This started as a class project
to put applied quant techniques into practice, and is being expanded into a
small research workspace.

## 📂 Project Structure

```
Statistical_Arbitrage_Quant_local/
├── Data/                 # Raw / processed market data (pickled, csv, parquet, …)
│   └── CoinData_4h_2016_2025.pkl
├── Strategy/             # Research notebooks & strategy code
│   └── ClassProject.ipynb
├── Result/               # Backtest outputs, plots, performance reports
├── requirements.txt      # Python dependencies
├── .gitignore            # Files/folders excluded from version control
└── README.md
```

## 🧰 Tech Stack

- Python 3.10+
- Jupyter Notebook
- `pandas`, `numpy` for data manipulation
- `python-binance` for market data ingestion
- `matplotlib` / `seaborn` for visualization (planned)
- `statsmodels` for cointegration / time-series tests (planned)

## 🚀 Getting Started

1. Clone the repository
   ```bash
   git clone https://github.com/VioletLinyuxuan/Statistical_Arbitrage_Quant.git
   cd Statistical_Arbitrage_Quant
   ```

2. Create and activate a virtual environment
   ```bash
   python -m venv .venv
   source .venv/bin/activate   # macOS / Linux
   # .venv\Scripts\activate    # Windows
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter and open the notebook
   ```bash
   jupyter notebook Strategy/ClassProject.ipynb
   ```

## 📊 Data

`Data/CoinData_4h_2016_2025.pkl` contains 4-hour OHLCV candles pulled from
the Binance US API. To re-pull the data, see the data ingestion cells at the
top of `Strategy/ClassProject.ipynb` (requires Binance API access).

## 📌 Roadmap

- [ ] Refactor notebook code into reusable Python modules under `src/`
- [ ] Add cointegration / pairs-selection module
- [ ] Add backtesting engine and performance reporting
- [ ] Persist outputs (equity curves, stats) into `Result/`

## 📝 License

For educational / research purposes.
