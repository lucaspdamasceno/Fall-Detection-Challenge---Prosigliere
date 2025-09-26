# Fall Detection Challenge — Prosigliere

This repository contains a complete solution for **fall detection** using IMU sensor data.  
It includes data preprocessing, feature extraction, Deep Learning models (LSTM, GRU, Transformer), and optional integration with Google Gemini for explainability reports.

## 📁 Repository Structure

```
Fall-Detection-Challenge---Prosigliere/
├── AI_ML_Challenge-Data/
│   ├── sub1/
│   │   ├── ADLs/*.xlsx
│   │   ├── Falls/*.xlsx
│   │   ├── Near_Falls/*.xlsx
│   ├── sub2/
│   └── …
├── Document Reports/
│   ├── Executive Summary - Visual Results - Lucas Damasceno.pdf
│   ├── Fall Detection Challenge - Technical Report - Lucas Damasceno.pdf
│   ├── GenAI Powered - Technical Report GenAI - Lucas Damasceno.pdf
├── Fall_Detection_Challenge_code.py
├── README.md
└── requirements.txt
```

- `AI_ML_Challenge-Data/` — dataset organized by subject (sub1, sub2, …)  
- `Document Reports/` — PDF reports with visual results and technical documentation  
- `Fall_Detection_Challenge_code.py` — main executable script  
- `README.md` — this file  
- `requirements.txt` — Python dependencies

## 🚀 How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/lucaspdamasceno/Fall-Detection-Challenge---Prosigliere.git
   cd Fall-Detection-Challenge---Prosigliere
   ```

2. **(Optional but recommended) Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate    # Linux / macOS
   venv\Scripts\activate       # Windows
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare the dataset:**
   - Place the folder `AI_ML_Challenge-Data` in the project root (alongside `Fall_Detection_Challenge_code.py`).
   - Ensure the folder structure adheres to:
     ```
     AI_ML_Challenge-Data/
       ├── sub1/
       │    ├── ADLs/*.xlsx
       │    ├── Falls/*.xlsx
       │    ├── Near_Falls/*.xlsx
       ├── sub2/
       └── …
     ```

5. **Run the main script:**
   ```bash
   python Fall_Detection_Challenge_code.py
   ```

6. **(Optional) Enable Gemini integration:**
   - Provide your Google Gemini API key in the script or via environment variable:
     ```bash
     export GEMINI_API_KEY="your_key_here"
     ```
   - ⚠️ Hardcoding API keys directly in code is **not recommended**. Use environment variables or secure vaults instead.

## 📊 Outputs & Results

- Training of both **general** and **subject-specific** models  
- Evaluation metrics: Accuracy, Precision, Recall, F1-score  
- Confusion matrices  
- Final report saved in a file named like `fall_detection_report_YYYYMMDD_HHMMSS.txt`  
- Additional **PDF reports** are available in the [`Document Reports/`](./Document%20Reports) folder:
  - *Executive Summary - Visual Results*  
  - *Technical Report*  
  - *GenAI Powered Technical Report*  

## 🛠 Dependencies & Technologies

- **Python 3.9+**  
- **TensorFlow / Keras**  
- **scikit-learn**  
- **imbalanced-learn**  
- **Pandas, NumPy, SciPy**  
- **Matplotlib / Seaborn**  
- **openpyxl**  
- **google-generativeai** (for Gemini integration, optional)
