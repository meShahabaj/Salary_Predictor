# 💰 Salary Predictor App

A simple and interactive **Machine Learning web application** built with **Streamlit** and **CatBoost** that predicts an individual's salary based on their age, experience, gender, education level, and job title.

---

## 🚀 Features

* 🧠 **AI-powered salary prediction** using a trained CatBoost Regressor model
* 📊 **User-friendly Streamlit interface** for easy data input
* 🎓 Supports multiple education levels and job titles
* 💾 Model loaded locally from a `.cbm` file
* ⚡ Fast and lightweight — runs directly on CPU

---

## 🧩 Tech Stack

| Component              | Technology                    |
| ---------------------- | ----------------------------- |
| **Frontend / UI**      | Streamlit                     |
| **Backend / ML Model** | CatBoost Regressor            |
| **Language**           | Python                        |
| **Data Processing**    | pandas, numpy                 |
| **Model Storage**      | `.cbm` (CatBoost saved model) |

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/salary-predictor.git
cd salary-predictor
```

### 2. Install dependencies (using uv or pip)

#### Using **uv**:

```bash
uv add streamlit catboost pandas numpy
```

#### Or using **pip**:

```bash
pip install -r requirements.txt
```

*(If you don’t have `requirements.txt`, create one with the above libraries.)*

---

## 🧠 Model Setup

Make sure your trained model file `salary_predictor.cbm` is present in the project root folder.

If you don’t have it yet, train and export a model in Python like this:

```python
from catboost import CatBoostRegressor

model = CatBoostRegressor()
model.fit(X_train, y_train, cat_features=[2,3,4])
model.save_model("salary_predictor.cbm")
```

---

## ▶️ Run the App

Run this command in your terminal:

```bash
streamlit run main.py
```

Then open the provided local URL (like `http://localhost:8501`) in your browser.

---

## 🧾 How It Works

1. User enters:

   * Age
   * Experience (in years)
   * Gender
   * Education Level
   * Job Title
2. The app sends the input to the CatBoost model
3. Model predicts and displays the **estimated salary**

---

## 📸 Example Output

```
Age: 29  
Experience: 5 years  
Gender: Male  
Education: Master's  
Job Title: Data Scientist  

💼 Predicted Salary: ₹12,40,000 / year
```

---

## 🛠️ Project Structure

```
salary-predictor/
│
├── main.py                  # Streamlit app
├── salary_predictor.cbm     # Trained CatBoost model
├── requirements.txt          # Dependencies
├── README.md                # Project documentation
└── data/                    # (Optional) Dataset for training
```

---

## 🌟 Future Enhancements

* Add visualization of salary distribution by job role
* Integrate feature importance chart
* Deploy on Streamlit Cloud or Hugging Face Spaces

---

## 👤 Author

**Your Name**
📧 [your.email@example.com](mailto:your.email@example.com)
🌐 [LinkedIn](https://www.linkedin.com/in/your-profile) | [GitHub](https://github.com/your-username)

---

Would you like me to tailor the README specifically for **Streamlit Cloud deployment** (including dataset and model upload instructions)?
