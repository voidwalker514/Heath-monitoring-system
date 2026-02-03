# Heath-monitoring-system
# healthmonitoringsystem

### 📝 The `README.md` File
# 🍃 Health360: AI-Powered Clinical Diagnostic Suite

Health360 is a comprehensive health monitoring application that combines modern machine learning with clinical data analysis. It features a **General Health Assessment** (Linear Regression) and a high-precision **13-Point Heart Disease Risk Monitor** (Logistic Regression).

---

## 🚀 Features

* **Clinical Heart Monitoring:** Analyze 13 medical parameters (BP, Cholesterol, ECG, etc.) to detect heart disease risk with ~85%+ accuracy.
* **General Health Index:** A chatbot-style interface to calculate a health score (0-100) based on lifestyle habits.
* **Ayurvedic & Modern Advice:** Integrated wellness recommendations based on diagnostic results.
* **Full-Stack Architecture:** FastAPI (Python) backend and React (Tailwind CSS) frontend.

---

## 🛠️ Project Structure

```text
Health360/
├── backend/            # FastAPI Server & ML Models
│   ├── myenv/          # Python Virtual Environment (Ignored)
│   ├── heart.csv       # Training Dataset
│   ├── main.py         # API Endpoints
│   └── train_heart_model.py
└── frontend/           # React Application
    ├── src/            # Components & Pages
    └── package.json    # Node Dependencies

```

---

## 💻 Installation & Setup

### 1. Backend Setup

Navigate to the backend folder and set up your environment:

```bash
cd backend
# Create virtual environment
python -m venv myenv

# Activate environment
# On Windows:
myenv\Scripts\activate
# On Mac/Linux:
source myenv/bin/activate

# Install dependencies
pip install fastapi uvicorn pandas scikit-learn joblib

```

### 2. Train the Models

Before running the server, you must generate the model files:

```bash
python train_model.py
python train_heart_model.py

```

### 3. Start the Backend

```bash
uvicorn main:app --reload

```

The backend will run at `http://127.0.0.1:8000`.

---

### 4. Frontend Setup

Open a new terminal and navigate to the frontend folder:

```bash
cd frontend
npm install
npm run dev

```

The frontend will run at `http://localhost:5173`.

---

## 🧪 Testing Data (Heart Monitor)

Use these values to verify the high-accuracy model:

| Field | High Risk Case | Low Risk Case |
| --- | --- | --- |
| **Age** | 63 | 37 |
| **Blood Pressure** | 145 | 130 |
| **Cholesterol** | 233 | 250 |
| **Max Heart Rate** | 150 | 187 |
| **ST Depression** | 2.3 | 0.0 |
| **Major Vessels** | 0 | 0 |

---

## ⚖️ Disclaimer

This application is an AI screening tool based on the UCI Heart Disease dataset. It is intended for educational purposes and is **not** a substitute for professional medical advice, diagnosis, or treatment.



---

### 🎨 Why this README is effective:

* **Visual Hierarchy:** Uses headings, bold text, and code blocks to make it scannable.
* **Table for Data:** Provides a quick way for anyone to test your app immediately.
* **Safety First:** Includes a medical disclaimer at the bottom, which is a standard requirement for health-related software.
* **Clear Instructions:** It guides a user through the exact order of operations (installing, training, and running).



---

### 🚀 Final Push Instructions
Since you are pushing both folders:
1.  Save this `README.md` in the root folder.
2.  Run `git add README.md`.
3.  Run `git commit -m "Added documentation"`.
4.  Run `git push origin main`.

**Would you like me to show you how to add "Badges" (like 'Build Passing' or 'Python 3.10+') to the top of your README to make it look even more professional?**
