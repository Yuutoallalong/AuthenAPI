```md
# 🌍 AuthenAPI - Simple Authentication API  

A **lightweight, beginner-friendly** authentication API built with Django & Django REST Framework (DRF).  

## 🚀 Features  
- ✅ **User authentication** (JWT-based)  
- ✅ **User registration & login**  
- ✅ **Token-based authentication**  

---

## 🛠️ Installation  

```bash
git clone https://github.com/YOUR_GITHUB/AuthenAPI.git
cd AuthenAPI
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

API runs at: `http://127.0.0.1:8000/`

---

## 📖 API Endpoints  

| Endpoint         | Method | Description |
|-----------------|--------|-------------|
| `/api/register/` | POST   | User registration |
| `/api/login/`   | POST   | User authentication (JWT) |

🔹 **More APIs coming soon!**  

---

## 📜 License  
This project is licensed under the MIT License.  

---
```
