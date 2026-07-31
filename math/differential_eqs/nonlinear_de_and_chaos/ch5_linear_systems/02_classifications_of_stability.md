---
tags:
  - diff_eqs
  - lin_alg
  - linear_systems
  - nonlinear_eqs
date: 2026-07-24
---

---
status: #complete
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

To evaluate the stability and phase portrait of a linear system, we look for solutions along eigenvectors $\textbf{v}$ satisfying:
$$A \textbf{v} = \lambda \textbf{v}$$
To find the eigenvalues $\lambda$, we solve the characteristic equation, which yields:
$$\lambda = \frac{\tau \pm \sqrt{\tau^2 - 4\Delta}}{2}$$
*(where $\tau$ is the trace and $\Delta$ is the determinant of matrix $A$)
### Classification of Fixed Points ($\textbf{x} \in \mathbb{R}^2$)

Depending on the values of $\tau$ and $\Delta$, the phase portrait is classified into the following distinct regimes:

 **Case 1: Saddle Points**

* **Condition:** Negative determinant ($\Delta < 0$). This guarantees that only one of the eigenvalues ($\lambda$) is negative, meaning the eigenvalues are real, distinct, and opposite in sign.

* **Dynamics:** Because the eigenvalues are distinct, the eigenvectors ($\textbf{v}$) are linearly independent. The general solution is a linear superposition of the two solutions found from the eigenvalues.

* **Phase Portrait:** Looks like a crossing through the fixed point, with nearby trajectories asymptote alongside the stable and unstable points.

**Case 2: Attracting and Repelling Points**

**Condition:** Positive determinant ($\Delta > 0$). The trace determines stability: attracting if $\tau < 0$, and repelling if $\tau > 0$.

**Case 2A: Nodes**

* **Math:** Real $\lambda$, same sign, distinct. The eigenvectors ($\textbf{v}$) are linearly independent.

* **Phase Portrait:** For the attractive case, arrows point directly towards the fixed point along the primary eigenspace.
  
**Case 2B: Spirals**

* **Math:** Complex $\lambda$ (such that $\lambda = \mu \pm i\omega$). Because the eigenvalues are complex, there are no real eigenvectors. Each component of $\textbf{x}$ is a linear combination of $e^{\mu t}\cos(\omega t)$ and $e^{\mu t}\sin(\omega t)$.

* **Phase Portrait:** $\mu$ controls the radial decay rate (stable rotates in, unstable rotates out), and $\omega$ controls the rotation rate. To easily determine the direction of rotation, simply calculate the vector field at one test coordinate on the axis.

**Case 3: Centers**

* **Condition:** $\Delta > 0$ and $\tau = 0$.

* **Math:** Purely imaginary eigenvalues ($\lambda = \pm i\omega$).

* **Phase Portrait:** No exponential growth or decay. All trajectories form completely closed orbits around the fixed point.

**Case 4: Degenerate Nodes (The Textbook Borderline)**

* **Condition:** $\tau^2 - 4\Delta = 0$.

* **Phase Portrait:** Repeated real eigenvalues. The system either forms a "star node" (if two independent eigenvectors exist) or a skewed degenerate node (if only one eigenvector exists).


---
Directly Related Subjects

- 


