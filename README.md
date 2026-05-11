# 🚗 Vehicle Service Management System

A full-stack Vehicle Service Management System built using Django REST Framework and React.js.  
The application helps service centers manage vehicle repairs, components, billing, and revenue analytics through a responsive dashboard.

---

# 📌 Project Overview

This project was developed as a Full-Stack Assignment to manage:

- Vehicle repair and service records
- Component registration and pricing
- Repair/replacement workflows
- Billing and payment simulation
- Revenue analytics dashboard

The system provides complete CRUD functionality with automatic bill calculation and responsive revenue charts.

---

# ✨ Features

## 🔧 Component Registration & Pricing Management
- Add, update, delete, and view vehicle components
- Store repair pricing and replacement/purchase pricing
- Manage stock quantities
- Search and filter components

## 🚗 Vehicle Repair Tracking
- Register vehicles requiring service
- Track repair status
- Store issue descriptions and vehicle details

## 🛠 Issue Reporting & Component Selection
- Create repair/service records
- Select repair or replacement service
- Add labor charges and component quantities

## 💳 Billing & Payment Simulation
- Automatic final bill generation
- Simulated payment workflow
- Invoice/payment summary screen
- Automatic stock deduction during replacement

## 📊 Revenue Analytics Dashboard
- Daily revenue charts
- Monthly revenue charts
- Yearly revenue charts
- Responsive graphs using Recharts

## ✅ Additional Features
- RESTful APIs
- Responsive UI using Tailwind CSS
- Toast notifications
- Loading states
- Error handling & validation
- Unit testing support

---

# 🛠 Tech Stack

## Backend
- Django
- Django REST Framework
- SQLite
- django-cors-headers

## Frontend
- React.js
- Vite
- Axios
- React Router DOM
- Tailwind CSS
- Recharts

---

# 📂 Project Structure

```bash
vehicle-management-system/
│
├── backend/
│   ├── components/
│   ├── vehicles/
│   ├── services/
│   ├── dashboard/
│   ├── vehicle_service/
│   ├── manage.py
│   ├── requirements.txt
│   └── db.sqlite3
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── api.js
│   │   └── App.jsx
│   │
│   ├── package.json
│   ├── vite.config.js
│   └── tailwind.config.js
│
└── README.md
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/vehicle-management-system.git

cd vehicle-management-system
```

---

# 🔙 Backend Setup

## Create Virtual Environment

```bash
cd backend

python -m venv .venv
```

## Activate Virtual Environment

### Windows

```bash
.venv\Scripts\activate
```

### macOS/Linux

```bash
source .venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Migrations

```bash
python manage.py migrate
```

---

## Start Backend Server

```bash
python manage.py runserver
```

Backend URL:

```bash
http://127.0.0.1:8000
```

---

# 🌐 Frontend Setup

## Navigate to Frontend

```bash
cd frontend
```

---

## Install Dependencies

```bash
npm install
```

---

## Start Frontend Development Server

```bash
npm run dev
```

Frontend URL:

```bash
http://localhost:5173
```

---

# 🔐 Environment Variables

Create a `.env` file inside the frontend folder:

```env
VITE_API_URL=http://127.0.0.1:8000/api
```

---

# 📡 API Endpoints

# Components APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/components/` | Get all components |
| POST | `/api/components/` | Create component |
| GET | `/api/components/{id}/` | Get single component |
| PUT | `/api/components/{id}/` | Update component |
| DELETE | `/api/components/{id}/` | Delete component |

### Filters

```bash
/api/components/?search=brake
/api/components/?type=engine
```

---

# Vehicles APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/vehicles/` | Get all vehicles |
| POST | `/api/vehicles/` | Create vehicle |
| GET | `/api/vehicles/{id}/` | Get single vehicle |
| PUT | `/api/vehicles/{id}/` | Update vehicle |
| DELETE | `/api/vehicles/{id}/` | Delete vehicle |

### Filters

```bash
/api/vehicles/?search=MH12
/api/vehicles/?status=Pending
```

---

# Services APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/services/` | Get all services |
| POST | `/api/services/` | Create service |
| GET | `/api/services/{id}/` | Get single service |
| PUT | `/api/services/{id}/` | Update service |
| DELETE | `/api/services/{id}/` | Delete service |

### Filters

```bash
/api/services/?vehicle=1
/api/services/?service_type=Repair
```

---

# Revenue APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/revenue/daily/` | Daily revenue |
| GET | `/api/revenue/monthly/` | Monthly revenue |
| GET | `/api/revenue/yearly/` | Yearly revenue |

---

# 💰 Billing Logic

## Repair Service

```text
repair_price × quantity + labor_charge
```

## Replacement Service

```text
purchase_price × quantity + labor_charge
```

---

# 🧪 Running Tests

```bash
cd backend

python manage.py test
```

Unit tests cover:
- Models
- APIs
- Billing calculations
- Service validations

---

# 📷 Screenshots

Add screenshots here:

- Dashboard
- Components Management
- Vehicle Registration
- Service Management
- Billing/Invoice Screen
- Revenue Analytics Dashboard

---

# 🚀 Future Enhancements

- JWT Authentication
- Role-Based Access Control
- PDF Invoice Generation
- Email Notifications
- PostgreSQL Support
- Docker Deployment
- Online Payment Integration

---

# ✅ Assignment Requirements Covered

✔ Component Registration & Pricing Management  
✔ Vehicle Repair Tracking  
✔ Issue Reporting & Component Selection  
✔ Final Price Calculation & Payment Simulation  
✔ Revenue Analytics Dashboard  
✔ Responsive Frontend Design  
✔ REST API Development  
✔ Unit Testing  
✔ Error Handling & Validation  

---

# 👨‍💻 Author

**Sneha**  
Full-Stack Developer | Django & React Developer

---
