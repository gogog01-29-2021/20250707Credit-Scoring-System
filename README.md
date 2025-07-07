# 20250707Credit-Scoring-System

This project contains a scaffold for replicating the credit-scoring benchmark of Lessmann et al. (2015). The repository provides configuration files, preprocessing utilities and training scripts for building individual and ensemble models.

## Quick start

Follow the steps below to run the benchmark on a sample dataset.

1. **Install dependencies**
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
2. **Add data**
   Place the raw CSV of your chosen dataset under `data/raw`. For example, copy `AustralianCredit.csv` to `data/raw/AC.csv`.

3. **Run preprocessing and training**
   Execute the main script with the dataset name. This will carry out the nested cross validation and save the results.
   ```bash
   python main.py AC
   ```

4. **Inspect results**
   After the run finishes, metrics for each outer fold are saved to `results/metrics`. Plots will appear in `results/plots` when implemented.

These instructions allow you to reproduce the benchmark on the supplied dataset. The remaining TODOs in the code base outline further implementation details for the full replication study.
