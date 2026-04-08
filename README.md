# CO₂ Prediction using Machine Learning

## 📌 Project Overview

This project predicts indoor carbon dioxide (CO₂) concentration using machine learning techniques based on environmental parameters such as temperature, humidity, light, and occupancy. The model helps in monitoring indoor air quality and can be used in smart buildings for ventilation control.

---

## 🎯 Objectives

* Predict indoor CO₂ concentration
* Compare multiple ML regression models
* Select best-performing model
* Save trained model for real-time prediction

---

## 📊 Dataset Features

The dataset contains the following attributes:

* Temperature
* Humidity
* Light
* CO₂
* HumidityRatio
* Occupancy
* Date (removed during preprocessing)

Target Variable:

* **CO₂ concentration**

---

## ⚙️ Preprocessing Steps

* Removed `date` column (non-numeric feature)
* Removed `HumidityRatio` (derived feature)
* Checked missing values
* Train-test split performed
* Feature selection applied

---

## 🤖 Machine Learning Models Used

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting Regressor

---

## 📈 Model Evaluation

Models were evaluated using **R² Score**.

| Model             | Performance       |
| ----------------- | ----------------- |
| Linear Regression | Low accuracy      |
| Decision Tree     | Good but unstable |
| Gradient Boosting | High accuracy     |
| Random Forest     | Best & stable     |

**Final Model Selected:** Random Forest Regressor

---

## 🧠 Why Random Forest?

* Handles non-linear relationships
* Reduces overfitting
* Stable predictions
* High R² score

---

## 💾 Model Saving

The trained model is saved using pickle:

```python
import pickle
pickle.dump(model, open('finalized_ml_mini.pkl','wb'))
```

---

## 🚀 Applications

* Smart classroom air quality monitoring
* Smart office ventilation control
* HVAC automation systems
* Smart home indoor air monitoring
* Energy-efficient building management

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

---

## 📁 Project Structure

```
CO2-prediction-using-ML
│
├── co2 pred.ipynb
├── finalized_ml_mini.pkl
├── dataset.csv
└── README.md
```

---

## 👥 Contributors

* Anora Sharon Tessie S
* Aashish M
* Abinaya Prabhu

---

## 📜 License

This project is for academic and educational purposes.

---

## ⭐ Acknowledgment

This project was developed for indoor air quality prediction using machine learning techniques.
