# Helformer Replication

This project replicates the Helformer model to evaluate its efficacy in forecasting Bitcoin (BTC) price movements.

### 📄 [Click here for the PDF](./Project_Summary.pdf)
**Key Insight:** While the replication confirmed the high statistical fit ($R^2 \approx 0.98$) reported in the original paper, the trading strategy proved highly sensitive to transaction costs. See the full report for the detailed breakdown.

## Usage

To replicate the results, run the notebooks in the following order:

1.  **Train the Model:**
    Run `Helformer model.ipynb` to train the model from scratch. Google Colab A100 is required. Estimated runtime of Step 4 (Optuna): 35min.

2.  **Run the Backtest:**
    The model is stored in Config. To run `Helformer backtesting.ipynb` on Colab, you must manually upload the following files in Config to the runtime's current directory before execution:
    > * `final_refit_model2.keras`
    > * `price_scale_const.joblib`

---
**Reference:**
Kehinde, T. O., et al. (2025). *Helformer: an attention-based deep learning model for cryptocurrency price forecasting*. Journal of Big Data. [doi:10.1186/s40537-025-01135-4](https://doi.org/10.1186/s40537-025-01135-4)
