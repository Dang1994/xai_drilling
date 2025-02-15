## Digitalization of Oil and Gas Industry
## Drilling Process Parameter Optimization, prediction of rate of penitrationand and drill bit failure: Advance Optimization techniques, XGboost, Explanable AI 

## 📌 Project Overview
This project investigates the relationship between drilling process parameters using two distinct datasets. The primary objectives are:
- EDA of drilling datasets
- Developing Explainable AI (XAI) models using SHapley Additive exPlanations (SHAP) and LIME with XGBoost model.
- Predicting the Rate of Penetration (ROP) using machine learning models.
- Predicting the drill bit failure and type of failure 
- Optimizing process parameters for ROP using various optimization techniques

## 📊 Datasets Used
Here we have used two dataset:
### Dateset_1️⃣ ROP Predictio
- **Source**: https://www.kaggle.com/datasets/raphaelwallsberger/xai-drilling-dataset.
- **Features**:
  - `Depth`: Depth of drilling
  - `WOB`: Weight on Bit
  - `SURF_RPM`: Rotation Per Minute (RPM)
  - `VSH`: Volume of Shale
  - `PHIF`: Porosity
  - `SW`: Water Saturation
  - `KLOGH`:
  - `ROP AVG`: Rate of Penetration (Target Variable)


### Dataset_2️⃣ Drill Bit Failure
- **Source**: https://www.kaggle.com/datasets/raphaelwallsberger/xai-drilling-dataset.
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
1. **EDA & Data Preprocessing**
   - Data cleaning and handling missing values.
   - Feature engineering and scaling for better model performance.
   - Visualization and Statistical Analysis
2. **Machine Learning Models for ROP Prediction and drilling failure preidction**
   - XGBoost and Random Forest models developed.
   - SHAP and LIME used for Explainable AI insights.
3. **Optimization Techniques for Process Parameter Optimization: datset_1**
   - Bayesian Optimization
   - Genetic Algorithms (GA)
   - Particle Swarm Optimization (PSO)
   - Differential Evolution (DE)
   - Simulated Annealing (SA)
4. **Evaluation & Validation**
   - Model performance metrics (R², RMSE, MAE): Dataset_1 ROP
   - Model performance metrics (precision, recall, f1-score, support):
   - Comparison of optimization techniques for ROP improvement.

## 🚀 Installation & Setup
1. Clone the repository:
   ```bash
   
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the preprocessing and modeling scripts:
   ```bash
   
   ```

## 📈 Results & Findings
- Explainable AI (SHAP) provided insights into the impact of each feature on ROP.
- Bayesian Optimization and Genetic Algorithms performed best in optimizing process parameters.
- Failure mode analysis from the second dataset helped identify key factors affecting drilling efficiency.
- Drill Bit failure 

