

# 🛡️ Adversarial Defense Toolkit

🔗 **Demo:**
- 🎨 [前端 (UI)](https://adversarial-defense-frontend-oaj0xjiby-52147s-projects.vercel.app/)
- 🚀 [後端 (API)](https://adversarial-defense-backend.onrender.com/)

🔗 **GitHub Repositories:**
- 📦 **後端 (FastAPI)** → [adversarial-defense-backend](https://github.com/52147/adversarial-defense-backend)
- 💻 **前端 (React)** → [adversarial-defense-frontend](https://github.com/52147/adversarial-defense-frontend)

---

## 📖 簡介
**Adversarial Defense Toolkit** 是一個用於防禦對抗攻擊（Adversarial Attacks）的工具包，支援：
- ✅ 生成對抗樣本（Adversarial Examples）
- ✅ 透過不同方法進行對抗樣本防禦
- ✅ 評估防禦效果（分類對比）
- ✅ 提供簡單易用的 UI 介面

本工具包支援 **MNIST 數據集**，並提供以下 **防禦方法**：
- **Gaussian Blur（高斯模糊）**
- **Bilateral Filter（雙邊濾波）**
- **Median Filter（中值濾波）**
- **Auto（自動應用所有防禦方法）**

---

## 🛠️ 安裝與使用

### 1️⃣ 後端（Backend - FastAPI）
#### **本地運行**
```bash
git clone https://github.com/52147/adversarial-defense-backend.git
cd adversarial-defense-backend
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8000
```
然後訪問 http://127.0.0.1:8000/docs 查看 API 文件。

2️⃣ 前端（Frontend - React）

本地運行

git clone https://github.com/52147/adversarial-defense-frontend.git
cd adversarial-defense-frontend
npm install
npm start

請在 .env 文件中配置 API 地址：

REACT_APP_API_URL=https://adversarial-defense-backend.onrender.com

## 📌 API 端點（Endpoints）

| 方法 | 端點 | 描述 |
|------|------|------|
| `GET`  | `/` | API 健康檢查 |
| `POST` | `/upload/` | 上傳並處理圖片 |
| `GET`  | `/generate_adversarial_example?epsilon=0.3` | 生成對抗樣本 |
| `POST` | `/defend/` | 進行防禦 |
| `POST` | `/classify/` | 對圖片進行分類 |

🏗️ 部署（Deployment）

後端 (Render)

已部署到 Render：

https://adversarial-defense-backend.onrender.com/

前端 (Vercel)

已部署到 Vercel：

https://adversarial-defense-frontend-oaj0xjiby-52147s-projects.vercel.app/

📜 授權（License）

本項目基於 MIT License 許可，詳見 LICENSE 文件。



