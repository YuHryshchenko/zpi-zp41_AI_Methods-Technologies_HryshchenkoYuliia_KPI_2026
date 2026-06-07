# 🤖 Методи та технології штучного інтелекту
## AI Methods and Technologies — Laboratory Work

**Student:** Hryshchenko Yuliia  
**Group:** ZP-41  
**Institution:** National Technical University of Ukraine "Igor Sikorsky Kyiv Polytechnic Institute" (KPI)  
**Year:** 2025–2026  
**Specialties:** 121 Software Engineering · 123 Computer Engineering · 126 Information Systems and Technologies

---

## 📖 About the Course

This repository contains the implementation of all laboratory assignments for the educational component **"Методи та технології штучного інтелекту"** (*AI Methods and Technologies*), taught at the Faculty of Informatics and Computer Engineering, KPI.

The course covers three foundational pillars of classical AI and computational intelligence:

- **Fuzzy Logic & Fuzzy Sets** — mathematical modelling of imprecise, linguistic knowledge
- **Artificial Neural Networks** — biologically inspired learning and function approximation
- **Genetic Algorithms** — evolutionary computation and metaheuristic optimisation

Together, these paradigms form the theoretical and practical backbone of intelligent systems design, bridging the gap between hard mathematics and real-world uncertainty.

---

## 🗂️ Repository Structure

```
.
├── Lab1/   — Fuzzy membership functions and logical operations
├── Lab2/   — Two-variable function modelling with fuzzy mathematics
├── Lab3/   — Fuzzy clustering (FCM algorithm)
├── Lab4/   — Two-variable function approximation via neural networks
├── Lab5/   — Hebbian neural network simulation
├── Lab6/   — Neuro-fuzzy modelling (ANFIS / TSK network)
├── Lab7/   — Function optimisation with genetic algorithms
├── Lab8/   — Applied genetic algorithms (network & placement optimisation)
└── README.md
```

---

## 🧪 Laboratory Works

### 🔷 Lab 1 — Fuzzy Membership Functions and Set Operations

**Goal:** Construct fuzzy sets using a variety of membership function types and perform the most common logical operations over fuzzy sets.

**Topics covered:**
- Triangular (`trimf`) and trapezoidal (`trapmf`) membership functions
- Gaussian (`gaussmf`) and two-sided Gaussian (`gauss2mf`) functions
- Generalised bell-shaped function (`gbellmf`)
- Sigmoidal functions: basic (`sigmf`), differential (`dsigmf`), product (`psigmf`)
- Polynomial functions: Z-function (`zmf`), PI-function (`pimf`), S-function (`smf`)
- Minimax interpretation of logical operators (min/max conjunction & disjunction)
- Probabilistic interpretation of conjunctive and disjunctive operators
- Fuzzy set complement

**Libraries:** `scikit-fuzzy` (`skfuzzy`), `numpy`, `matplotlib`

---

### 🔷 Lab 2 — Two-Variable Function Modelling with Fuzzy Mathematics

**Goal:** Build and analyse a Mamdani-type fuzzy inference system for modelling a function of two input variables.

**Topics covered:**
- Fuzzy rule base construction
- Mamdani fuzzy inference engine
- Defuzzification (centroid, bisector, mean-of-maximum methods)
- 3D surface visualisation of the fuzzy model output
- Comparison of approximation quality across different membership function configurations

**Libraries:** `scikit-fuzzy`, `numpy`, `matplotlib`, `mpl_toolkits`

---

### 🔷 Lab 3 — Fuzzy Clustering Algorithm (FCM)

**Goal:** Investigate and implement the Fuzzy C-Means (FCM) clustering algorithm and analyse its behaviour on different datasets.

**Topics covered:**
- Principles of fuzzy (soft) clustering vs. hard clustering
- FCM objective function and iterative optimisation
- Membership degree matrix and cluster centre update rules
- Effect of the fuzziness parameter *m* on cluster boundaries
- Cluster validity indices

**Libraries:** `scikit-fuzzy`, `numpy`, `matplotlib`, `sklearn`

---

### 🔷 Lab 4 — Neural Network Function Approximation (MISO)

**Goal:** Model a two-variable function using a feedforward artificial neural network with two inputs and one output (MISO — Multiple Input, Single Output).

**Topics covered:**
- Multi-layer perceptron (MLP) architecture design
- Backpropagation training algorithm
- Activation functions: sigmoid, ReLU, tanh
- Loss function selection and gradient descent
- Approximation accuracy evaluation; comparison with the target function surface

**Libraries:** `tensorflow` / `keras` or `torch`, `numpy`, `matplotlib`

---

### 🔷 Lab 5 — Hebbian Neural Network

**Goal:** Simulate a Hebbian learning neural network and study the fundamental unsupervised weight-update rule that underlies associative memory.

**Topics covered:**
- Hebb's learning rule: biological motivation and mathematical formulation
- Weight matrix initialisation and incremental update
- Pattern storage and associative recall
- Hopfield network as an extension of Hebbian learning
- Analysis of storage capacity and noise tolerance

**Libraries:** `numpy`, `matplotlib`

---

### 🔷 Lab 6 — Neuro-Fuzzy Modelling (ANFIS / TSK)

**Goal:** Acquire and reinforce knowledge of neuro-fuzzy system design and implement a Takagi–Sugeno–Kang (TSK) type neuro-fuzzy network for forecasting tasks.

**Topics covered:**
- Architecture of the ANFIS (Adaptive Neuro-Fuzzy Inference System)
- TSK inference model with generalised *M*-rule, *N*-variable scheme
- Hybrid learning: gradient descent + least-squares estimation
- Application to economic time-series forecasting under uncertainty
- Interpretability of fuzzy rules extracted from the network

**Libraries:** `scikit-fuzzy`, `numpy`, `pandas`, `matplotlib`, optionally `anfis` or custom implementation

---

### 🔷 Lab 7 — Function Optimisation with Genetic Algorithms

**Goal:** Find minima and maxima of mathematical functions using a classical genetic algorithm and study the influence of GA parameters on convergence.

**Topics covered:**
- Genetic algorithm structure: population, chromosome, fitness function
- Selection operators: roulette wheel, tournament, rank-based
- Crossover operators: single-point, two-point, uniform
- Mutation operators and mutation probability effects
- Convergence analysis and premature convergence avoidance
- Single- and multi-variable function optimisation

**Libraries:** `numpy`, `matplotlib`, optionally `deap` or `pygad`

---

### 🔷 Lab 8 — Applied Genetic Algorithms (Network & Component Placement Optimisation)

**Goal:** Apply genetic algorithms to solve two real-world engineering optimisation problems: minimising backbone traffic in a branched computing network, and optimal placement of electronic components on a mounting field.

**Topics covered:**

*Network topology optimisation:*
- Backbone (ring topology) traffic modelling
- Chromosome encoding for host-to-concentrator assignment
- Fitness function based on total backbone traffic load
- Elite selection, crossover at gene boundaries, modular mutation

*PCB component placement optimisation:*
- Placement problem formulation: minimise total wire length + area overlap penalty
- Chromosome as a list of (x, y) coordinate pairs
- Overlap penalty function and connection length normalisation
- Mobile GA, evolutionary strategies: mutation-only, recombination (m, k)
- Convergence analysis across different packing densities

**Libraries:** `numpy`, `matplotlib`, optionally `deap`, `scipy`

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python 3.x** | Primary programming language across all labs |
| **scikit-fuzzy** | Fuzzy membership functions, FCM clustering, fuzzy inference |
| **NumPy** | Numerical computation, matrix operations |
| **Matplotlib / mpl_toolkits** | 2D/3D visualisation of functions, surfaces, and results |
| **TensorFlow / Keras** or **PyTorch** | Neural network construction and training (Labs 4, 5) |
| **Pandas** | Data handling for time-series tasks (Lab 6) |
| **DEAP / PyGAD** | Genetic algorithm framework (Labs 7, 8) |
| **Jupyter Notebook** | Interactive exploration and result presentation |

---

## 🎯 Learning Outcomes

Upon completing these laboratories, the student is able to:

- ✅ Design and implement fuzzy inference systems (Mamdani, TSK) from scratch
- ✅ Apply fuzzy C-means clustering to real datasets and interpret membership degrees
- ✅ Build, train, and evaluate feedforward neural networks for function approximation
- ✅ Understand and implement Hebbian unsupervised learning
- ✅ Construct neuro-fuzzy hybrid models combining the interpretability of fuzzy rules with the adaptability of neural networks
- ✅ Design genetic algorithms with appropriate encoding, operators, and fitness functions for custom optimisation problems
- ✅ Analyse convergence behaviour and tune GA hyperparameters for practical engineering tasks

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/YuHryshchenko/zpi-zp41_AI_Methods-Technologies_HryshchenkoYuliia_KPI_2026.git
cd zpi-zp41_AI_Methods-Technologies_HryshchenkoYuliia_KPI_2026

# Install dependencies
pip install numpy matplotlib scikit-fuzzy pandas tensorflow deap jupyter

# Launch Jupyter
jupyter notebook
```

---

## 📚 References

- Shimkovich V.M. *Methods and technologies of piece intelligence: laboratory workshop.* KPI im. Igor Sikorsky, 2025.
- Zadeh, L.A. — Fuzzy Sets (1965)
- Haykin, S. — *Neural Networks and Learning Machines* (3rd ed.)
- Holland, J.H. — *Adaptation in Natural and Artificial Systems* (1975)

---

*Faculty of Informatics and Computer Engineering · KPI Igor Sikorsky · Kyiv, Ukraine*
