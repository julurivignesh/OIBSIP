# Task : Email/SMS Spam Detection with Machine Learning

## What this project does
This project builds a spam detector that can look at a text message and figure out whether it's spam or a normal ("ham") message. I used the classic SMS Spam Collection dataset, which has around 5,500 real text messages labeled as spam or ham.

## How it works
1. **Cleaned the data** — lowercased everything, stripped out punctuation and numbers, and removed common filler words (like "the", "is", "and") that don't help tell spam apart from real messages.
2. **Converted text to numbers** using TF-IDF, which basically scores each word based on how unique and important it is to a message, instead of just counting words.
3. **Trained two models** — Naive Bayes (the go-to model for text classification) and Logistic Regression — to see which one does a better job.
4. **Compared their performance** using accuracy, precision, recall, and F1-score.

## Results
| Model | Accuracy |
|---|---|
| Naive Bayes | 96.4% |
| Logistic Regression | 95.7% |

Naive Bayes performed better overall, so that's the model I went with. It's really good at not mislabeling real messages as spam, though it does miss some actual spam — a trade-off that's usually fine for spam filters since it's worse to block a real message than to let one spam text through.

## Tech used
- Python
- pandas, numpy
- scikit-learn (TF-IDF, Naive Bayes, Logistic Regression)
- NLTK (for stopword removal)
- Jupyter Notebook

## Files in this folder
- `task_spam_detection.ipynb` — the full notebook with code, results, and explanations
- `spam.csv` — the dataset used
- `README.md` — this file

## What I'd improve next
The model still misses about a quarter of actual spam messages. With more time, I'd try adding extra features (like message length or whether it contains a link), or experiment with other models to catch more spam without falsely flagging real messages.
