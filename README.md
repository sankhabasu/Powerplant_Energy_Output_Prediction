# ⚡ **Power Plant Energy Output Prediction using Artificial Neural Network**

An end-to-end Machine Learning project that predicts the electrical energy output of a combined-cycle power plant using an Artificial Neural Network (ANN) implemented with PyTorch.

---

# 📌 **Project Overview**

Combined-cycle power plants generate electrical energy based on several environmental and operational conditions.

This project builds an Artificial Neural Network regression model to predict power plant energy output using:

- Ambient Temperature (AT)
- Exhaust Vacuum (V)
- Ambient Pressure (AP)
- Relative Humidity (RH)

The target variable is:

- Produced Energy (PE)

The complete workflow includes data loading, preprocessing, feature scaling, tensor conversion, ANN model development, GPU-based training, model evaluation and prediction analysis.

---

# ⚙ **Technologies Used**

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- PyTorch
- Artificial Neural Network (ANN)
- ReLU Activation Function
- Adam Optimizer
- Mean Squared Error (MSE)
- R² Score
- CUDA / GPU
- Jupyter Notebook

---

# 📊 **Dataset**

- **9568 power plant records**
- **4 input features**
- **1 target variable**

### **Input Features**

| Feature | Description |
|---------|-------------|
| **AT** | Ambient Temperature |
| **V** | Exhaust Vacuum |
| **AP** | Ambient Pressure |
| **RH** | Relative Humidity |

### **Target**

| Feature | Description |
|---------|-------------|
| **PE** | Produced Electrical Energy |

The dataset was split into:

- **80% Training Data**
- **20% Testing Data**

StandardScaler was used to scale the input features before training.

---

# 🧠 **Artificial Neural Network Architecture**

The ANN consists of:

Input Layer → 4 Features

↓

Hidden Layer 1 → 6 Neurons

↓

ReLU Activation

↓

Hidden Layer 2 → 6 Neurons

↓

ReLU Activation

↓

Output Layer → 1 Neuron

↓

Predicted Energy Output

### **Architecture**

- Input Layer → **4 neurons**
- Hidden Layer 1 → **6 neurons + ReLU**
- Hidden Layer 2 → **6 neurons + ReLU**
- Output Layer → **1 neuron**

The model was implemented using PyTorch's `nn.Sequential` and trained using the Adam optimizer with Mean Squared Error (MSE) as the loss function.

---

# 🖥️ **GPU Acceleration**

The ANN was trained using GPU acceleration through CUDA.

PyTorch

↓

CUDA

↓

NVIDIA GPU

↓

ANN Training

The model was trained using an **NVIDIA GeForce RTX 2050** GPU.

---

# 📈 **Model Performance**

The trained ANN achieved the following results:

| Metric | Score |
|--------|------:|
| **Testing MSE** | **20.3985** |
| **R² Score** | **0.9287** |

### **Final Model**

**Artificial Neural Network (ANN) using PyTorch**

The model achieved an **R² score of 0.9287**, indicating strong predictive performance on the test dataset.

---

# 🚀 **Project Workflow**

Raw Dataset

↓

Data Loading

↓

Data Exploration

↓

Missing Value Check

↓

Feature & Target Separation

↓

Train-Test Split

↓

Feature Scaling using StandardScaler

↓

Conversion to PyTorch Tensors

↓

TensorDataset & DataLoader

↓

ANN Architecture Design

↓

ReLU Activation

↓

MSE Loss Function

↓

Adam Optimizer

↓

GPU-Accelerated Training using CUDA

↓

Validation & Best Model Saving

↓

Loss Visualization

↓

Model Evaluation

↓

R² Score Calculation

↓

Actual vs Predicted Values

---

# 📁 **Repository Structure**

powerplant_energy_output_prediction

├── Powerplant_Energy_Prediction.ipynb

├── powerplant_data.csv

├── Powerplant_Energy_Output_Prediction_Report.pdf

├── README.md

└── .gitignore

### **File Description**

- **Powerplant_Energy_Prediction.ipynb** → Complete ANN regression pipeline implemented using PyTorch
- **powerplant_data.csv** → Power plant energy dataset
- **Powerplant_Energy_Output_Prediction_Report.pdf** → Detailed project report
- **README.md** → Project documentation

---

# 🎯 **Key Features**

- Dataset exploration
- Missing value analysis
- Feature-target separation
- Train-test splitting
- Feature scaling
- PyTorch tensor conversion
- TensorDataset and DataLoader
- Custom ANN architecture
- ReLU activation
- MSE loss calculation
- Adam optimization
- GPU acceleration using CUDA
- Training and validation loss tracking
- Best model parameter saving
- Model evaluation using MSE
- R² score calculation
- Actual vs predicted value analysis

---

# 👨‍💻 **Author**

**Sankhasubhra Basu**

Aspiring AI & Machine Learning Engineer

If you found this project interesting, feel free to ⭐ the repository.
