# Data Science Notebooks for Colombia

Jupyter notebooks prepared by Eric Van Dusen (UC Berkeley College of Computing, Data Science, and Society) for students in Colombia, October 2026. Each notebook asks one question and answers it with real data, moving from economics to finance to sports.

| # | Notebook | Colab | JupyterLite |
|---|---|---|---|
| 01 | **The US Vibecession**<br>Why did Americans feel so bad about the economy after COVID, even as unemployment stayed low and inflation fell? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/01_us_vibecession.ipynb) | [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://ericvd-ucb.github.io/Colombia-26-NB/lab/index.html?path=notebooks/01_us_vibecession.ipynb) |
| 02 | **Colombia and the Vibecession**<br>Do Colombians feel worse about the economy than inflation, unemployment, interest rates and markets would predict? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/02_colombia_vibecession.ipynb) | [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://ericvd-ucb.github.io/Colombia-26-NB/lab/index.html?path=notebooks/02_colombia_vibecession.ipynb) |
| 03 | **Colombia's Economy by President**<br>Which Colombian president presided over the strongest economy, and how much does the answer depend on how you measure it? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/03_colombia_by_president.ipynb) | [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://ericvd-ucb.github.io/Colombia-26-NB/lab/index.html?path=notebooks/03_colombia_by_president.ipynb) |
| 04 | **Bollinger Bands**<br>Can a simple statistical band around a stock price tell you when to buy or sell? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/04_bollinger_bands.ipynb) | [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://ericvd-ucb.github.io/Colombia-26-NB/lab/index.html?path=notebooks/04_bollinger_bands.ipynb) |
| 05 | **Can the Model Beat the Market? ARIMA vs XGBoost**<br>Can a machine learning model (XGBoost) beat a classic econometric model (ARIMA), or just buying and holding? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/05_ml_trading_arima_vs_xgboost.ipynb) | Colab only |
| 06 | **Can the Model Beat the Market? ARIMA vs Kronos**<br>Does a foundation model trained on financial time series (Kronos) forecast better than ARIMA? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/06_ml_trading_arima_vs_kronos.ipynb) | Colab only |
| 07 | **Picking a Fantasy Premier League Team**<br>What is the best Fantasy Premier League squad you can buy with £100 million? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/07_fantasy_premier_league.ipynb) | [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://ericvd-ucb.github.io/Colombia-26-NB/lab/index.html?path=notebooks/07_fantasy_premier_league.ipynb) |
| 08 | **Introduction to SQL with Formula 1**<br>Who dominates Formula 1, and in which era? | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ericvd-ucb/Colombia-26-NB/blob/main/notebooks/08_sql_intro_f1.ipynb) | [![JupyterLite](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://ericvd-ucb.github.io/Colombia-26-NB/lab/index.html?path=notebooks/08_sql_intro_f1.ipynb) |

## How to run them

**Google Colab** (recommended): click a Colab badge. Run the first code cell (Setup) before anything else. It installs what the notebook needs and downloads saved data from this repo when required.

**JupyterLite**: click a JupyterLite badge. Everything runs inside your browser with nothing to install, but live downloads from data APIs usually do not work there, so these notebooks fall back to the saved data in `data/`.

**Your own computer**: clone the repo, `pip install -r requirements.txt`, and open the notebooks in Jupyter or VS Code.

## API keys

- `01` uses a free [FRED API key](https://fred.stlouisfed.org/docs/api/api_key.html) to download the raw data. Without one, start at Part 2, which uses the saved data.
- `05` and `06` optionally ask an LLM to critique the results (`ANTHROPIC_API_KEY` or `OPENROUTER_API_KEY`).

In Colab, add keys under **Secrets** (the key icon in the left sidebar). Never paste a key into a notebook you share.

## Repository layout

```
notebooks/   the notebooks, numbered in teaching order
data/        saved data so every notebook runs without live downloads
```

## License

Materials are shared for teaching. Data sources are credited in each notebook.
