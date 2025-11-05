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
git clone https://github.com/meShahabaj/Salary_Predictor.git
cd salary-predictor
```

### 2. Install dependencies (using uv or pip)

#### Using **uv**:

```bash
uv add streamlit catboost
```

#### Or using **pip**:

```bash
pip install streamlit catboost
```

---

## 🧠 Model Setup

Make sure your trained model file `salary_predictor.cbm` is present in the project root folder.

If you don’t have it yet, train and export a model using given notebook on kaggle:
---

## ▶️ Run the App

Run this command in your terminal:

```bash
uv run streamlit run main.py
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

💼 Predicted Salary: ₹1,40,000 / Month
```

---

## 🛠️ Project Structure

```
salary-predictor/
│
├── main.py                                 # Streamlit app
├── salary_predictor.cbm                    # Trained CatBoost model
├── README.md                               # Project documentation
└── Kaggle_training_notebook.ipynb          # notebook for training
```

---

## 🌟 Future Enhancements

* Add visualization of salary distribution by job role
* Integrate feature importance chart
* Deploy on Streamlit Cloud or Hugging Face Spaces

---

## 👤 Author

**Your Name**
📧 [shahabaj773@gmail.com]
🌐 [LinkedIn](https://www.linkedin.com/in/shahabaj-khan-b05388225/)