
# ✈️ Airline Passenger Satisfaction Prediction  

## 📌 Description  
This project predicts airline passenger satisfaction using machine learning.  
We analyze passenger demographics, flight details, and service ratings, then build and compare models: **Logistic Regression**, **Decision Tree**, and **Random Forest**.  
Final predictions are generated for `test.csv`.

---

## 📊 Dataset  
- **train.csv** → used for model training & validation.  
- **test.csv** → used for final predictions.  

Features include:  
- Passenger info (Age, Gender, Customer Type).  
- Flight details (Class, Flight Distance, Type of Travel).  
- Service ratings (Inflight wifi, Cleanliness, Check-in service, etc.).  
- Delays (Departure & Arrival).  

Target: **satisfaction**  
- 0 = Neutral or Dissatisfied  
- 1 = Satisfied  

---

## ⚙️ Workflow  
1. **Data Preprocessing**  
   - Drop unnecessary columns (`id`, `Unnamed: 0`).  
   - Encode categorical variables.  

2. **EDA (Exploratory Data Analysis)**  
   - Average age per class.  
   - Flight distance per customer type.  
   - Gender vs Satisfaction counts.  
   - Class vs Satisfaction counts.  

3. **Model Training**  
   - Logistic Regression (baseline).  
   - Decision Tree (simple & explainable).  
   - Random Forest (higher accuracy).  

4. **Evaluation**  
   - Accuracy, Precision, Recall, F1-score.  
   - Prevent overfitting with parameter tuning.  

5. **Predictions**  
   - Generate results on `test.csv`.  
   - Save outputs as `logistic_predictions.csv`, `rf_predictions.csv`, `dt_predictions.csv`.  

---

## 🚀 How to Run  
```bash
# Install dependencies
pip install -r requirements.txt

# Run the model training & prediction script
python src/model.py

