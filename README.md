
# 🌟 **TDS Project 2: Data Analyst Agent** — *AI-Powered Data Sidekick*

## ✨ **Features at a Glance**

| Feature                     | Description                                        |
| --------------------------- | -------------------------------------------------- |
| 🔍 **Intelligent Analysis** | Understands your data using Google's Generative AI |
| 📈 **Dynamic Charts**       | Visualizes data with Matplotlib & Seaborn          |
| 🌐 **Web Scraping**         | Pulls data from URLs in seconds                    |
| 📁 **Multi-Format Support** | Works with CSV, Excel, JSON, Parquet, TXT          |
| 🔄 **Batch Processing**     | Answers multiple questions in one go               |
| 🎨 **Modern UI**            | Clean, responsive, and beginner-friendly           |
| ⚡ **Real-Time Results**     | Progress tracking with fast computations           |

---

## 🚀 **Quick Start**

```bash
pip install -r requirements.txt
```

### ** Set Environment Variables**

Create a `.env` file:

```env
# Google Gemini API Keys (Add 1–10 keys for load balancing if you don't have multiple key just paste your one key in all variable)
gemini_api_1=your_api_key_here
gemini_api_2=your_api_key_here
gemini_api_3=your_api_key_here
gemini_api_4=your_api_key_here
gemini_api_5=your_api_key_here
gemini_api_6=your_api_key_here
gemini_api_7=your_api_key_here
gemini_api_8=your_api_key_here
gemini_api_9=your_api_key_here
gemini_api_10=your_api_key_here
LLM_TIMEOUT_SECONDS=240
```

### ** Run the App**

```bash
python app.py
```

Then open **[http://localhost:8000](http://localhost:8000)** in your browser.

---

## 📖 **How to Use**

### **Step 1: Write Your Questions**

Create a `.txt` file:

```
What are the top-selling products?
Find correlation between variable X and Y
Show sales trends over the last 6 months
```

### **Step 2: Upload Your Data**

* **Required:** Questions file (`.txt`)
* **Optional:** Dataset in CSV/Excel/JSON/Parquet/TXT

### **Step 3: Get Your Insights**

* 🧮 **Processed by AI**
* 📊 **Visualized beautifully**
* 💡 **Actionable recommendations generated**

---

## 🛠 **Tech Stack**

**Backend**

* FastAPI 🚀 (Ultra-fast web framework)
* LangChain 🧠 (LLM orchestration)
* Google Generative AI ✨ (Smart insights)
* Pandas + NumPy 📊 (Data manipulation)
* Matplotlib + Seaborn 🎨 (Visualizations)

**Frontend**

* HTML5, CSS3, JavaScript
* Bootstrap-inspired styling for a professional look

---

## 🔧 **API Endpoints**

| Method | Endpoint   | Description                |
| ------ | ---------- | -------------------------- |
| `GET`  | `/`        | Main web interface         |
| `POST` | `/api` | Process questions + data   |
| `GET` | `/summary`  | Advanced Diagnosis of app |

---

## 📂 **Supported Data Formats**

| Format  | Extensions      |
| ------- | --------------- |
| CSV     | `.csv`          |
| Excel   | `.xlsx`, `.xls` |
| JSON    | `.json`         |
| Parquet | `.parquet`      |
| Text    | `.txt`          |

---

## 🎯 **Use Cases**

* **Business Intelligence** – Sales trends, customer insights
* **Research** – Statistical summaries, hypothesis testing
* **Data Science** – EDA, feature analysis, anomaly detection

---

## 🔒 **Security**

* Local data processing (no cloud storage)
* Environment variable protection for API keys
* Configurable CORS for production environments

---

## 🚀 **Deployment Options**

* **Local** → `python app.py`
* **Production** → `gunicorn app:app -w 4 -k uvicorn.workers.UvicornWorker`
* **Docker**

```dockerfile
FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
EXPOSE 8000
CMD ["python", "app.py"]
```

---

## 🤝 **Contributing**

We welcome PRs!

1. Fork the repo
2. Create a branch: `git checkout -b feature-name`
3. Commit + push
4. Submit PR 🚀

---

## 📜 **License**

Licensed under **MIT** — Free to use, modify, and share.

---



