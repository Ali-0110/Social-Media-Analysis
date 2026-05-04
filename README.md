# Social Media Data Analysis

This project explores YouTube channel performance using the YouTube Data API and Python data analysis tools.

The notebook collects video metadata from popular YouTube channels, performs cleaning and preprocessing, calculates engagement metrics, and prepares the dataset for exploratory analysis.

## Contents

- `Social Media.ipynb` - main analysis notebook
- `Figures/` - directory for charts and visual output
- `README.md` - project overview and usage instructions

## Project Overview

The notebook is designed to:

- fetch video statistics from YouTube channels
- load and inspect the raw dataset
- clean and preprocess values for analysis
- calculate an engagement rate metric
- save the collected data to `youtube_raw_data.csv`

## Key Features

- Uses the YouTube Data API to gather channel and video data
- Handles ISO 8601 duration conversion to numeric seconds
- Cleans views, likes, and comments for reliable analysis
- Derives engagement rate from likes, comments, and views
- Supports exploratory data analysis and visualization

## Setup

1. Install Python 3.10+ or a compatible Python version.
2. Create a virtual environment (recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Install required packages:

```powershell
pip install google-api-python-client pandas numpy scipy matplotlib seaborn isodate scikit-learn
```

4. Set your YouTube Data API key inside `Social Media.ipynb`:

```python
api_key = '<YOUR_API_KEY>'
```

## Usage

1. Open `Social Media.ipynb` in Jupyter or VS Code.
2. Run the notebook cells from top to bottom.
3. Update `target_channels` with any YouTube channel IDs you want to analyze.
4. Review the resulting `youtube_raw_data.csv` and any generated visualizations.

## Notes

- The notebook includes sample channels such as MrBeast, PewDiePie, TED, and more.
- API quota limits may apply when collecting video statistics.
- The notebook saves the raw YouTube data locally as `youtube_raw_data.csv`.

## License

This project is provided as an example analysis workflow for learning and exploration.
