# Extracting-and-Visualizing-Stock-Data
Course Project: End-to-end Python project: web scraping + yfinance + pandas + Plotly to compare Tesla &amp; GameStop revenue vs share price.

# Tesla vs GameStop — Revenue vs Share Price (Python)

End-to-end analysis that **scrapes quarterly revenue**, pulls **full price history** via `yfinance`, **cleans & joins** in pandas, and **visualizes** how fundamentals track (or don’t) with market behavior.

Scrape quarterly revenue tables (HTML → BeautifulSoup → DataFrame).

Pull full trading history with yfinance (period="max").

Clean: strip $/, from revenue; to_numeric; to_datetime.

Merge & filter: align dates, handle missingness, validate shapes.

Visualize: interactive plots of price vs revenue to compare path and pace

---

## Why this project matters
Great analysts turn fuzzy questions into clear, decision-ready stories. This repo shows the full loop:
**collect → clean → validate → analyze → visualize → communicate** on real financial data (TSLA & GME).

---

## Key insights

Tesla (TSLA)

Quarterly revenue climbs from near-zero to ~$10B+ by 2021, with a visible inflection ~2018–2019.

The price regime shift (2019–2021) tracks that revenue acceleration—periods of consolidation line up with flatter revenue phases.

Takeaway: TSLA’s run is fundamentals-supported; sustained top-line growth explains the market re-rating.

GameStop (GME)

Long stretch of flat-to-declining revenue through 2016–2020 while price stays low single digits.

The 2021 price spike shows no corresponding revenue breakout—a clear decoupling from fundamentals consistent with short-squeeze dynamics.

Post-spike volatility without revenue lift underscores sentiment/structure over fundamentals.

Cross-company takeaway

Side-by-side, TSLA illustrates a fundamentals-driven trend, while GME shows a sentiment-driven anomaly.

Building this pipeline (scrape → clean → align → visualize) makes it obvious when price action is supported by the business and when it isn’t.



---

## Skills & tools demonstrated
- **Python, Jupyter**
- **Data collection:** `requests`, **BeautifulSoup** (web scraping), **yfinance** (market data)
- **Data wrangling:** `pandas` (type coercion, joins, time series), `lxml`
- **Visualization:** **Plotly** (interactive) with optional static export via `kaleido`
- **Good practice:** reproducible notebook, minimal deps, clean README, preview images

---

## Repo contents
.
├── Extracting&Visualizing_StockData.ipynb # polished, runnable notebook
├── README.md
├── requirements.txt # minimal dependencies
├── .gitignore
└── images/
├── TeslaPlot.png # optional exported figures
└── gamestop_plot.png

yaml
Copy
Edit

---

## Quickstart (local)
```bash
 install & run
pip install -r requirements.txt
jupyter notebook WebScraping-Review-Lab-v2.ipynb
Requirements (pinned in requirements.txt)
shell
Copy
Edit
beautifulsoup4>=4.12
lxml>=5.2
pandas>=2.2
requests>=2.32
yfinance>=0.2
plotly>=5.22
kaleido>=0.2
jupyter>=1.0
