Energy Consumption Forecasting for Smart Buildings

A full-stack web application that predicts and analyzes building energy usage with **machine learning models** and **AI-powered insights**.

---

## Key Features

* **Multi-building support**: Office, residential, retail, industrial, schools, hospitals
* **Machine Learning Forecasting**: Linear Regression, Random Forest, SVR
* **AI Insights**: GPT-powered energy optimization recommendations
* **Interactive Dashboard**: 4-tab interface (Overview, Forecast, Model Comparison, AI Insights)
* **Forecast Options**: 3, 7, 14, or 30-day predictions with real-time visualizations

---

## Tech Stack

**Frontend:** React 19, TypeScript, Tailwind, shadcn/ui, Recharts
**Backend:** FastAPI, Python 3.11+, scikit-learn, pandas, numpy, MongoDB
**DevOps:** Docker, Kubernetes, GitHub Actions, MongoDB Atlas

---

### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
pip install -r requirements.txt
uvicorn server:app --reload --port 8001
```

### Frontend Setup

```bash
cd frontend
yarn install
yarn start
```

* Frontend: [http://localhost:3000](http://localhost:3000)
* Backend API: [http://localhost:8001/docs](http://localhost:8001/docs)

---

## System Architecture

```
React (Frontend) <--> FastAPI (Backend) <--> MongoDB
        |                  |                  |
   Recharts          scikit-learn        Forecast Storage
                          |
                    OpenAI GPT-4o
```

---

## Highlights

* Achieved **R² score up to 82.8%** with Random Forest
* Designed advanced **feature engineering pipeline** (cyclical time features, lag variables, rolling averages)
* Integrated **AI-driven analysis** for building-specific optimization strategies
* Built a **responsive, production-ready dashboard**

---

## License

MIT License.

**Built to enable smarter, data-driven building energy management.**

