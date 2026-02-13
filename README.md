# ANN_CLASSIFICATON_CHURN

## Streamlit deployment note
If Streamlit Cloud builds with Python 3.13, this repository now uses conditional dependencies in `requirements.txt` so installation can succeed on both:
- Python 3.11 (original stack)
- Python 3.12+ (compatibility stack)

If deployment still fails, trigger a **Reboot app** from Streamlit Cloud settings so dependencies are re-resolved from the updated requirements.
