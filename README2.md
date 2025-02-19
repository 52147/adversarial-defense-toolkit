
# 🛡️ Adversarial Defense Toolkit

🔗 **Demo:**
- 🎨 [Frontend (UI)](https://adversarial-defense-frontend-oaj0xjiby-52147s-projects.vercel.app/)
- 🚀 [Backend (API)](https://adversarial-defense-backend.onrender.com/)

🔗 **GitHub Repositories:**
- 📦 **Backend (FastAPI)** → [adversarial-defense-backend](https://github.com/52147/adversarial-defense-backend)
- 💻 **Frontend (React)** → [adversarial-defense-frontend](https://github.com/52147/adversarial-defense-frontend)

---

## 📖 Introduction
**Adversarial Defense Toolkit** is a tool designed to defend against adversarial attacks, supporting:
- ✅ Generation of adversarial examples
- ✅ Defense against adversarial examples using different methods
- ✅ Evaluation of defense effectiveness through classification comparison
- ✅ A user-friendly UI for easy interaction

This toolkit supports the **MNIST dataset** and provides the following **defense methods**:
- **Gaussian Blur**
- **Bilateral Filter**
- **Median Filter**
- **Auto (Apply all defenses automatically)**

---

## 🛠️ Installation & Usage

### 1️⃣ Backend (FastAPI)
#### **Run Locally**
```bash
git clone https://github.com/52147/adversarial-defense-backend.git
cd adversarial-defense-backend
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8000
```
Then, visit http://127.0.0.1:8000/docs to check the API documentation.

2️⃣ Frontend (React)

Run Locally

git clone https://github.com/52147/adversarial-defense-frontend.git
cd adversarial-defense-frontend
npm install
npm start

Set up the .env file with the API URL:

REACT_APP_API_URL=https://adversarial-defense-backend.onrender.com

📌 API Endpoints

| Method | Endpoint | Description |
|--------|---------|-------------|
| `GET`  | `/` | API health check |
| `POST` | `/upload/` | Upload and process an image |
| `GET`  | `/generate_adversarial_example?epsilon=0.3` | Generate adversarial example |
| `POST` | `/defend/` | Apply defense methods |
| `POST` | `/classify/` | Classify an image |

🏗️ Deployment

Backend (Render)

Deployed on Render:

https://adversarial-defense-backend.onrender.com/

Frontend (Vercel)

Deployed on Vercel:

https://adversarial-defense-frontend-oaj0xjiby-52147s-projects.vercel.app/

📜 License

This project is licensed under the MIT License - see the LICENSE file for details.
