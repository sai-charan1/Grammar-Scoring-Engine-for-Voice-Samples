# Grammar Scoring Engine for Spoken Data Samples

## Project Overview
The **Grammar Scoring Engine** is a machine learning-based solution designed to evaluate spoken data samples by predicting grammar scores. It processes audio files (45-60 seconds long) and assigns a continuous grammar score between 0 and 5, based on the MOS Likert Grammar Scores. The project uses Mel-Frequency Cepstral Coefficients (MFCCs) for feature extraction and a Random Forest Regressor for score prediction.

### Key Features
- Processes `.wav` audio files using `librosa` for feature extraction.
- Extracts MFCC features, summarized by mean and standard deviation.
- Trains a Random Forest model to predict grammar scores.
- Evaluates performance with metrics like Pearson Correlation, MSE, MAE, and R².
- Generates predictions for test data and saves them in a submission file.

### Dataset
- **Training Data**: 444 audio samples with grammar scores (in `train.csv`).
- **Testing Data**: 195 audio samples (in `test.csv` with placeholder labels).
- **Audio Files**: Stored in `.wav` format.

---

## Requirements
To run this project, you’ll need:
- **Python**: Version 3.8 or higher
- **Jupyter Notebook** or **JupyterLab**
- Python libraries listed in `requirements.txt`

### Dependencies
The project depends on the following libraries:
- `pandas`
- `numpy`
- `librosa`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`

