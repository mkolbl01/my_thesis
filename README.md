# Master's Thesis Code Repository

This repository contains the codes, data, and results used in my Master's thesis titled Loop Reduction for Cosmological Correlators, which studies the one- and two-loop power spectrum of dark matter by means of IBP reduction.

The project is divided into two main parts:

* **1-loop calculations** (full pipeline with code, data, and results)
* **2-loop calculations** (standalone computation)

---

## Requirements

* Maple
* Wolfram Mathematica

---

## Running the 1-loop code

1. Open Maple

2. Set the working directory to the folder:

   ```
   my_thesis/one-loop
   ```

3. Run the main script titled:

   ```
   read "codes/momentum_evaluation.map":
   ```

### Important note

It is necessary to restart the Maple kernel before each run to ensure a clean environment.

---

## Running the 2-loop code

The 2-loop calculation is self-contained.

1. Set the working directory to:

   ```
   my_thesis/two-loop
   ```

2. Run the script directly (e.g.):

   ```
   read "IBP_solver_suncut.map":
   ```

---

## Results

* **1-loop results** are written to the `results/` folder inside `one-loop/`
* **2-loop results** includes the coefficients of the reduction of integral SC(1,0,2,0,2), found in the `coeffs10202.txt` file located in the `two-loop/` directory

---

## Structure

```
my_thesis/
├── one-loop/
│   ├── codes/
│   ├── data/
│   └── results/
│
├── two-loop/
│   └── ...
│
└── README.md
```

---

## Notes

This repository is intended to accompany the thesis and provide reproducibility of the results.
