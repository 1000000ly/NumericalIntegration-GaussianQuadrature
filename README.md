# NumericalIntegration-GaussianQuadrature

This repository contains a symbolic and numerical implementation of n-point Gaussian quadrature using Legendre orthogonal polynomials, written in Maple. It presents a complete symbolic and numerical derivation of n-point Gaussian quadrature based on Legendre orthogonal polynomials, with full validation of recurrence, weights, and integration accuracy.


---

## Project Overview

The project focuses on deriving and implementing Gaussian quadrature rules from scratch. Using symbolic computation in Maple, Legendre polynomials were constructed via recurrence, and their properties were applied to compute integration nodes and weights.

Key objectives included:
- Deriving recurrence relations for Legendre polynomials
- Computing nodes by solving for the roots of Pₙ(x)
- Calculating weights using analytical formulas
- Verifying the accuracy and symmetry of the quadrature rule

---

## Files

| File                  | Description                                             |
|-----------------------|---------------------------------------------------------|
| `GaussianQuadrature.mw` | Maple worksheet with all derivations, code, and output |
| `Results.txt`          | Output for n = 3, 10, 15: nodes, weights, and validation |
| `README.md`            | This file                                               |

---

## Method Summary

The weights are computed using the identity:

$$
w_k = \frac{\hat{S}_n(t_k)}{P_n'(t_k)}
$$

where:

$$
\hat{S}_n(t) = \int_{-1}^{1} \frac{P_n(t) - P_n(x)}{t - x} \, dx
$$


These formulas are implemented symbolically in Maple and evaluated numerically for different values of \( n \).


These properties were verified for multiple values of 𝑛, confirming node symmetry and that the total weight sums to 2.

---

## How to Run

1. Open `GaussianQuadrature.mw` in Maple (tested with Maple 2023)
2. Run the worksheet step by step or as a whole
3. Modify the value of `n` to explore different degrees of quadrature

---

## 👤 Author

Claire Du
MSc Financial Mathematics  
University of Liverpool  
GitHub: [1000000ly](https://github.com/1000000ly)
For questions or collaboration, feel free to reach out via GitHub.
---

## License

This repository is licensed under the [MPL 2.0 License](LICENSE).







