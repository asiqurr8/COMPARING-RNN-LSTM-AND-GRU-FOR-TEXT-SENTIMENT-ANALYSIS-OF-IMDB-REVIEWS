# COMPARING-RNN-LSTM-AND-GRU-FOR-TEXT-SENTIMENT-ANALYSIS-OF-IMDB-REVIEWS
Sentiment Analysis using LSTM

## Overview
This project implements a Long Short-Term Memory (LSTM) model to perform sentiment classification on text data. The model is trained to classify reviews as either positive or negative using a deep learning approach.

## Features
- Pre-processing: Cleans and tokenizes text data
- LSTM Model: Uses an LSTM-based deep learning architecture
- Prediction Functions: Supports single and batch sentiment predictions
- Evaluation Metrics: Includes accuracy, precision, recall, F1-score, and confusion matrix
- Visualization: Plots model loss and performance metrics

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/lstm-sentiment-analysis.git
   cd lstm-sentiment-analysis
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
### Train the Model
Run the script to train the LSTM model:
```bash
python train.py
```

### Predict Sentiment
For a single review:
```python
from model import predict_sentiment
print(predict_sentiment("This movie was amazing!"))  # Output: Positive or Negative
```
For batch predictions:
```python
from model import predict_batch_sentiments
reviews = ["The product is great!", "Worst experience ever."]
print(predict_batch_sentiments(reviews))
```

## Evaluation
The model achieves an accuracy of 88% with:
- Precision: 90% (negative), 87% (positive)
- Recall: 87% (negative), 90% (positive)
- F1-score: 88% (negative), 89% (positive)

### Confusion Matrix
A confusion matrix is generated to assess classification errors.

## Results
The model successfully classifies sentiments but may require fine-tuning for better generalization.
