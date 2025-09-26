# Fall Detection Challenge - Complete Solution

This project implements a **fall detection system** using IMU sensor
data.\
It includes **data preprocessing**, **feature extraction**, **Deep
Learning models (LSTM, GRU, Transformer)**, and optional integration
with **Google Gemini** for explainability reports.

## 📂 Project Structure

-   `Fall_Detection_Challenge_code.py` → Main script
-   `AI_ML_Challenge-Data/` → Dataset organized by subject folders
    (sub1, sub2, ...)
-   Reports are automatically generated in `.txt` format

## 🚀 How to Run

1.  **Clone the repository:**

    ``` bash
    git clone https://github.com/your-username/fall-detection-challenge.git
    cd fall-detection-challenge
    ```

2.  **Create a virtual environment (optional but recommended):**

    ``` bash
    python -m venv venv
    source venv/bin/activate   # Linux/Mac
    venv\Scripts\activate    # Windows
    ```

3.  **Install dependencies:**

    ``` bash
    pip install -r requirements.txt
    ```

4.  **Prepare the dataset:**

    -   Place the folder `AI_ML_Challenge-Data` in the project root.

    -   The structure must look like this:

            AI_ML_Challenge-Data/
              ├── AI_ML_Challenge/
                  ├── sub1/
                  │    ├── ADLs/*.xlsx
                  │    ├── Falls/*.xlsx
                  │    ├── Near_Falls/*.xlsx
                  ├── sub2/
                  └── ...

5.  **Run the script:**

    ``` bash
    python Fall_Detection_Challenge_code.py
    ```

6.  **(Optional) Enable Gemini integration:**

    -   Provide your Google Gemini API Key in the script or via
        environment variable:

        ``` bash
        export GEMINI_API_KEY="your_key_here"
        ```

    -   **⚠ Warning:** Hardcoding API keys directly in code is not
        recommended. The key included in the script is only for the
        challenge and may not work properly.

## 📊 Outputs

-   Training of general and subject-specific models
-   Evaluation metrics (Accuracy, Precision, Recall, F1)
-   Confusion matrices
-   Final report saved as `fall_detection_report_YYYYMMDD_HHMMSS.txt`

## 🛠 Technologies

-   **Python 3.9+**
-   **TensorFlow / Keras**
-   **Scikit-learn**
-   **Imbalanced-learn**
-   **Pandas, Numpy, Scipy**
-   **Matplotlib / Seaborn**
-   **Google Generative AI (Gemini)** (optional)
