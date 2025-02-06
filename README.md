Linear Quadratic State Estimation
This project explores Linear Quadratic State Estimation (LQSE) techniques applied to linear dynamical systems, focusing on both theoretical formulations and practical implementations. The work delves into both input and no-input cases, addressing the challenges of state estimation in the presence of process and measurement noise.
Project Overview
The goal is to estimate system states from noisy observations using constrained least squares techniques, complemented by hyperparameter tuning and cross-validation for optimization. The project simulates different scenarios including:
No Input Case: Pure state estimation without external control inputs.
Single Input Case: Incorporating sinusoidal control inputs to analyze system robustness.
Two Input Case: Extending the system dynamics with multiple inputs to test model flexibility.
Key Concepts and Methods
Linear Dynamical System Modeling
State and measurement equations to describe system dynamics.
Handling of process (wt) and measurement (vt) noise.
Constrained Least Squares Estimation
Minimizing measurement residuals and process noise using a trade-off parameter λ.
Mathematical formulation for both input and no-input cases.
Data Generation
Simulation of state vectors, control inputs, and noise using multivariate normal distributions.
Sinusoidal inputs to test dynamic system response.
K-Fold Cross-Validation & Hyperparameter Tuning
Dividing datasets into training and testing subsets.
Tuning the regularization parameter λ to optimize model performance.
Ensuring robust results via multiple validation folds.
Implementation Details
Language: Python (Jupyter Notebooks)
Simulation Time Horizon: T = 100
Key Libraries: NumPy, SciPy, Matplotlib
Notebooks Included:
beginning.ipynb
Input_case.ipynb
Kfold_cross_validation_with_u_has_2_inputs.ipynb
Research_extension.ipynb
And more...
Results
State Estimation: Comparison between actual states and their estimates over time.
Error Analysis: Measurement of reconstruction errors across different configurations.
Optimal λ Selection:
No Input Case: λ ≈ 1000
Single Input Case: λ ≈ 10
Two Input Case: λ ≈ 1000
Visualizations: Graphical representation of state estimation accuracy, control input tracking, and error minimization.
Conclusion
This project highlights the importance of advanced state estimation techniques in dynamic systems. By integrating constrained least squares, hyperparameter tuning, and cross-validation, the model achieves reliable and accurate state predictions, even under noisy conditions.

