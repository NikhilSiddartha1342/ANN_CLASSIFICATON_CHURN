# ANN_CLASSIFICATON_CHURN

## Streamlit deployment note
This repo uses **conditional dependencies** in `requirements.txt`:
- Python < 3.12: original stack used during model training.
- Python >= 3.12: compatibility stack for Streamlit Cloud images that provision newer Python versions.

In particular, Streamlit is version-split so newer Python environments do not hit the `streamlit==1.32.2` + `numpy==2.x` resolver conflict.

After pushing changes, use **Reboot app** in Streamlit Cloud to force a fresh dependency resolution.
