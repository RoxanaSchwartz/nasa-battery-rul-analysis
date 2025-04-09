# NASA Battery RUL Analysis

This project analyzes the Remaining Useful Life (RUL) of a battery (B0005) from NASA's Battery Dataset. It predicts when the battery capacity falls below the End of Life (EOL) threshold of 1.4 Ah using linear regression.

## Dataset
- Source: `B0005.mat` from NASA's Battery Aging ARC dataset.
- Contains 168 discharge cycles with capacity measurements.

## Analysis
- **File**: `battery_rul_B0005.ipynb`
- **Steps**:
  1. Load and extract discharge cycle capacities.
  2. Sort capacities in descending order (highest to lowest).
  3. Plot capacity degradation over cycles.
  4. Fit a linear regression model to predict RUL.
- **Results**:
  - Predicted cycles to failure (at 1.4 Ah): 127
  - First actual cycle below 1.4 Ah: 124

## Tools
- Python: `scipy`, `numpy`, `matplotlib`, `sklearn`

## Notes
- The capacity slightly "snakes" around the linear fit due to real-world battery behavior (non-linear degradation).
- Created by @RoxanaSchwartz – part of my data analysis learning journey!
