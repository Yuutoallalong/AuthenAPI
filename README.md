```md
# 🌍 AuthenAPI - Node.js Authentication API  

A **secure, lightweight authentication API** built with **Node.js, Express, MongoDB, and JWT**.  

## 🚀 Features  
- ✅ **User registration & login (JWT-based authentication)**  
- ✅ **Password hashing with bcrypt**  
- ✅ **Protected routes with token authentication**  
- ✅ **User profile retrieval**  

---

## 🛠️ Installation  

### **1️⃣ Clone the repository**  
```bash
git clone https://github.com/YOUR_GITHUB/AuthenAPI.git
cd AuthenAPI
```

### **2️⃣ Install dependencies**  
```bash
npm install
```

### **3️⃣ Set up environment variables**  
Create a `.env` file in the root directory and add:  
```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/auth-api
JWT_SECRET=your_jwt_secret_key
```

### **4️⃣ Start the server**  
```bash
npm start
```
The API will run at **`http://localhost:5000/`**.

---

## 📖 API Endpoints  

| Endpoint         | Method | Description |
|-----------------|--------|-------------|
| `/api/auth/register` | POST   | User registration |
| `/api/auth/login`    | POST   | User authentication (JWT) |
| `/api/auth/profile`  | GET    | Get user profile (requires token) |

🔹 **More APIs coming soon!**  

---

## 📝 Usage  

### **🔑 Register a User**  
```http
POST /api/auth/register
Content-Type: application/json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "securepassword"
}
```

### **🔑 Login & Get Token**  
```http
POST /api/auth/login
Content-Type: application/json
{
  "email": "john@example.com",
  "password": "securepassword"
}
```
✅ **Response**  
```json
{
  "token": "your_jwt_token"
}
```

### **🔒 Access Protected Routes**  
Send the token in the **Authorization** header:  
```http
GET /api/auth/profile
Authorization: Bearer your_jwt_token
```

---

## 📜 License  
This project is licensed under the MIT License.
