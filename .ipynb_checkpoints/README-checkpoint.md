## Explainable-AI_Drilling
## Drilling Process Parameter Optimization and Explainable AI (XAI) for ROP Prediction

## 📌 Project Overview
This project investigates the relationship between drilling process parameters using two distinct datasets. The primary objectives are:
- Developing Explainable AI (XAI) models using SHapley Additive exPlanations (SHAP) with XGBoost and Random Forest.
- Predicting the Rate of Penetration (ROP) using machine learning models.
- Optimizing process parameters for ROP using various optimization techniques, including Bayesian Optimization, Genetic Algorithms (GA), Particle Swarm Optimization (PSO), Differential Evolution (DE), and Simulated Annealing (SA).

## 📊 Datasets Used

### 1️⃣ Real-Time Drilling Data & Computed Petrophysical Output (CPO) Log Data
- **Source**: Well number 15/9-F-15 in the Volve Oil Field, North Sea.
- **Features**:
  - `Depth`: Depth of drilling
  - `WOB`: Weight on Bit
  - `SURF_RPM`: Rotation Per Minute (RPM)
  - `ROP AVG`: Rate of Penetration (Target Variable)
  - `PHIF`: Porosity
  - `VSH`: Volume of Shale
  - `SW`: Water Saturation
  - `KLOGH`: 

### 2️⃣ XAI Drilling Dataset
- **Source**: [TransAI 2023 Conference Paper](http://dx.doi.org/10.1109/TransAI60598.2023.00032)
- **Size**: 20,000 drilling operations (rows) with 10 features, 1 binary main failure label, and 4 binary subgroup failure modes.
- **Features**:
  - `ID`: Unique identifier for each data point
  - `Cutting Speed (vc)`: Speed at which the drill bit moves through material (m/min)
  - `Spindle Speed (n)`: Rotational speed of the drill bit (1/min)
  - `Feed (f)`: Depth the drill bit penetrates per revolution (mm/rev)
  - `Feed Rate (vf)`: Speed of material feed to drill bit (mm/min)
  - `Power (Pc)`: Power consumption (kW)
  - `Cooling (%)`: Cooling levels (0%, 25%, 50%, 75%, 100%)
  - `Material`: Type of material being drilled (Steel, Cast Iron, Non-Ferrous Metal)
  - `Drill Bit Type`: Type of drill bit used
  - `Process Time (t)`: Duration of drilling operation (s)
  - `Main Failure`: Binary indicator of major drilling failure
- **Subgroup Failures**:
  - `Build-up Edge Failure`: Material accumulation on the cutting edge
  - `Compression Chips Failure`: Formation of compressed chips
  - `Flank Wear Failure`: Wear on the drill bit flank
  - `Wrong Drill Bit Failure`: Incompatible drill bit usage

## 🛠 Methodology
1. **Data Preprocessing**
   - Data cleaning and handling missing values.
   - Feature engineering and scaling for better model performance.
2. **Machine Learning Models for ROP Prediction**
   - XGBoost and Random Forest models developed.
   - SHAP used for Explainable AI insights.
3. **Optimization Techniques for Process Parameter Optimization**
   - Bayesian Optimization
   - Genetic Algorithms (GA)
   - Particle Swarm Optimization (PSO)
   - Differential Evolution (DE)
   - Simulated Annealing (SA)
4. **Evaluation & Validation**
   - Model performance metrics (R², RMSE, MAE)
   - Comparison of optimization techniques for ROP improvement.

## 🚀 Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/drilling-optimization.git
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the preprocessing and modeling scripts:
   ```bash
   python train_model.py
   ```

## 📈 Results & Findings
- Explainable AI (SHAP) provided insights into the impact of each feature on ROP.
- Bayesian Optimization and Genetic Algorithms performed best in optimizing process parameters.
- Failure mode analysis from the second dataset helped identify key factors affecting drilling efficiency.

