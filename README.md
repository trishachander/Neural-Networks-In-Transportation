# 🚌 Bus Arrival Delay Prediction using Neural Networks

## 📚 Course Information
- **Course**: AH2179
- **Module**: 7
- **Project**: Neural Network Implementation for Bus Arrival Time Delay Prediction

## 🎯 Project Overview
This project implements a neural network model to predict bus arrival delays using various activation functions and optimization techniques. The model was developed to understand the effectiveness of different neural network architectures in transportation delay prediction.

## 🏗️ Model Architecture
- **Input Layer**: Takes in preprocessed bus transit data (2000 records)
- **Hidden Layers**: 
  - First Dense Layer: 32 units
  - Second Dense Layer: 64 units
- **Output Layer**: Single unit (delay prediction)
- **Data Split**: 80% training, 20% testing

## 📊 Performance Analysis

### 🔄 Activation Function Comparison
| Activation Function | MSE | MAE | R² Score |
|-------------------|-----|-----|----------|
| relu | 1392.053759 | 29.821039 | 0.907481 |
| softmax | 18597.757826 | 82.023904 | -0.236043 |
| selu | 1397.169728 | 29.811784 | 0.907141 |
| elu | 1404.077092 | 29.880604 | 0.906682 |
| tanh | 8238.983291 | 45.722405 | 0.452421 |
| sigmoid | 8756.712782 | 46.699190 | 0.418012 |

### ⭐ Best Model Configuration
- **Activation Function**: SELU
- **Optimizer**: Adamax
- **Performance Metrics**:
  - MSE: 1385.657358
  - MAE: 29.679956
  - R² Score: 0.907907

## 📈 Training Results
The training process showed consistent improvement in model performance, with both training and validation MAE decreasing over epochs. The model achieved convergence around epoch 6, maintaining stable performance thereafter.

## 💡 Key Findings
- SELU activation function performed best among all tested functions
- The model shows good generalization with similar training and validation errors
- Performance stabilized after approximately 6 epochs
- Model achieved a high R² score of 0.907907, indicating strong predictive capability

## 🔮 Applications and Future Work
The techniques learned can be applied to various transportation problems, particularly:
- 🚗 Heavy traffic prediction during adverse weather conditions
- ⏰ Rush hour delay estimation
- 🌐 Multi-factor transportation system analysis
- ⚡ Real-time arrival prediction systems

## 🛠️ Dependencies
- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---
*Note: This project was completed as part of the AH2179 course, Module 7.* 🎓
