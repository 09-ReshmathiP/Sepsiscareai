# 🏥 SepsisAI — Early Sepsis Risk Assessment System
### Allopathy + Siddha Dual Treatment Recommendation

---

## 🚀 Quick Start (VS Code)

### Prerequisites
- Python 3.8+ installed
- VS Code installed

### Step 1 — Open in VS Code
```
File → Open Folder → select "sepsis_app"
```

### Step 2 — Open Terminal in VS Code
```
Terminal → New Terminal
```

### Step 3 — Install & Setup (ONE COMMAND)
```bash
python setup.py
```
This will:
- Install all Python packages
- Train the AI models
- Auto-create the database

### Step 4 — Run the App
```bash
python app.py
```

### Step 5 — Open Browser
```
http://localhost:5000
```

### Default Login
| Field    | Value       |
|----------|-------------|
| Username | `admin`     |
| Password | `Admin@123` |

---

## 📁 Project Structure

```
sepsis_app/
├── app.py              ← Main Flask application
├── prediction.py       ← AI prediction engine
├── model_training.py   ← ML model training script
├── config.py           ← Configuration
├── setup.py            ← One-click setup
├── requirements.txt    ← Python dependencies
├── database.sql        ← MySQL schema (optional)
├── models/             ← Trained AI models (auto-created)
├── templates/          ← HTML pages
│   ├── base.html
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   ├── assess.html
│   ├── result.html
│   ├── patients.html
│   ├── patient_detail.html
│   └── profile.html
├── static/             ← CSS, JS, Images
└── instance/
    └── sepsis.db       ← SQLite database (auto-created)
```

---

## 🗄️ Database Options

### SQLite (Default — No Setup Required)
Works out-of-the-box. Database saved to `instance/sepsis.db`

### MySQL (Optional)
Set environment variables:
```bash
export DB_USER=root
export DB_PASS=yourpassword
export DB_HOST=localhost
export DB_NAME=sepsis_db
```
Then run: `mysql -u root -p < database.sql`

---

## 🤖 AI Models Used

| Model | Purpose |
|-------|---------|
| XGBoost | Primary classifier |
| LightGBM | Secondary classifier |
| Random Forest | Tertiary + Feature importance |
| **Ensemble** | Final prediction (average of 3) |

---

## 🌿 Risk Levels

| Level | Description |
|-------|-------------|
| No Sepsis | No significant indicators |
| Mild Risk | Early monitoring needed |
| Moderate Risk | Immediate assessment required |
| High Risk | Urgent ICU consideration |
| Critical Risk | Emergency intervention NOW |

---

## ⚕️ Features

- ✅ 5-tier Sepsis Risk Classification
- ✅ Allopathy Treatment Recommendations  
- ✅ Siddha Traditional Medicine Guidance
- ✅ XGBoost + LightGBM + Random Forest Ensemble
- ✅ Feature Importance Charts (SHAP-style)
- ✅ Probability Distribution Charts
- ✅ Patient Management System
- ✅ Role-based Authentication (Admin/Doctor/Researcher)
- ✅ Real-time Clinical Dashboard
- ✅ MySQL & SQLite Support
- ✅ Mobile Responsive Design
- ✅ Glassmorphism UI

---

## ⚠️ Medical Disclaimer

This system provides **educational decision-support information only** and does not replace licensed medical professionals. Always consult qualified Allopathy and Siddha practitioners for clinical decisions.

---

## 📞 Tech Stack

- **Backend:** Python Flask + SQLAlchemy
- **AI/ML:** XGBoost, LightGBM, Scikit-Learn
- **Frontend:** HTML5, CSS3, Bootstrap 5, Chart.js
- **Database:** SQLite (default) / MySQL
- **Fonts:** Inter + Playfair Display (Google Fonts)
