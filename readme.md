# 🚀 Udyog 4.0 – Web3 Full Stack + ML Service

This project is a full-stack application with:

* 🧠 Machine Learning service (Python)
* ⚙️ Backend API (Node.js + Express)
* 🎨 Frontend (React + Vite)

---

# 📦 Project Structure

```
Backend/
Frontend/
ML_Service/
```

---

# ⚠️ Important Notes (Read First)

* `.env` files are NOT included → you must create them manually
* ML models are NOT included → you must train or download them
* `node_modules` and `venv` are NOT included

---

# 🛠️ Prerequisites

Make sure you have installed:

* Node.js (v18+ recommended)
* Python (3.9+)
* npm / yarn
* pip

---

# 📥 Clone the Repository

```bash
git clone https://github.com/rrrsahil/Web3.0.git
cd Web3.0
```

---

# ⚙️ Backend Setup

```bash
cd Backend
npm install
```

### Create `.env` file inside `Backend/`

Example:

```
PORT=5000
MONGO_URI=your_mongodb_connection
CLOUDINARY_URL=your_cloudinary_url
```

### Run backend

```bash
npm run dev
# OR
node server.js
```

---

# 🎨 Frontend Setup

```bash
cd ../Frontend
npm install
npm run dev
```

👉 App will run on:

```
http://localhost:5173
```

---

# 🧠 ML Service Setup

```bash
cd ML_Service
```

---

## 🔧 Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate   # Windows
```

---

## 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ⚠️ ML Models Required

Pre-trained models are NOT included in this repository.

---

## ▶️ Run ML Service (IMPORTANT)

ML service run karne ke liye `run.txt` file follow karo.

### Step-by-step run:

```bash
$env:TF_ENABLE_ONEDNN_OPTS=0
```

```bash
python -m uvicorn main:app --reload --port 8001
```

👉 Dono commands **one by one run karni hain**

---

## 🌐 ML Service URL

```text
http://localhost:8001
```

---

## ❗ Common Errors

### 1. Model not found

```
FileNotFoundError: saved_models/...
```

➡️ Solution: Run training script

---

### 2. TensorFlow warning / performance issue

➡️ Ensure this command is executed before running server:

```bash
$env:TF_ENABLE_ONEDNN_OPTS=0
```

---

## 🧠 Notes

* `run.txt` contains the exact commands required to start ML service
* Always run environment variable command before starting server


---

# 🔗 Running Full System

Make sure all 3 are running:

| Service  | Command        |
| -------- | -------------- |
| Backend  | npm run dev    |
| Frontend | npm run dev    |
| ML       | python main.py |

---

# ❗ Common Errors & Fixes

### 1. Missing `.env`

Error: Server not starting
➡️ Create `.env` file

---

### 2. ML model not found

Error:

```
FileNotFoundError: saved_models/...
```

➡️ Run training script

---

### 3. Port conflict

➡️ Change PORT in `.env`

---

# 🧠 Notes for Developers

* ML models are intentionally ignored via `.gitignore`
* Uploads folder is ignored
* This project is not fully decentralized yet (Web3 integration pending)

---

# 🚀 Future Improvements

* Smart contract integration
* Wallet authentication
* Decentralized storage (IPFS)

---

# 📜 License

MIT License
