---
tags:
  - diff_eqs
  - linear_systems
  - lin_alg
  - nonlinear_eqs
date: 2026-07-24
---

---
status: #complete
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

**Def:** A two-dimensional linear system is a system of the form:
$$\dot{\textbf{x}} = A\textbf{x}$$
where:
$$A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}, \quad \textbf{x} = \begin{pmatrix} x \\ y \end{pmatrix}$$
**Example 5.1.1: Simple Harmonic Oscillator (Energy Conservation)**
This is an excellent example of extracting physical laws purely from geometric phase space. Starting with $m\ddot{x} + kx = 0$, we can define the system as:
$$\dot{x} = v$$
$$\dot{v} = -\omega^2 x$$
*(where $\omega^2 = k/m$)*
By establishing the orbital equations in the phase plane, we can geometrically derive the conservation of energy:

$$\frac{dx}{dv} = \frac{\dot{x}}{\dot{v}} = \frac{v}{-\omega^2 x}$$
$$-\omega^2 x \, dx = v \, dv$$
Integrating both sides:
$$\int -\omega^2 x \, dx = \int v \, dv$$$$\frac{-\omega^2}{2}x^2 = \frac{v^2}{2} + C_1$$
Because $C_1$ is an arbitrary constant, we can manipulate the equation (and substitute $k/m$ back in for $\omega^2$) to retrieve the classic sum of potential and kinetic energy:
$$\frac{1}{2}kx^2 + \frac{1}{2}mv^2 = C$$

---
Directly Related Subjects

- 





