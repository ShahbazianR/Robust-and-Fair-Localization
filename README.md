

# Robust & Fair Localization (RFL)

This repository includes a small, reproducible simulation for a hybrid localization method that combines:
- a learning-based prior,
- a damped Gauss–Newton refinement,
- a confidence-weighted consensus step.

It compares four methods: Optimization, Consensus (on kNN), kNN, and RFL (proposed). The notebook produces four figures and a metrics table.

## Quick start
1. Create a virtual environment (optional, but recommended).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open `RFL_notebook.ipynb` in Jupyter or Colab and run all cells.

## Output
Running the notebook saves these figures in the working directory:
- `fig_rmse_vs_noise_all_smooth.png`
- `fig_fairness_vs_noise_all_smooth.png`
- `fig_robustness_bar_smooth.png`
- `fig_radar_metrics_all_smooth.png`

## Notes
- One chart per figure, default Matplotlib colors, and no seaborn.
- Fixed colors and markers so each method looks the same across figures.
- Seeds are set for reproducibility.
- The code is compact and commented for clarity.

## Requirements
See `requirements.txt`.

## License
MIT
