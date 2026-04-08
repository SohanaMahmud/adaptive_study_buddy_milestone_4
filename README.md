# Adaptive Study Buddy — Milestone 4
 
**INSE 6450: AI in Systems Engineering | Concordia University | Winter 2026**
 
Sohana Mahmud | Student ID: 40271073
 
---
 
## Project Description
 
Binary classification system that predicts whether a student will correctly answer a question in an adaptive learning platform. Built with PyTorch using an MLP architecture (128→64→32→1) on a synthetic RIIID dataset (300,000 records). Milestone 4 adds continual learning (Experience Replay), human-in-the-loop simulation, and active learning.
 
## Repository Contents
 
- `adaptive_study_buddy_milestone4.ipynb` — Main notebook (run in Google Colab)
- `data.csv` — Dataset (300,000 rows, 5,000 users, 10,000 items)
- `milestone4_artifacts.pt` — Saved model states and configuration
- `model_config_v4.txt` — Model version info and hyperparameters
 
## How to Run
 
### Step 1: Open the Notebook
 
1. Download `adaptive_study_buddy_milestone4.ipynb` from this repository.
2. Go to [Google Colab](https://colab.research.google.com/).
3. Click **File → Upload notebook** and select the `.ipynb` file.
 
### Step 2: Upload the Dataset
 
1. Download `data.csv` from this repository to your local machine.
2. Run the first two code cells in the notebook.
3. When the **file upload dialog** appears, click **"Choose Files"** and select `data.csv`.
4. Wait until you see `Saving data.csv to data.csv` in the output.
 
### Step 3: Run All Cells
 
Go to **Runtime → Run all** or run each cell with `Shift + Enter` from top to bottom.
 
Estimated runtime: ~10–15 minutes (CPU is sufficient, no GPU needed).
 
### Step 4: View Results
 
The notebook will output all results, tables, and 5 figures automatically:
- Baseline model metrics
- Continual learning drift recovery (5 steps)
- Active learning comparison (3 strategies, 5 cycles)
- System architecture diagram
- Complete results dashboard
 
## References
 
1. RIIID Answer Correctness Prediction — https://www.kaggle.com/c/riiid-test-answer-prediction
2. Settles, B. (2010). Active Learning Literature Survey. UW–Madison.
3. Vitter, J. S. (1985). Random sampling with a reservoir. ACM TOMS.
4. Kirkpatrick, J., et al. (2017). Overcoming catastrophic forgetting. PNAS.
5. Rolnick, D., et al. (2019). Experience replay for continual learning. NeurIPS.
