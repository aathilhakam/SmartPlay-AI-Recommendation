
The backend loads exported model artifacts from `models/` (via a scheduled sync or artifact registry) and serves recommendations through REST endpoints.

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **ML Libraries:** scikit-learn, pandas, NumPy
- **Notebooks:** Jupyter
- **Model Export:** joblib / pickle
- **Testing:** pytest

---

## 🔗 Integration with Backend

- Trained models are exported to `models/` and versioned.
- The Spring Boot backend consumes these via a Python microservice **or** precomputed recommendation tables.
- API contract and JSON schemas are documented in `docs/integration.md`.

---

## 🚀 Getting Started

```bash
git clone https://github.com/<your-username>/SmartPlay-AI-Recommendation.git
cd SmartPlay-AI-Recommendation
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook