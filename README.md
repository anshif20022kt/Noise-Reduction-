# Noise-Reduction-
Noise Reduction in Chaotic Time Series using Gradient Descent

This project explores reducing noise in chaotic and nonlinear time series data using a gradient descent optimization method. Real-world data (e.g., heart rhythms, climate systems, financial markets) is often messy, and filtering out noise without destroying underlying patterns is a major challenge.

We treat noise reduction as an optimization problem, minimizing the errors between what the system predicts and what we observe. Using the steepest descent algorithm, we denoise the data while preserving key dynamical features such as attractor shapes and Lyapunov exponents.

🚀 Key Contributions

Reformulated noise reduction as an optimization problem using gradient descent.  

Successfully tested on the Hénon map, demonstrating improved clarity without overfitting.

Proved that for hyperbolic systems, the method can exactly recover the original trajectory (Exact Shadowing).

Benchmarked against the Schreiber–Grassberger algorithm, showing where each method performs best.

Provided theoretical backing and experimental validation for robust, real-world noisy datasets.

🧩 Methodology

Noise Reduction as Minimization Problem

Constructed a cost function from dynamic errors.

Minimized trajectory error using gradient descent.

Gradient Descent Algorithm

Iteratively updated trajectories using steepest descent.

Preserved nonlinear dynamical invariants.

Exact Shadowing

Demonstrated that in hyperbolic systems, the denoised trajectory is identical to the true trajectory.

Comparison with Schreiber–Grassberger

Showed that while their method is simpler, our gradient descent approach is more stable under high noise.

📊 Results

Recovered clear attractor structures from noisy signals.

For the Hénon map with 1% Gaussian noise:

Dynamic error reduced by 24×.

True error reduced by 2.77× after 30 iterations.

Extended results to 3D Hénon-like systems and Lorenz-type maps.

🛠️ Tools & Libraries

Python 3

NumPy (numerical computations)

Matplotlib (visualization)

(Optional) SciPy for optimization and analysis

📂 Project Structure
├── henon_map_denoising.py   # Main implementation
├── requirements.txt         # Dependencies (NumPy, Matplotlib, etc.)
├── results/                 # Plots and figures
└── README.md                # Project documentation


Install dependencies:

pip install -r requirements.txt


Run the Hénon map demo:

python henon_map_denoising.py

📚 References

Schreiber, T. & Grassberger, P. (1991). A simple noise-reduction method for real data. Physics Letters A.

Kantz, H. & Schreiber, T. (2003). Nonlinear Time Series Analysis. Cambridge University Press.

Project Report: Noise Reduction Using Gradient Descent, Digital University of Kerala, 2025.

👩‍💻 Authors

Arshida Mahmooda

Sreya K

Neha Pramod K

Muhammed Anshif K T

Adil Rabeu T

Sishu Shankar Muni (Supervisor)
