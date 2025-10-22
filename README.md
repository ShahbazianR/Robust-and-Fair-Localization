

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
- <img width="855" height="547" alt="fig_rmse_vs_noise_all_smooth" src="https://github.com/user-attachments/assets/25465872-47fd-46ce-9513-20df059e8860" />

- `fig_fairness_vs_noise_all_smooth.png`
- <img width="855" height="547" alt="fig_fairness_vs_noise_all_smooth" src="https://github.com/user-attachments/assets/f434d868-3add-400b-b6a3-6b75bc06caa6" />

- `fig_robustness_bar_smooth.png`
- <img width="700" height="528" alt="fig_robustness_bar_smooth" src="https://github.com/user-attachments/assets/30b82d9f-e963-4d3c-b924-312b9a6332a2" />

- `fig_radar_metrics_all_smooth.png`
<img width="752" height="690" alt="fig_radar_metrics_all_smooth" src="https://github.com/user-attachments/assets/cc73b3f6-b63e-42b6-9321-5819d5754941" />

## Notes
- One chart per figure, default Matplotlib colors, and no seaborn.
- Fixed colors and markers so each method looks the same across figures.
- Seeds are set for reproducibility.
- The code is compact and commented for clarity.

## Requirements
See `requirements.txt`.

## License
MIT
