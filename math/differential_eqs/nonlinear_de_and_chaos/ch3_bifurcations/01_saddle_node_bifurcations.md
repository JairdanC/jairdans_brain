---
tags:
  - bifurcations
  - diff_eqs
  - nonlinear_eqs
  - taylor_series
  - normal_forms
date: 2026-07-31
---

---
status: #complete 
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

# Intro to Bifurcations

**Bifurcation:** Bifurcations are qualitative changes in the dynamics of a system based on variance of the parameters. Where these happen are bifurcation points. Control parameters affect dynamical variables.

For the normal form: 
$\dot{x} = r + x^2$
* $r < 0$: Vector field contains two fixed points (one stable, one unstable).
* $r = 0$: Vector field contains one half-stable fixed point (saddle-node).
* $r > 0$: Vector field contains no fixed points.
A bifurcation occurs at $r = 0$ since the gradients are fundamentally different before and after.

This is a **Saddle Node Bifurcation**

![[Pasted image 20260731121323.png]]

**Bifurcation Diagram**
When plotted on a bifurcation diagram (typically $x$ vs $r$, since $x$ is dependent), the curve is a parabola opening to the left ($r = -x^2$).
* The solid line (upper branch) indicates the location of the stable fixed point.
* The dotted line (lower branch) indicates the location of the unstable fixed point.

# Normal Forms
The forms $\dot{x} = r \pm x^2$ are prototypical for saddle-node bifurcations. With a Taylor series approximation, we can find similar forms for all saddle-node bifurcations.
General formulation (Taylor expansion of $f(x,r)$ around the bifurcation point $(x^*, r_c)$):
$\dot{x} = f(x,r) = f(x^*, r_c) + (x - x^*)\frac{\partial f}{\partial x}\bigg|_{(x^*, r_c)} + (r - r_c)\frac{\partial f}{\partial r}\bigg|_{(x^*, r_c)} + \frac{1}{2}(x - x^*)^2 \frac{\partial^2 f}{\partial x^2}\bigg|_{(x^*, r_c)} + \dots$

**Example 3.1.2:** Show $\dot{x} = r - x - e^{-x}$ undergoes a saddle-node bifurcation as $r$ is varied.
Fixed points occur at $\dot{x} = 0$:
$r = x + e^{-x}$
Using a Taylor series approximation (near the stable point):
$\dot{x} = r - x - e^{-x}$
$\dot{x} = r - x - \left[1 - x + \frac{x^2}{2!} - \dots\right]$
$\dot{x} \approx r - 1 - \frac{x^2}{2!}$
This yields a parabolic approximation where the curve shifts up and down as $r$ crosses the critical value $r_c = 1$.

- AI transcription of physical notes

---
Directly Related Subjects

- 


