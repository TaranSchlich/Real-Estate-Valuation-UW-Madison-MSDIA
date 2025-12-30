# Real Estate Valuation Analysis
**By: Taran Schlichtmann**
**Date: 10/07/2025**
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1e-TnVDpEh6sH065Lh7a6U5-FN2e8aMra)

---

## Business Context
Analyze factors influencing property values by examining correlations between home price and key attributes such as location, age, and neighborhood amenities. Use statistical methods and visualizations to uncover insights that support data-driven real estate decisions.

---

## Learning Objectives
- Perform **data exploration** and **correlation analysis**.
- Visualize relationships between home price and key variables.
- Interpret correlation coefficients and their business implications.

---

## Repository Structure
```
.
├── gb881_assignment_5_schlichtmann_t.py   # Core analysis script
└── README.md                               # Project documentation
```

---

## Tech Stack
- Python 3.x
- Pandas — Data manipulation
- Seaborn — Visualization

---

## Dataset
- **Source**: [Real Estate Dataset](http://bit.ly/real-estate-data)
- Loaded via:
```python
url_Real_Estate = 'http://bit.ly/real-estate-data'
Dataframe_Real_Estate = pd.read_csv(url_Real_Estate)
```

---

## Objective
Explore correlations between home price per unit area and factors such as:
- House age
- Distance to MRT station
- Number of convenience stores

---

## Methodology
1. **Load & Inspect Data**: `.shape`, `.info()`, `.head()`
2. **Rename Columns** for clarity
3. **Descriptive Statistics**: `.describe()`
4. **Visualizations**:
   - Histogram of home prices
   - Scatterplot: house age vs. price
   - Heatmap of correlation matrix
5. **Correlation Analysis**:
   - Compute correlation coefficients
   - Interpret strongest relationships

---

## Results Summary
- **Distance to MRT station**: Strong negative correlation (-0.67) → closer homes are more valuable.
- **Number of convenience stores**: Moderate positive correlation (0.57) → amenities increase value.
- **House age**: Weak negative correlation (-0.21) → older homes slightly less expensive.

> **Conclusion**: Location and amenities are key drivers of home value; age has minor impact.

---

## Visualizations
- Histogram of home prices
- Scatterplot of house age vs. price
- Heatmap of correlation matrix

---

## How to Run
### Google Colab
Open: [Colab Notebook](https://colab.research.google.com/drive/1e-TnVDpEh6sH065Lh7a6U5-FN2e8aMra)

### Local Environment
```bash
# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies
pip install pandas seaborn matplotlib

# Run script
python gb881_assignment_5_schlichtmann_t.py
```

---

## Statistical Notes
- Correlation does not imply causation.
- Consider regression for predictive modeling.

---

## Future Work
- Build **linear regression models** to predict home price.
- Include **geospatial analysis** using latitude/longitude.
- Explore **time trends** in transaction dates.

---

## References
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Seaborn Documentation](https://seaborn.pydata.org/)

---

## License
MIT License — Educational use only.
