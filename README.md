# 🧠 NeoVenue – Real Estate + Event Ticketing Intelligence Suite

![Tech](https://img.shields.io/badge/Tech-Python%20%7C%20ML%20%7C%20Streamlit%20%7C%20MySQL-informational)

> A unified machine learning platform combining real estate and event ticketing applications. Predict interests, estimate ticket prices, and generate smart recommendations – all in one place.

---

## 🔍 Modules Included

### 🎟️ 1. **Event Interest Prediction**
- Uses **Logistic Regression** to predict user interest in attending an event.
- Input: Event features (type, date, user demographics, etc.)
- Output: Binary prediction with confidence level.

### 💰 2. **Ticket Price Estimation**
- Uses **Linear Regression** to suggest a fair ticket price.
- Input: Event metadata, location, type, time
- Output: Price prediction with SHAP explainability.

### 🤝 3. **Recommendation System**
- Uses **KMeans Clustering** and **Similarity Matching** to recommend events or properties.
- Input: User preferences
- Output: Top-N relevant suggestions

---

## ⚙️ Tech Stack

- **Frontend**: Streamlit  
- **Backend**: Python  
- **Database**: MySQL  
- **ML Models**: Scikit-learn, SHAP  
- **Deployment**: Localhost / Streamlit Cloud / Docker  

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/survi09mukherjee/combned-project.git
cd combned-project
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:
```bash
pip install streamlit scikit-learn pandas numpy shap mysql-connector-python
```

### 3. Start the App

```bash
streamlit run app.py
```

---

## 🗃️ Database Setup (MySQL)

1. Create a database:
   ```sql
   CREATE DATABASE intelligence_suite;
   ```

2. Import tables using the provided SQL dump or connect from code (`db_utils.py`).

3. Configure credentials in the script:
   ```python
   connection = mysql.connector.connect(
       host="localhost",
       user="root",
       password="yourpassword",
       database="intelligence_suite"
   )
   ```

---

## 📸 Screenshots

> Screenshots taken from the [NeoVenue Portfolio](https://survimukherjeeportfolio.framer.website/portfolio/neovenue)

| Event Interest Prediction | Ticket Price Estimation | Recommendation Engine |
|---------------------------|--------------------------|------------------------|


---
![13](https://github.com/user-attachments/assets/e437e265-ef82-43c7-b56c-5c81ac726559)
![14](https://github.com/user-attachments/assets/e242d15f-891f-4ee0-818f-6c8a9d49a15a)
!![12](https://github.com/user-attachments/assets/a5cdef32-6aa7-4ee9-84ea-9687e6c5fabb)
![11](https://github.com/user-attachments/assets/615d033a-0144-41a0-96fc-ebb486d8781d)

---
## 📊 Project Architecture

```
combned-project/
├── app.py                    # Streamlit main app
├── models/                   # Saved ML models
├── utils/                    # db_utils.py, shap_utils.py
├── logs/                     # Logs for predictions
├── requirements.txt
└── README.md
```

---

## 💡 Future Enhancements

- Add user authentication  
- Enable real-time updates via API  
- Dashboard with visual insights and history  
- Emotion-aware recommendations (from facial analysis)  
- Deploy via Streamlit Cloud or Docker  

---


## 🙋‍♀️ Author

**Survi Mukherjee**  
🔗 [GitHub](https://github.com/survi09mukherjee)  
🌐 [Portfolio](https://survimukherjeeportfolio.framer.website/)

---

## ⭐ Support

If you found this project useful, give it a ⭐ and share it with others!
