# ANN_CLASSIFICATON_CHURN

## Streamlit deployment note
If your Streamlit Cloud logs show dependency resolver failures, use this repo's latest commit and reboot the app.

This project now uses a single deployment dependency stack in `requirements.txt` that is compatible with modern Streamlit Cloud Python environments (including Python 3.13), avoiding the previous `streamlit==1.32.2` vs `numpy==2.x` conflict.

After pushing, click **Reboot app** in Streamlit Cloud to force a fresh install.
