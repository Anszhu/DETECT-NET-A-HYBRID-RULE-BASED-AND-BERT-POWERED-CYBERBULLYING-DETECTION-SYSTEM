# DetectNet

DetectNet is a final-year project prototype for multilingual cyberbullying detection. It combines:

- Rule-based NLP for transparent abusive pattern detection
- A transformer-ready ML scoring layer for contextual risk estimation
- FastAPI for backend APIs
- Streamlit for the frontend dashboard and live analysis workflow

## Project Structure

- `backend/` - API, schemas, and analysis services
- `frontend/` - Streamlit app
- `storage/` - Local evidence and report logs created at runtime

## Run Locally

1. Create a virtual environment and install dependencies:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

2. Start the FastAPI backend:

```powershell
python -m uvicorn backend.app:app --host 127.0.0.1 --port 8000
```

3. Start the Streamlit frontend in another terminal:

```powershell
python -m streamlit run frontend/streamlit_app.py --server.address 127.0.0.1 --server.port 8501
```

## Demo URLs

- Streamlit: `http://127.0.0.1:8501`
- FastAPI docs: `http://127.0.0.1:8000/docs`
