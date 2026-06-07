# Stochastic Interest Rate Modelling using CIR Model
##  CIR Model

The CIR model is defined as:

dr_t = κ(θ - r_t)dt + σ√(r_t) dW_t

Where:
- r_t → interest rate at time t  
- κ → mean reversion speed  
- θ → long-term mean  
- σ → volatility  
- W_t → Brownian motion  

---

## Project Structure
.
├── model.ipynb<br>
├── train_data.csv<br>
├── test_data.csv<br>
├── README.md


---

## Installation

Install dependencies:

```bash
pip install pandas numpy matplotlib scipy
```
## Data Preprocessing
Handling Missing Values
Linear interpolation
Forward/backward filling
Outlier Removal

Using IQR method:

Lower bound = Q1 - 3 × IQR
Upper bound = Q3 + 3 × IQR

## Results
Successfully Acheived a R^2 Score of ~ 0.934467(BASE CIR) and 0.934467(CIR++)
