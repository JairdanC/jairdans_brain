---
tags:
  - diff_eqs
  - nonlinear_eqs
  - bifurcations
  - example
  - fbd
  - symmetry
  - dynamics
  - classical_mech
  - dimensionless_analysis
date: 2026-07-31
---

---
status: #complete 
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

# Overdamped Bead on a Hoop

Key analysis steps:
* FBD Analysis
* Symmetry
* Linear Stability Analysis
* How the stable points are found
* Dimensional Analysis and groups

**FBD Analysis:**
$mr\ddot{\phi} = -br\dot{\phi} - mg\sin\phi + mr\omega^2\sin\phi\cos\phi$
Neglect $\ddot{\phi}$ (overdamped limit) and find regime later:
$br\dot{\phi} = -mg\sin\phi + mr\omega^2\sin\phi\cos\phi$
$br\dot{\phi} = mg\sin\phi\left(\frac{r\omega^2}{g}\cos\phi - 1\right)$
Fixed points: $\phi^* = 0, \pi \land \text{if } \frac{r\omega^2}{g} > 1 \text{ then } \phi^* = \pm \cos^{-1}\left(\frac{g}{r\omega^2}\right)$


**Symmetry broken solutions:** Solution $<$ governing equation symmetry, the solution has less symmetry than the governing equation.

Pitchfork Bifurcation can be expected with symmetrical conditions.

**Dimensional Analysis:** 
$\tau := \frac{t}{T} ; T$ is characteristic time scale and
$\hookrightarrow \dot{\phi} = \frac{d\phi}{dt} = \frac{d\phi}{d\tau}\frac{d\tau}{dt} = \frac{1}{T}\frac{d\phi}{d\tau}$ 
$\hookrightarrow \ddot{\phi} = \frac{d^2\phi}{dt^2} = \frac{d^2\phi}{d\tau^2}\frac{d\tau^2}{dt^2} = \frac{d^2\phi}{d\tau^2}\left(\frac{d\tau}{dt}\right)^2 = \frac{1}{T^2}\frac{d^2\phi}{d\tau^2}$ 
(governing eq) $\frac{mr}{T^2}\frac{d^2\phi}{d\tau^2} = -\frac{br}{T}\frac{d\phi}{d\tau} - mg\sin\phi + mr\omega^2\sin\phi\cos\phi$
$\hookrightarrow$ turn to dimensionless groups
$\hookrightarrow \epsilon\frac{d^2\phi}{d\tau^2} = -\frac{d\phi}{d\tau} - \sin\phi + \gamma\sin\phi\cos\phi \quad \epsilon \to 0$ (6) 

**Singular Limit**: When investigating some limit of interest such as limit of strong damping in this case. Higher orders drop out and IC/BCs can't be satisfied $\hookrightarrow$ Singular Perturbation Theory

**Phase Plane Analysis Intro:**
Let $\Omega = \dot{\phi} = \frac{d\phi}{d\tau}$
The equation becomes $\epsilon \Omega' = f(\phi) - \Omega$ and $(\phi', \Omega')$ is the velocity of the "phase fluid" in phase space.
$\epsilon \to 0$ sets $\Omega'$ to $\pm\infty$ to the curve $f(\phi) = \Omega$ (fig 3.5.8 is good to illustrate).
*Consider: Transient phase and characteristic time scale, why?*
![[Pasted image 20260731124736.png]]

---
Directly Related Subjects
- [[04_pitchfork_bifurcation]]


