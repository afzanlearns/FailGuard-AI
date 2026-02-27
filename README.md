# FailGuard AI  
### Predict Business Failure Before It Happens

FailGuard AI is a real-time business failure prediction platform that analyzes operational and financial health signals to detect hidden decline trajectories early. It reconstructs the causal chain behind rising risk, enabling founders and decision-makers to understand when the failure started, why it happened, and how to prevent it before collapse occurs.

---

## Problem

Most businesses do not fail suddenly. They fail gradually due to small operational and strategic decisions that compound into hidden risks over time. Traditional dashboards only display surface-level metrics and historical performance but rarely explain the origin of decline or predict future failure trajectories.

This results in delayed interventions, unclear root-cause visibility, and reactive decision-making that often arrives too late to prevent collapse.

---

## Solution

FailGuard AI introduces an explainable failure intelligence system that converts raw business metrics into predictive risk insights. Instead of only reporting what went wrong, it traces the causal timeline of decline and simulates alternate decisions to prevent future collapse.

The system computes a real-time Failure Score based on key business signals and uses AI to generate a root-cause autopsy and recovery recommendations tailored to each business scenario.

---

## Core Features

### Real-Time Failure Risk Scoring  
Instantly calculates a composite failure score using normalized business metrics such as revenue growth, burn rate ratio, churn rate, gross margin, and cash runway.

### Failure Autopsy Mode  
Reconstructs the exact chain of operational events that caused the risk trajectory, identifying when the failure started and why it escalated.

### What-If Decision Simulator  
Allows users to test alternate strategic decisions and observe their projected impact on future failure risk.

### Multi-Business Analysis  
Supports analysis of multiple businesses through manual input or CSV dataset uploads, enabling comparative risk tracking.

### AI Recovery Plan Generation  
Uses Gemini 1.5 Flash via FastAPI backend to generate actionable recovery strategies based on detected risk factors.

---

## System Architecture

FailGuard AI follows a layered architecture designed for explainability and real-time feedback:

1. **Data Input Layer**  
   Accepts manual business metrics or CSV datasets for historical analysis.

2. **Metric Normalization Engine**  
   Converts raw financial and operational data into standardized risk variables.

3. **Deterministic Scoring Engine**  
   Calculates a weighted failure risk score using client-side logic.

4. **AI Causal Reasoning Layer**  
   Generates root-cause analysis narratives and recovery plans using Gemini.

5. **Decision Intelligence Dashboard**  
   Displays live risk alerts, score trends, and simulation insights through an interactive UI.

---

## How “Real-Time” Works

FailGuard AI operates in real time by instantly recalculating failure risk whenever business metrics change. The deterministic scoring engine runs client-side in milliseconds, while the FastAPI backend generates AI-driven causal analysis and recovery strategies on demand.

This hybrid approach ensures fast responsiveness without requiring continuous external data streaming.

---

## Tech Stack

### Frontend
- React (Vite)
- Tailwind CSS
- Recharts
- Framer Motion
- PapaParse (CSV parsing)
- React Router DOM

### Backend
- FastAPI (Python)
- Gemini 1.5 Flash (AI inference)
- python-dotenv

### Deployment
- Frontend hosted on Vercel  
- Backend deployed using FastAPI service (Vercel / Render)

---

## Project Flow

1. User enters business data manually or uploads CSV dataset  
2. Metrics are normalized and passed to scoring engine  
3. Failure Score and risk factors are computed instantly  
4. Backend generates AI Failure Autopsy and Recovery Plan  
5. Dashboard visualizes risk trajectory and decision insights  

This enables proactive decision-making before business decline becomes irreversible.

---

## Installation & Setup

### Clone Repository
```bash
git clone https://github.com/afzanlearns/FailGuard-AI.git
cd FailGuard-AI

Frontend Setup
cd client
npm install
npm run dev

Backend Setup (FastAPI)
cd server
pip install -r requirements.txt
uvicorn main:app --reload

Create a .env file inside server/:

GEMINI_API_KEY=your_gemini_api_key_here
```
--- 
## Dataset Strategy

The platform supports:

- Manual metric input for instant analysis  
- CSV upload for historical business trajectory evaluation  
- Synthetic demo dataset modeled on real SMB growth and decline patterns  

These datasets allow early detection of hidden risks months before visible collapse signals appear.

---

## Use Cases

- Startup founders monitoring burn and runway risk  
- SMEs evaluating operational sustainability  
- Financial analysts detecting hidden decline signals  
- Educational case studies on business collapse trajectories  
- Decision-makers simulating strategic trade-offs  

---

## Future Scope

- Integration with CRM and accounting tools for live data ingestion  
- Advanced predictive modeling using real historical failure datasets  
- Enterprise multi-company portfolio risk dashboards  
- Automated anomaly detection and proactive alerting  

---

## Impact

FailGuard AI shifts business analytics from reactive reporting to proactive failure prevention. By combining deterministic scoring, causal AI reasoning, and simulation-based insights, the platform enables organizations to detect hidden decline signals early and make informed decisions before collapse occurs.

---

## License

This project is developed for hackathon and educational purposes. Licensing terms can be extended for production and commercial usage.

---

## Acknowledgement

Inspired by real-world startup collapse case studies where surface metrics appeared strong while underlying operational decisions gradually created invisible risks. FailGuard AI aims to make such risks visible, explainable, and preventable.
