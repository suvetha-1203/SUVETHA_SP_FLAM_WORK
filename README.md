# SUVETHA_SP_FLAM_WORK
“Optimization-based curve fitting for unknown parameters (θ, M, X) using L1 and L2 minimization.”
# 🧮 Parametric Curve Assignment – Research & Development / AI

## 🎯 Objective
Estimate the unknown parameters **θ**, **M**, and **X** for a given parametric equation using optimization on real-world data.  
The goal is to minimize the **L1 distance** between the predicted and actual (x, y) points.

---

## 📘 Mathematical Model
\[
\begin{cases}
x(t) = t\cos(\theta) - e^{M|t|}\sin(0.3t)\sin(\theta) + X\\[6pt]
y(t) = 42 + t\sin(\theta) + e^{M|t|}\sin(0.3t)\cos(\theta)
\end{cases}
\]
Range: \( 6 < t < 60 \)

---

## 🔢 Final Optimized Parameters (L1 Fit)

| Parameter | Symbol | Value |
|------------|---------|--------|
| Angle | θ | 28.1184° |
| Exponential factor | M | 0.02139 |
| Shift | X | 54.9003 |

---

## 📊 Error Metrics

| Metric | Value |
|---------|--------|
| L1 Total Error | 37865.09 |
| MAE | 18.93 |
| RMSE | 22.76 |
| Estimated Curve Length | ≈ (your output) |

---

## 🧮 Final Parametric Equation (LaTeX)
\[
\left(
t\cos(0.4909)
- e^{0.02139|t|}\sin(0.3t)\sin(0.4909)
+ 54.9003,\ 
42 + t\sin(0.4909)
+ e^{0.02139|t|}\sin(0.3t)\cos(0.4909)
\right)
\]

---

## 📈 Plots & Analysis

- ✅ Raw Data vs Fitted Curve (L1 & L2)
- 📉 Optimization Convergence (Loss Curve)
- 📊 Residual Distribution
- 🔁 Sensitivity Analysis for θ, M, X

(Include screenshots of your plots here if you want a professional look)

---

## 🧠 Interpretation

- **θ (28.1°)** controls rotation of the curve.  
- **M (0.02139)** controls exponential amplitude or distortion.  
- **X (54.9)** shifts the curve horizontally.  
- Low RMSE and L1 error confirm that the fitted model accurately captures the shape of the data.

---

## 🔮 Future Scope

- Try **Huber Loss** for robust fitting.  
- Apply **Differential Evolution** for global optimization.  
- Explore **time-warping of t** for non-uniform sampling.  
- Integrate results into **robotics trajectory planning** or **computer vision curve fitting**.

## 🔗 Desmos Visualization (Optional)

Copy this into Desmos parametric mode:
Range: `6 ≤ t ≤ 60`

🔗 Desmos: [https://www.desmos.com/calculator/rfj91yrxob](https://www.desmos.com/calculator/rfj91yrxob)

---

## 💻 Files in this Repository

| File | Description |
|------|--------------|
| `Suvetha_SP.ipynb` | Full Kaggle notebook with code |
| `README.md` | Project summary and results |
| `README_SNIPPET.txt` | Auto-generated result summary |
| `xy_data.csv` | Input dataset (if allowed) |

---

## 🏁 Conclusion
This project demonstrates how parameter estimation, optimization, and mathematical modeling can accurately reconstruct complex parametric curves from real data.


