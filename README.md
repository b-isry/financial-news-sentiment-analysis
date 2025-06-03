# News Sentiment and Stock Moves 

This project analyzes financial news headlines to understand their impact on stock prices. The repository includes:

- Project structure
- Exploratory Data Analysis (EDA) on headline texts
- Basic descriptive statistics
- Sentiment analysis utilities
- Example Jupyter notebooks for analysis
- Unit tests for EDA and analysis functions

## Structure

- `src/`: Source code for EDA and sentiment analysis functions ([src/](src/))
    - `sentiment_analyzer.py`: Sentiment analysis utilities
- `notebooks/`: Jupyter notebooks for EDA and quantitative analysis ([notebooks/](notebooks/))
    - `EDA.ipynb`, `correlation.ipynb`, `stock_data_quant_analysis.ipynb`
- `data/`: Raw analyst ratings and historical stock data ([data/](data/))
    - `raw_analyst_ratings.csv`
    - `yfinance_data/`: Historical stock data for multiple tickers
- `tests/`: Unit tests for EDA and analysis ([tests/](tests/))
- `.github/workflows/`: CI/CD configurations ([.github/workflows/](.github/workflows/))
    - `unittests.yml`: Automated test workflow
- `.vscode/`: VS Code settings ([.vscode/](.vscode/))

## Installation

1. Clone the repository:
    ```sh
    git clone <repo-url>
    cd financial-news-sentiment-analysis
    ```

2. Install dependencies:
    ```sh
    pip install -r requirements.txt
    ```

    **Main dependencies:**
    - pandas
    - numpy
    - matplotlib
    - seaborn
    - nltk
    - scikit-learn
    - jupyter
    - pynance
    - TextBlob

## Usage

1. Start Jupyter Notebook:
    ```sh
    jupyter notebook
    ```
2. Open and run the notebooks in the `notebooks/` directory for EDA and analysis.

## Testing

Run unit tests with:
```sh
python -m unittest discover tests
```

## Data

- Place additional raw data in the `data/` directory as needed.
- Historical stock data is organized under `data/yfinance_data/`.

## CI/CD

- Automated tests are run via GitHub Actions ([.github/workflows/unittests.yml](.github/workflows/unittests.yml)) on each push.

---
