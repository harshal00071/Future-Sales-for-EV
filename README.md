# 📊 Predictive Model for EV Vehcile SALES
 
A complete AI-powered sales forecasting application built using **React + TypeScript**, **FastAPI**, **SQLite**, and **Recharts**.  
This system predicts future sales, updates analytics in real-time, manages historical insights, and allows users to upload CSV/Excel data for improved forecasting.

---

## ⚡ Tech Stack

### **Frontend**

- React + TypeScript
- Vite
- TailwindCSS + shadcn/ui
- Recharts (Data Visualization)
- Lucide Icons
- React Router

### **Backend**

- FastAPI (Python)
- SQLite (Local persistent database)
- Uvicorn (ASGI Server)
- Pydantic (Request validation)
- CORS Middleware

### **Other Tools**

- Git & GitHub
- CSV/XLSX file handling
- REST API architecture

---

## 🌟 Features

### 🔮 **Sales Prediction**

- Enter product, pricing, discount, region, and season details
- FastAPI model generates predicted sales
- Confidence metrics & insights included
- Prediction results saved to database

### 📈 **Real-Time Analytics**

- Overview metrics update automatically:
  - Growth Rate
  - Active Customers
  - Total Orders
- Charts generated using Recharts:
  - Sales vs Forecast
  - Category distribution
  - Regional performance
  - Monthly trends

### 🕒 **Prediction History**

- View past prediction results
- See accuracy, trends, and actual vs predicted numbers
- Automatically updates after new predictions

### 📤 **Upload Data**

- Upload CSV/XLSX sales data
- Files stored in backend `/uploads`
- Triggers analytics refresh

### ⚙️ **Settings**

- Update user profile
- Configure prediction model settings
- Notification preferences
- Data retention & update rules
- Settings saved persistently in the backend

---

## 🛠️ Installation & Setup

### **1. Clone the Repository**

```bash
git clone <repo-url>
cd data-forecaster-x-main


##Create virtual environment:
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt


##Start backend:
uvicorn main:app --reload --port 8000

##▶️ Run Frontend (React + Vite)
##Install dependencies:
npm install

##Start dev server:
npm run dev

##🧩 Environment Variables
##Create .env in the project root:
VITE_API_BASE_URL=http://localhost:8000



##📁 Folder Structure:
project/
│
├── backend/
│   ├── main.py
│   ├── app_data.db
│   ├── uploads/
│   └── venv/
│
└── src/
    ├── pages/
    │   ├── Home.tsx
    │   ├── Prediction.tsx
    │   ├── Analytics.tsx
    │   ├── History.tsx
    │   ├── Upload.tsx
    │   └── Settings.tsx
    │
    ├── components/
    ├── lib/api.ts
    ├── App.tsx
    └── main.tsx
"# project"
```
