# Suspicious Behavior Detection using Deep Learning

This repository contains a **group project** focused on applying deep learning techniques for the detection of suspicious human activities in video streams.  
Our work explores different model architectures and approaches for anomaly detection in surveillance scenarios, with all experiments implemented in Jupyter notebooks for transparency and reproducibility.

---

##  Project Overview
- **Objective:** Develop deep learning models to detect suspicious or abnormal behavior from video surveillance data.  
- **Approach:**  
  - Data preprocessing and preparation  
  - Training of custom CNN architectures  
  - Transfer learning using ResNet50  
  - Temporal sequence modeling with BiLSTMs  
- **Outcome:** A structured comparison of different modeling strategies for anomaly detection, demonstrating the strengths of each approach.

---

##  Team & Contributions
This project was completed collaboratively, with clear division of responsibilities:

- **Member 1** — Data preprocessing and pipeline design (`preprocessing.ipynb`)  
- **Member 2** — Custom CNN model development (`CNN_custom.ipynb`)  
- **Member 3** — Transfer learning with ResNet50 (`ResNet50.ipynb`)  
- **Member 4** — Temporal modeling with BiLSTM (`BiLSTM.ipynb`)  

> Note: Each notebook is self-contained and can be run independently.

---

##  Repository Structure

```
suspicious-behavior-detection-notebooks/
├── notebooks/
│   ├── preprocessing.ipynb
│   ├── CNN_custom.ipynb
│   ├── ResNet50.ipynb
│   └── BiLSTM.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```

- **notebooks/**: Contains all experimental Jupyter notebooks.  
- **requirements.txt**: Python dependencies required to run the notebooks.  
- **.gitignore**: Ensures large datasets, model checkpoints, and temporary files are excluded from version control.  

---

## Dataset
This project is designed to work with publicly available video anomaly detection datasets such as:  
- **UCF-Crime**  
- **UCSD Anomaly Detection Dataset**  
- **ShanghaiTech Campus Dataset**

Please download the dataset separately and place it under a local folder such as:

```
data/
└── raw/
    └── <dataset_name>/
        ├── train/...
        ├── val/...
        └── test/...
```

Update dataset paths inside each notebook before running.

---

##  Environment Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/suspicious-behavior-detection-notebooks.git
   cd suspicious-behavior-detection-notebooks
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv .venv
   source .venv/bin/activate        # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   python -m ipykernel install --user --name sbd_env --display-name "SBD (venv)"
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   Select the **"SBD (venv)"** kernel when running the notebooks.

---

##  How to Run

1. **`preprocessing.ipynb`**  
   - Handles dataset setup, transformations, and preparation.  

2. **`CNN_custom.ipynb`**  
   - Implements a custom CNN baseline for anomaly detection.  

3. **`ResNet50.ipynb`**  
   - Uses transfer learning with ResNet50 for feature extraction and classification.  

4. **`BiLSTM.ipynb`**  
   - Applies temporal modeling over frame features using BiLSTM.  

---

##  Future Work
- Integration of real-time video stream processing.  
- Exploration of Transformer-based architectures for video anomaly detection.  
- Deployment as a web application or edge-based system for practical use.  

---

##  License
This project is for **academic purposes**. If shared publicly, please include an open-source license (e.g., MIT) in a `LICENSE` file.

---

##  Acknowledgements
- Public datasets (UCF-Crime, UCSD, ShanghaiTech).  
- Libraries: PyTorch, TensorFlow, scikit-learn, OpenCV, NumPy, and others.  
- Research papers and tutorials that inspired this implementation.  
- Academic supervisors and mentors for their guidance.

---
