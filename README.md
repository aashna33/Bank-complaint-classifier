🧠 FinBERT Financial Complaint Classifier

Fine-tuned FinBERT model for classifying financial customer complaints across multiple product categories, with an interactive Gradio interface for real-time sentiment and category prediction.


📘 Overview

This project fine-tunes the FinBERT model (ProsusAI/finbert) on the Consumer Financial Protection Bureau (CFPB) complaints dataset.
The goal is to classify complaint narratives into financial product categories (e.g., Mortgage, Credit Card, Debt Collection, etc.), enabling institutions to detect and analyze complaint trends efficiently.


Link of the dataset: https://www.consumerfinance.gov/data-research/consumer-complaints/

🧩 Key Features

📂 Preprocessing: Loads, cleans, and filters 19K real-world complaint records

⚙️ FinBERT Fine-Tuning: Adapts pretrained ProsusAI/finbert model for multi-class classification

🧮 Model Evaluation: Computes accuracy on validation and test datasets

🖼 Interactive UI: Built with Gradio to test model predictions instantly

📊 Explainable Results: Outputs predicted label and confidence score for each complaint

📁 Dataset

The dataset used is from the Consumer Financial Protection Bureau (CFPB)
.
Each entry contains complaint details such as product, issue, and free-text narrative.

Columns of interest: Product, Issue, Consumer complaint narrative, CompanyState, Complaint ID

🚀 Training and Evaluation

Run the notebook:

jupyter notebook nlp.ipynb

🧰 Technologies Used

Python 3.10+

Transformers (Hugging Face)

PyTorch

Pandas, NumPy, scikit-learn

Gradio

🎯 Future Improvements

Add explainability with SHAP or LIME

Fine-tune model per category cluster

Deploy on Hugging Face Spaces or AWS SageMaker
