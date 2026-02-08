🦠 Infectious Disease Models – COVID-19 SEIR Modeling & Data Analysis

This repository presents a mathematical and data-driven study of COVID-19 using SEIR-based compartmental models, real-world datasets, nonlinear parameter estimation, and reproduction number analysis.

The project integrates epidemiological modeling, data preprocessing, numerical simulation, and least-squares optimization to understand disease transmission dynamics, as detailed in the MSc Phase I project report 

Project_Phase_1

.

📌 Project Overview

The main goal of this project is to model the spread of COVID-19 using SEIR-type models and calibrate them using real epidemic data from multiple regions.

Key components include:

COVID-19 time-series data analysis (India & Nigeria)

Simulation of classical and extended SEIR models

Parameter estimation using nonlinear Least Squares Method (LSM)

Computation and interpretation of the basic reproduction number (R₀)

Model validation using real cumulative case data

📊 Features

✔ Real-world COVID-19 dataset preprocessing and smoothing
✔ Implementation of extended and classical SEIR ODE systems
✔ Nonlinear least-squares parameter estimation
✔ Numerical simulations and curve fitting
✔ R₀ derivation via next-generation matrix approach
✔ Comparative analysis across regions

🧪 Methodology
🔹 Data Analysis

Collected cumulative COVID-19 confirmed case data

Cleaned inconsistencies, reporting spikes, and missing values

Applied smoothing for stable model fitting

🔹 SEIR Modeling

Implemented:

Classical SEIR model (S, E, I, R)

Extended SEIR models including quarantine and demographic effects

🔹 Parameter Estimation (LSM)

Optimized epidemiological parameters by minimizing:

𝐽
(
𝜃
)
=
∑
𝑖
=
1
𝑛
(
𝐼
𝑚
(
𝑡
𝑖
;
𝜃
)
−
𝑦
𝑖
)
2
J(θ)=
i=1
∑
n
	​

(I
m
	​

(t
i
	​

;θ)−y
i
	​

)
2

using numerical solvers (e.g., Levenberg–Marquardt).

🔹 Reproduction Number
𝑅
0
=
𝛼
1
𝛼
2
(
𝛼
2
+
𝛼
7
)
(
𝛼
3
+
𝛼
4
+
𝛼
7
)
R
0
	​

=
(α
2
	​

+α
7
	​

)(α
3
	​

+α
4
	​

+α
7
	​

)
α
1
	​

α
2
	​

	​


Used to assess transmission strength and epidemic stability.

📈 Results

Strong model fit to cumulative COVID-19 data for India and Nigeria

Realistic estimates of transmission, progression, and recovery rates

R₀ values > 1 indicating sustained transmission during study periods

Demonstrated sensitivity of parameter estimates to data preprocessing

📂 Repository Structure
Infectious-Disease-Models/
│
├── data/            # COVID-19 datasets (India, Nigeria)
├── models/         # SEIR & extended SEIR equations
├── notebooks/      # Analysis, fitting & simulations
├── results/        # Plots & fitted curves
└── README.md

🛠 Tech Stack

Python

NumPy

Pandas

SciPy (optimization & ODE solvers)

Matplotlib

🚀 Future Work

Time-varying transmission parameters

Vaccination and intervention modeling

Spatial and age-structured models

Application to other diseases (e.g., Leptospirosis)

Sensitivity & uncertainty analysis

📚 References

Key literature used includes:

SEIR model parameter estimation studies

COVID-19 real-world public datasets

Mathematical epidemiology frameworks

(Full reference list available in the project report.)
