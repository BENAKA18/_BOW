# Movie Review Sentiment Analysis (LSTM Project)

## Overview
This project is the beginning of a sentiment analysis pipeline for movie reviews, intended to eventually use an LSTM (Long Short-Term Memory) neural network for classification. The notebook `LSTM.ipynb` currently covers **Task 1: Load and Understand the Dataset** — the data-loading and exploratory data analysis (EDA) stage. Model building and training are not yet implemented.

## Current Contents (`LSTM.ipynb`)

### Task 1: Load and Understand the Dataset
1. **Data Loading** — Reads `movie_reviews.csv` (a two-column dataset with `review` text and `sentiment` labels). If the file isn't found, the notebook falls back to a small built-in dummy dataset of 10 example reviews so the code can still run end-to-end.
2. **Preview** — Displays the first 10 rows of the dataset.
3. **Shape Check** — Prints the number of rows and columns.
4. **Missing Value Check** — Reports missing values per column.
5. **Class Distribution** — Counts and visualizes (bar chart) the number of Positive vs. Negative reviews using `seaborn`/`matplotlib`.
6. **Class Count** — Prints the number of unique sentiment classes.

## Requirements
- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- Jupyter Notebook

Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Dataset
Place a `movie_reviews.csv` file in the same directory as the notebook, with at minimum these columns:
| Column | Description |
|---|---|
| `review` | Text of the movie review |
| `sentiment` | Label — e.g., `Positive` / `Negative` |

If no CSV is provided, the notebook will auto-generate a small dummy dataset so you can still test the code.

## How to Run
1. Clone/download this repository.
2. Place `movie_reviews.csv` in the project folder (optional — a dummy dataset will be used otherwise).
3. Launch Jupyter:
   ```bash
   jupyter notebook LSTM.ipynb
   ```
4. Run all cells in order.

## Project Status / Next Steps
This notebook currently only performs data loading and EDA. Despite the filename, no LSTM model has been built yet. Suggested next steps to complete the project:
- [ ] Text preprocessing (cleaning, tokenization, stopword removal)
- [ ] Text vectorization / embedding (e.g., Keras `Tokenizer`, padding sequences, or pretrained embeddings like GloVe)
- [ ] Train/test split
- [ ] Build the LSTM model architecture (e.g., using TensorFlow/Keras)
- [ ] Train and evaluate the model (accuracy, precision/recall, confusion matrix)
- [ ] Save/export the trained model

## License
Add your preferred license here (e.g., MIT).
