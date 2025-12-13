# applied-statistics
Assessment repository

# Applied Statistics — Assessment Repository

This repository contains solutions to a set of applied statistics problems, implemented primarily using Python and Jupyter Notebooks. 

Each problem directory contains code, explanations, and visualizations that answer specific statistical questions as part of the assessment the applied statistics course.

---

## 📁 Repository Structure

The repository is organized into the following folders:

- **Problem_1** — First statistical task (likely introductory simulation or basic inference)
- **Problem_2** — Second task involving hypothesis testing or simulation
- **Problem_3** — t-Test simulations and type II error analysis
- **Problem_4** — ANOVA and multiple comparison methods  
- **.gitignore** — Git ignore configuration
- **README.md** — This file

---

## 🧪 Problem Descriptions

### 📌 Problem 1 : Extending the Lady Tasting Tea
In this problem I explore basic probability or inference tasks (e.g., simulations related to statistical distributions, confidence intervals, or random sampling). With the code I demonstrate how to use NumPy and standard Python tools to perform simulations and summarize results.

---

### 📌 Problem 2: Normal Distribution  
In the second problem I have built inferential techniques such as hypothesis testing, confidence sets, or permutation testing. I have used methods such as Python’s `scipy.stats` module to implement exact tests and draw conclusions from simulated or real data.

---

### 📌 Problem 3 — **t-Tests and Type II Error Simulation**

In this problem, I investigate the behavior of **independent samples t-tests** in relation to effect size:

- I generate pairs of normal samples with increasing mean differences \(d = 0, 0.1, 0.2, ..., 1.0\) and sample size \(n = 100\).
- For each value of \(d\), we simulate 1,000 trials where we:
  - Draw two samples
  - Perform a two-sample t-test
  - Evaluate rejection at \(\alpha = 0.05\)
- I record the **proportion of non-rejections** (the estimated *type II error rate*) and plot it against the mean difference.

This demonstrates how **statistical power increases as effect size increases**, and how t-tests behave under different signal strengths.

---

### 📌 Problem 4 — **One-Way ANOVA and Pairwise t-Tests**

In this problem I use three independent samples with distinct means (e.g., 0, 0.5, 1) to compare:

1. A **one-way ANOVA** to test the global null hypothesis that all group means are equal.
2. Three **independent two-sample t-tests** to compare group pairs.

The solution:
- Performs the ANOVA using `scipy.stats.f_oneway`.
- Performs pairwise t-tests using `scipy.stats.ttest_ind`.
- Compares conclusions from the ANOVA and pairwise tests.
- Explains why **ANOVA is preferred** over running multiple unadjusted t-tests, due to issues like inflated Type I error with multiple comparisons.

---

## 📦 References

In this repository I used the following Python libraries:

- **NumPy** — for numerical computing and random sampling  
- **SciPy** — for statistical tests including t-tests and ANOVA  
- **Matplotlib** — for plotting and data visualization  
- **Jupyter Notebook** — for interactive execution and documentation

Specific functions referenced:
- `numpy.random.default_rng` — reproducible random sampling  
- `scipy.stats.ttest_ind` — two-sample independent t-test  
- `scipy.stats.f_oneway` — one-way ANOVA test  
- `matplotlib.pyplot` — plotting

---

## 📖 Additional Notes

This repository demonstrates good practice in statistical computing:
- **Reproducible simulations**
- **Clear hypothesis test interpretation**
- **Comparison of statistical methods**
- **Integration of code and explanation**


---

## 🧠 Acknowledgments

I have developed this work as part of the Applied Statistics coursework, with an emphasis on simulation, statistical hypothesis testing, and the practical application of statistical theory.

---

