# 📧 Spam Email Classification System

A machine learning-based application that classifies emails as **Spam** or **Ham (Legitimate)** using multiple classification algorithms. Built with Python and Streamlit, the system provides an interactive interface for single-email classification and batch processing of MBOX email archives.

## 🚀 Live Demo

**[Launch Spam Email Classifier](https://spam-email-detection-dznahsh4mb4owbnqrf8evq.streamlit.app/)**

## ✨ Key Features

- **Email Classification:** Predict whether an email is Spam or Ham using machine learning.
- **Multiple ML Algorithms:** Supports SVM, Logistic Regression, Decision Trees, and Random Forest.
- **Interactive Web Interface:** User-friendly Streamlit application for real-time email analysis.
- **Single Email Detection:** Classify individual emails by entering their content.
- **Batch MBOX Processing:** Upload and classify multiple emails from `.mbox` archives.
- **Performance Evaluation:** Evaluate models using Accuracy, Precision, Recall, and F1-Score.
- **Modular Architecture:** Separate components for data ingestion, transformation, training, and prediction.

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python 3.10+ |
| Frontend | Streamlit |
| Machine Learning | Scikit-learn |
| Data Processing | Pandas, NumPy |
| Text Processing | BeautifulSoup4 |
| Package Management | pip, uv |

## 📂 Project Structure

```text
Spam-Email-Detection/
│
├── app.py
├── main.py
├── requirements.txt
│
├── src/
│   ├── components/
│   ├── pipeline/
│   ├── config/
│   └── utils/
│
├── data/
├── outputs/
├── logs/
│
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yokai-og/Spam-Email-Detection.git

cd Spam-Email-Detection
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment:

**Windows:**
```powershell
.venv\Scripts\activate
```

**Linux / macOS:**
```bash
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py
```

Open the local URL provided in your terminal to access the application.

## 🖥️ Application Usage

### Single Email Classification

1. Navigate to the Single Email tab.
2. Enter or paste the email content.
3. Click the classification button.
4. View the predicted result: Spam or Ham.

### Batch MBOX Processing

1. Navigate to the Batch MBOX Processing tab.
2. Upload an `.mbox` email archive.
3. Process multiple emails.
4. Review the classification results and download the output as a CSV file.

## 🧠 Machine Learning Models

The project explores multiple classification algorithms:

- Support Vector Machine (SVM)
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

Model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score

The training pipeline uses cross-validation to evaluate model performance and identify a suitable model for prediction.

## 🔄 Model Training

To retrain the models:

1. Place the dataset at `data/dataset/dataset.csv`.
2. Execute the training pipeline:

```bash
python -m src.pipeline.training_pipeline
```

3. The generated model and vectorizer artifacts are saved in the `outputs/` directory.

Update the configuration paths if the generated artifact locations change.

## 🌐 Deployment

The application is deployed using **Streamlit Community Cloud**.

**Live Application:**  
https://spam-email-detection-dznahsh4mb4owbnqrf8evq.streamlit.app/

## 📌 Repository

**GitHub:**  
https://github.com/yokai-og/Spam-Email-Detection

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch to GitHub.
5. Open a Pull Request.

## 👨‍💻 Author

**GitHub:** [yokai-og](https://github.com/yokai-og)
