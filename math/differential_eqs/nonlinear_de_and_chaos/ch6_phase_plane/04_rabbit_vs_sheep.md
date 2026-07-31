---
tags:
  - population_dynamics
  - diff_eqs
  - nonlinear_eqs
  - example
date: 2026-07-28
---

---
status: #complete 
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

### Lotka-Volterra Model of Competition

- Two species competing for the same food supply, which is limited
- All other factors (predators, seasons, other foods) are neglected

We can think about the qualitative behavior first
1. A species should grow to its carrying capacity in the absence of the other, modelled by logistic growth
2. There is some conflict or competition for food resources, the amount of conflict is proportional to the size of each population (more likely to encounter each other with large populations)

$$
\dot x = x (3 - x - 2y)
$$
$$
\dot y = y (2 - x - y)
$$
- where $x(t)$ is the population of rabbits and $y(t)$ is the population of sheep
- The coefficients are arbitrary

These equations are then solved using the Jacobian around the fixed points to find the phase portrait

$$
\mathbf{A} = \begin{pmatrix} \frac{ \partial \dot{x} }{ \partial x } & \frac{ \partial \dot{x} }{ \partial y } \\ \frac{ \partial \dot{x} }{ \partial y } & \frac{ \partial \dot{x} }{ \partial y } \end{pmatrix} = \begin{pmatrix}
3 - 2x -2y & -2x \\
-y & 2 -x -2y
\end{pmatrix}
$$
With the four fixed points of $(0, 0), (0,2) ,(3,0), (1,1)$ we obtain the phase portrait of 

![[Pasted image 20260728142607.png]]

**Stable Manifold**: The eigenvector of a staddle node which attracts towards it
**Basin of Attraction**: For some fixed point $\mathbf{x}*$ the set of initial conditions $x_{0}$ such that $x(t) \to \mathbf{x}* \text{ as } t \to \infty$ 
**Basin Boundary**: The boundary along which the set of initial conditions ends or is defined. **Separatrices** are the trajectories that comprise the stable manifold
- These are important as they partition the phase space into the regimes of qualitative behaviour which the system will follow in the long-term

---
Directly Related Subjects

- 


