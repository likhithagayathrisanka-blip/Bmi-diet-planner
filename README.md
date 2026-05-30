# 🥗 BMI-Aware Diet Planner — Personalized Nutrition Recommendation System

> A smart, region-aware diet planning web app built with Flask that generates **personalized Indian meal plans** based on BMI, dietary preferences, age, and state/region.

---

## 📌 Project Overview

Most diet apps offer generic, western meal plans that don't suit Indian users. This project solves that by delivering **truly personalized diet plans** based on:
- Your **BMI category** (Underweight / Normal / Overweight / Obese)
- Your **Indian state & region** (Andhra, Punjab, etc.)
- Your **food preference** (Veg / Non-Veg)
- Your **age and gender**

---

## 🚀 Features

- ✅ Real-time BMI calculation and classification
- ✅ Region-specific Indian food recommendations
- ✅ Full day meal plan: Breakfast, Lunch, Dinner, Snacks
- ✅ Calorie targets based on BMI goal
- ✅ Water intake & exercise suggestions
- ✅ Smart filtering algorithm with fallback system
- ✅ Supports Veg & Non-Veg preferences

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS |
| Backend | Python, Flask |
| Data Processing | Pandas |
| Dataset | CSV (Indian food dataset) |

---

## 🔄 How It Works

```
User Input (Name, Age, Gender, Height, Weight, Region, State, Veg/Non-veg)
        ↓
BMI Calculation → Category (Underweight / Normal / Overweight / Obese)
        ↓
Calorie Target Calculation
        ↓
Smart Filtering Algorithm (Region → State → Veg/Non-veg preference)
        ↓
Fallback System (ensures output even if strict filters find no match)
        ↓
Output: Full Day Meal Plan + Water Intake + Exercise Plan
```

---

## 🍽️ Sample Output

**User:** Female, 24 yrs, Andhra Pradesh, Vegetarian, BMI: 27 (Overweight)

| Meal | Recommendation |
|------|---------------|
| Breakfast | Idli (3 pcs) + Sambar + Green Chutney |
| Lunch | Brown Rice + Dal + Mixed Veg Curry |
| Snacks | Sprouts Salad + Buttermilk |
| Dinner | Roti (2) + Palak Paneer + Cucumber Salad |
| Water | 2.5 litres/day |
| Exercise | 30 mins brisk walk |

---

## 🎯 Target Users

- 🧑‍🎓 Students — maintain healthy lifestyle on a budget
- 👨‍💼 Working professionals — quick personalized diet plans
- 🏋️ Fitness enthusiasts — weight gain/loss goals
- 🧓 Elderly people — controlled, safe nutrition
- 🏥 General public — prevent obesity, diabetes, and lifestyle diseases

---

## ▶️ Run Locally

```bash
# Clone the repo
git clone https://github.com/likhithagayathri-sanka/bmi-diet-planner.git
cd bmi-diet-planner

# Install dependencies
pip install flask pandas

# Run the app
python app.py

# Open in browser
http://localhost:5000
```

---

## 📁 Project Structure

```
bmi-diet-planner/
│
├── app.py              # Flask backend
├── food_dataset.csv    # Indian regional food dataset
├── templates/
│   ├── index.html      # Input form
│   └── result.html     # Diet plan output
└── static/
    └── style.css       # Styling
```

---

## 🧠 Smart Filtering Algorithm

The filtering engine works in steps:
1. **Strict filter** — Match exact region + state + veg preference + BMI category
2. **Relaxed filter** — If strict fails, drop BMI category constraint
3. **Fallback** — If relaxed fails, return popular regional defaults

This guarantees a result is **always returned**, never a blank page.

---

## 👩‍💻 Author

**Sanka Likhitha**  
B.Tech in Computer Science & Data Science — NRI Institute of Technology (2022–2026)  
📧 likhithagayathrisanka@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/likhithagayathri-sanka-8735a3314)
# Bmi-diet-planner
