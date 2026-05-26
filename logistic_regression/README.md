# Loan Approval Predictor — Streamlit Deployment

Quick steps to run locally and deploy to Streamlit Cloud.

1. Create a virtual environment and install pinned deps:

```bash
python -m venv .venv
source .venv/bin/activate   # macOS / Linux
.venv\\Scripts\\activate     # Windows PowerShell
pip install --upgrade pip
pip install -r requirements.txt
```

2. Run locally to verify:

```bash
streamlit run App.py
```

3. Commit and push your repo. On Streamlit Cloud (or Share), create a new app and point the app file to `logistic_regression/App.py` (or the repository subfolder containing this file).

Notes and troubleshooting:
- If the app fails loading the model with an AttributeError or InconsistentVersionWarning, ensure the deployed Python environment uses the pinned package versions in `requirements.txt`.
- If Streamlit Cloud uses a different Python, create a `runtime.txt` with the desired Python version (e.g. `python-3.11`).
- You can change the app entry file in Streamlit Cloud settings — point it to `App.py` if needed.

If you want, I can commit & push these changes and attempt to trigger a deploy — tell me to proceed.