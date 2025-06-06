# AI-Driven Drug Discovery Pipeline

A modular pipeline for virtual drug screening using machine learning and reinforcement learning. This project enables efficient exploration of large chemical databases like PubChem, reducing the cost and time of traditional molecular docking.

## 🔍 Features

- 🧪 **Data Preprocessing**: Converts SMILES to RDKit descriptors.
- 🤖 **ML Models**:
  - Random Forest for fast, interpretable predictions.
  - 1D CNN for deep learning-based activity prediction.
- ♻️ **Reinforcement Learning**:
  - PPO-based SMILES generator guided by RF output.
  - Custom reward function based on predicted bioactivity and drug-likeness.
- ⚙️ **Scalable Design**: Runs efficiently on standard consumer hardware.

## 📂 Project Structure

├── data/ # Input and output molecular data

├── models/ # Saved models and training scripts

├── rl_generator/ # Reinforcement learning agent

├── utils/ # Helper scripts and descriptors

├── main_pipeline.py # Main pipeline script

└── README.md


## 🧠 Contributors

- **Assylkhan Geniyat** – Reinforcement Learning & SMILES Generator  
- **Daryn Alkhaidar** – CNN Model & Evaluation  
- **Vitaliy Khan** – Random Forest & Feature Engineering  

## 📈 Results

- Screened over **119 million** compounds from PubChem.  
- Significantly reduced processing time compared to brute-force docking.  
- Generated novel, drug-like molecules with high predicted activity.

## 💻 Requirements

- Python 3.8+
- RDKit  
- scikit-learn  
- PyTorch  
- Gym (e.g., `stable-baselines3` for RL)

Install all dependencies with:
```bash
pip install -r requirements.txt
