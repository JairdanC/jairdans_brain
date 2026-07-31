---
tags:
  - diff_eqs
  - nonlinear_eqs
  - bifurcations
  - dynamics
  - normal_forms
date: 2026-07-31
---

---
status: #complete 
class backlink:[[nonlinear_differential_equations_and_chaos_strogatz]]

Common in physical problems with symmetry. Think of the buckling beam from 3.0; the beam could deflect to the left or the right.

# Supercritical Pitchfork Bifurcation
**Normal form:** $\dot{x} = rx - x^3$
The system is invariant under $x \to -x$ (spatial symmetry):
$-(-\dot{x}) = -r(-x) + (-x)^3 \implies -\dot{x} = -rx - x^3 \implies \dot{x} = rx + x^3$ (same)
$\therefore$ the vector field is equivariant.
* $r < 0$: Stable origin.
* $r = 0$: Critical slowing down, slower decay towards stability (see eq 2.4.9).
* $r > 0$: Unstable origin, stable at $x^* = \pm\sqrt{r}$.

- Exercise 3.6.7 Neural Nets $\dot{x} = -x - \beta\tanh(x)$ was cool
- Example 3.4.1). Finding the potential was a good example for physics where $V(x)$ is defined as for some system $\dot{x} = f(x) \implies f(x) = -\frac{dV}{dx}$ (Example 3.4.2)
### Subcritical Pitchfork Bifurcation
**Normal form:** $\dot{x} = rx + x^3$

The cubic term is destabilizing (pushing away when the supercritical is pulling and vice versa). Easy way to remember: sub $\to$ split converges as $r \to 0^-$ and super $\to$ split occurs and diverges as $r \to \infty$. $x^* = \pm\sqrt{-r}$ (non-zero fixed points).


In physical systems this "explosion instability" is damped by higher-order terms ($x^5$ if $x \to -x$ is invariant). 

**Canonical form with higher-order damping:** $\dot{x} = rx + x^3 - x^5$
This looks the same under small $x$ but allows for jumps and hysteresis as $r$ is varied. When $x^* = 0$ it is stable once $r<0$ and $x$ is nudged. $x^*=0$ is no longer stable and jumps to a large amplitude branch. This is hard to reverse since you have to move $r < r_s$ to get the point back to the origin. $r_s$ is a saddle-node bifurcation.

---
Directly Related Subjects

- 


