# 🚖 Uber Ride Analytics – Predictive Analytics Dashboard

## 📌 Project Overview

Uber Ride Analytics is a data analytics and predictive analytics mini-project developed using the Uber Rides NCR dataset.

The project analyzes ride-booking data to understand booking patterns, vehicle preferences, payment methods, ride outcomes, and daily booking trends.

It includes data preprocessing, exploratory data analysis (EDA), regression, classification, time-series analysis, and an interactive dashboard to present meaningful insights.

## 🎯 Objectives

- Analyze Uber ride-booking patterns.
- Identify the most popular vehicle types.
- Study booking status and cancellation trends.
- Analyze customer payment preferences.
- Explore relationships between ride distance, booking value, and other variables.
- Build regression and classification models.
- Visualize analytical results through an interactive dashboard.

## 📂 Dataset

**Dataset:** Uber Rides NCR Dataset

- Initial records: 150,000
- Initial features: 21
- Records after duplicate removal: 148,767
- Data period: January 2024 – December 2024

The dataset includes information such as:
- Date and time
- Booking ID and customer ID
- Booking status
- Vehicle type
- Pickup and drop locations
- Booking value
- Ride distance
- Driver and customer ratings
- Payment method

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming |
| JupyterLite / Jupyter Notebook | Development environment |
| Pandas | Data manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine learning |
| Plotly | Interactive visualizations |
| HTML | Dashboard presentation |

## ⚙️ Project Methodology

1. **Data Collection:** Loaded the Uber Rides NCR dataset.
2. **Data Preprocessing:** Handled missing values and removed duplicate booking IDs.
3. **Feature Engineering:** Extracted hour, day, month, and day name from date and time.
4. **Exploratory Data Analysis:** Analyzed booking status, vehicle types, payment methods, and booking trends.
5. **Correlation Analysis:** Examined relationships among numerical variables.
6. **Predictive Modeling:** Implemented Linear Regression, Random Forest Regression, and Decision Tree Classification.
7. **Time-Series Analysis:** Analyzed daily booking trends and calculated a 7-day moving average.
8. **Dashboard Development:** Created interactive visualizations using Plotly and HTML.

## 🤖 Machine Learning Models

### 1. Regression

Models implemented:
- Linear Regression
- Random Forest Regression

**Target variable:** Booking Value

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 283.04 | 389.72 | -0.00035 |
| Random Forest | 283.66 | 390.49 | -0.00430 |

The regression models showed limited predictive performance, indicating that the selected features were not sufficient to accurately predict booking value.

### 2. Classification

**Model:** Decision Tree Classifier

**Target variable:** Ride Outcome

- Completed ride = 1
- Not completed = 0

A balanced Decision Tree model was also tested to improve detection of both classes.

| Metric | Balanced Decision Tree |
|---|---:|
| Accuracy | 52.61% |
| Precision (Completed) | 62.59% |
| Recall (Completed) | 58.61% |
| F1 Score (Completed) | 60.54% |

## 📊 Key Analytical Insights

- Total bookings after preprocessing: **148,767**
- Completed bookings: **92,248**
- Cancelled by drivers: **26,789**
- Cancelled by customers: **10,402**
- No driver found: **10,401**
- Incomplete rides: **8,927**
- Booking completion rate: **62.01%**
- Average booking value: **₹508.29**
- Average ride distance: **24.64 km**
- Peak booking hour: **6 PM**
- Most popular vehicle type: **Auto**
- Most commonly used payment method: **UPI**

## 📈 Interactive Dashboard

The project includes an interactive dashboard containing:

1. Daily Booking Analysis
2. Vehicle Type Analysis
3. Payment Method Analysis
4. Booking Status Analysis

**Dashboard file:** `Uber_Analytics_Dashboard.html`

Open the HTML file in a web browser to explore the visualizations.

## 📁 Repository Structure

```text
Uber-Ride-Analytics/
│
├── README.md
├── uber_rides.ipynb
├── ncr_ride_bookings.csv
│
├── Uber_Analytics_Dashboard.html
├── uber_daily_bookings.html
├── uber_vehicle_bookings.html
├── uber_payment_analysis.html
└── uber_booking_status.html
```

## ▶️ How to Run the Project

1. Download or clone this repository.
2. Open the notebook `uber_rides.ipynb` using Jupyter Notebook, JupyterLab, Google Colab, or JupyterLite.
3. Upload `ncr_ride_bookings.csv` into the notebook environment.
4. Install the required Python libraries if they are not already available.
5. Run the notebook cells sequentially.
6. Open `Uber_Analytics_Dashboard.html` in a browser to view the dashboard.

### Required Libraries

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
plotly
```

## 🔮 Future Scope

- Improve regression performance through additional feature engineering.
- Experiment with advanced machine learning algorithms.
- Develop more accurate ride-demand forecasting models.
- Add interactive filters for vehicle type, date, and booking status.
- Deploy the dashboard as a web application using Streamlit or another suitable framework.

## 🎓 Conclusion

This project demonstrates how data analytics and machine learning techniques can be applied to real-world ride-booking data.

It provides insights into ride demand, vehicle preferences, payment methods, and booking outcomes through data visualization and an interactive dashboard.

The project also demonstrates the practical implementation of data preprocessing, exploratory data analysis, predictive modeling, and dashboard development.

---

## 👩‍💻 Author

**Anushka Kalekar**

Electronics and Computer Engineering Student

GitHub: [Anushka-0111](https://github.com/Anushka-0111)

---

⭐ If you find this project useful, feel free to explore the repository!
