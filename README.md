# 🏥 Healthcare Appointment No-Show Prediction

## 📌 Objective
To predict whether a patient will miss a scheduled medical appointment using historical data and provide actionable insights for improving scheduling efficiency and reducing no-show rates.

---

## 📊 Tools & Technologies
- **Python**: Pandas, Scikit-learn, Matplotlib, Seaborn
- **Power BI**: Dashboard for insights
- **Model**: Decision Tree Classifier

---

## 🧾 Dataset Summary
The dataset contains over 100k appointment records with the following features:
- `age`: Patient age
- `gender`: Male/Female
- `scholarship`: Whether the patient is enrolled in a social welfare program
- `hypertension`, `diabetes`, `alcoholism`, `handicap`: Medical conditions
- `sms_received`: Whether an SMS reminder was sent
- `neighbourhood`: Where the appointment was scheduled
- `noshow`: Target variable (Yes = missed, No = attended)

---

## 🛠️ Steps Performed

### 1. Data Preprocessing
- Removed irrelevant features (`patientId`, `appointmentId`)
- Converted date fields and handled invalid age values
- Created new features such as waiting days and weekday

### 2. Exploratory Data Analysis
- Analyzed no-show patterns across age, SMS reminders, and weekdays
- Found correlations between missed appointments and factors like SMS, waiting time

### 3. Model Training
- Trained a Decision Tree Classifier
- Achieved ~82% accuracy on the test set
- Exported model using `joblib`

### 4. Power BI Dashboard
- Built interactive visualizations:
  - No-show rate by age, gender, neighbourhood
  - Impact of SMS reminders
  - Appointment weekday patterns
- Slicers added for demographic exploration

---

## 📈 Key Insights
- SMS reminders reduce no-shows by ~30%
- Patients with longer waiting times are more likely to miss appointments
- No-show rates are higher in some neighborhoods

---

## 📦 Deliverables
- ✅ `no_show_model.pkl` - Trained ML model
- ✅ `cleaned_appointment_data.csv` - Processed dataset for BI
- ✅ Power BI `.pbix` dashboard (available on request)
- ✅ Python notebook with EDA and modeling

---

## 🧠 Optimization Suggestions
- Automate SMS reminders 1–2 days prior
- Reduce scheduling delays to under 3 days
- Consider overbooking where no-show likelihood is high

---


