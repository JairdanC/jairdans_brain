---
tags:
  - nonlinear_eqs
  - diff_eqs
  - bifurcations
  - taylor_series
  - normal_forms
date: 2026-07-31
---

---
status: #complete 
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

# Transcritical Bifurcation

Normal form: $\dot{x} = rx - x^2$
This is for a fixed point which always must exist but may change stability depending on parameters (e.g., $x^* = 0$ for the logistic equation).
* $r < 0$: Stable fixed point at origin, unstable at $x=r$.
* $r = 0$: Half-stable fixed point at origin.
* $r > 0$: Unstable fixed point at origin, stable at $x=r$.
**Transcritical Bifurcation Diagram:** An exchange of stabilities occurs at the origin. The lines $x=0$ and $x=r$ intersect at $r=0$. $x=0$ is stable for $r<0$ and unstable for $r>0$. $x=r$ is unstable for $r<0$ and stable for $r>0$.

![[Pasted image 20260731121522.png]]

**Example 3.2.1:** Show $\dot{x} = x(1 - x^2) - a(1 - e^{-bx})$ undergoes a transcritical bifurcation at $x=0$ when $(a,b)$ satisfy an equation. This is a bifurcation curve in $(a,b)$ space.
Use the Taylor series to approximate near $x=0$:
$\dot{x} = x(1 - x^2) - a(1 - (1 - bx + \frac{b^2 x^2}{2!} - \frac{b^3 x^3}{3!} + \frac{b^4 x^4}{4!} - \dots))$
$\dot{x} = x - x^3 - a(bx - \frac{b^2 x^2}{2} + \frac{b^3 x^3}{6} - \frac{b^4 x^4}{24} + \dots)$
$\dot{x} = x - abx + a\frac{b^2 x^2}{2} - a\frac{b^3 x^3}{6} + a\frac{b^4 x^4}{24} - \dots - x^3$
$\dot{x} = (1 - ab)x + \left(\frac{1}{2}ab^2\right)x^2 + \mathcal{O}(x^3)$
We can approximate $\mathcal{O}(x^3)$ as negligible:
$\dot{x} \approx (1 - ab)x + \left(\frac{1}{2}ab^2\right)x^2$
Finding fixed points ($\dot{x} = 0$):
$0 = (1 - ab)x^* + \left(\frac{1}{2}ab^2\right)x^{*2}$
$0 = x^*\left(1 - ab + \frac{1}{2}ab^2 x^*\right)$

---
Directly Related Subjects

- 


