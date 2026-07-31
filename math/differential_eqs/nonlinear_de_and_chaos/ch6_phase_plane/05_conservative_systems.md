---
tags:
  - nonlinear_eqs
  - dynamics
  - diff_eqs
  - conservation_laws
date: 2026-07-28
---

---
status: #complete
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

### Conserved Quantities

Starting with the example $m\ddot{x} = F(x)$, Newton's Second Law, if $V(x)$ denotes the potential energy, defined by $F(x) = -\frac{dV}{dt}$ then 
$$
m\ddot{x} + \frac{dV}{dt} = 0
$$
- Trick: multiply both sides by $\dot{x}$ to det the exact time-derivate
$$
m\dot{x}\ddot{x} + \frac{d}{dt} V\dot{x} = 0 \rightarrow \frac{d}{dt} \left[ \frac{1}{2}m\dot{x} + V(x)  \right] = 0
$$
Then for a given solution of $x(t)$ the total energy is then equal to: 
$$
E = \frac{1}{2} m \dot{x}^2 + V(x)
$$
which is constant as a function of time. The energy is then a **conserved quantity**, and system for which a conserved quantity exists are **conservative systems.**

**Conserved Quantity:** Given a system $\dot{x} = \mathbf{f(x)}$, a conserved quantity is a real-valued and continuous function $E(\mathbf{x})$ that is constant on trajectories (meaning that $\frac{d}{dt} E(\mathbf{x}) = 0$), this function $E(\mathbf{x})$ must also be nonconstant on every open set, meaning $E(\mathbf{x}) = c$ wouldn't qualify. 

- Example 6.5.1 shows that conservative systems cannot have attracting fixed points

- Example 6.5.2 Shows how a center can arise in nonlinear systems despite the nonlinear terms (as discussed in [[03_fixed_points_and_linearization]]) by showing the conserved energy defines contours along which centers do arise. It also introduces **homoclinic orbits** which are orbits which start and end at the same point, these are rare outside of conservative systems

- Example 6.5.3 Shows the graph of $E(x,y)$ on the phase plane and how the surface creates the contours/trajectories on which the conserved system will stay, the local minima (stable) and maxima (unstable) being fixed points
---
 ![[Pasted image 20260728163512.png]]


### Nonlinear Centers

Centers are ordinarily very delicate, but as the examples above show, they become more robust when in a conservative system. This leads to the following Theorem

**Theorem 6.5.1**: Nonlinear centers for conservative systems, consider the system $\dot{x} = f(\mathbf{x})$ where $\mathbf{x} = (x,y) \in \mathbb{R}^2$ and $f$ is continuously differentiable. Suppose there exists some conserved quantity $E(\mathbf{x})$ and suppose that $\mathbf{x}*$ is an isolated fixed point. Then if $\mathbf{x}*$ is a local minimum of $E$, then all the trajectories sufficiently close to $\mathbf{x}*$ are closed.

- Note from the book: Since $E$ is constant on trajectories, each trajectory is contained in some contour of $E$. Near a local maximum or minimum, the contours are closed. The only remaining question is whether the trajectory actually goes all the way around the contour or whether it stops at a fixed point on the contour. But because we’re assuming that $\mathbf{x}*$ is an isolated fixed point, there cannot be any fixed points on contours sufficiently close to $\mathbf{x}*$. Hence all trajectories in a sufficiently small neighborhood of $\mathbf{x}*$ are closed orbits, and therefore $\mathbf{x}*$ is a center. 
	1. The theorem is valid for local maxima of $E$ also. Just replace the function E by $−E$, and maxima get converted to minima; then **Theorem 6.5.1** applies. 
	2. We need to assume that $\mathbf{x}*$ is isolated. Otherwise there are counterexamples due to fixed points on the energy contour—see Exercise 6.5.12.

---
Directly Related Subjects

- 


