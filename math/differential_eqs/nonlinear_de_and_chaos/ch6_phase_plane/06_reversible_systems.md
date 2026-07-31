---
tags:
  - nonlinear_eqs
  - reversibility
  - dynamics
  - diff_eqs
date: 2026-07-30
---

---
status: #complete 
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

# Time-Reversal Symmetry

**Time-Reversal Symmetry**: Their dynamics look the same whether time runs forward or backward. That is to say the governing equation of the system e.x. $m \ddot{x} =F(x)$ is invariant under the change of variables $t\rightarrow-t$, velocity is reversed but the governing equation is the same.

**Reversible System**: A reversible system is defined as any second-order system that is invariant under the change of variables $t\rightarrow-t$ and $y\to-y$  where the coordinates of the phase plane are $(x,y)$ and there derivates are in terms of $t$. For example the system:
$$
\dot{x} = f(x,y)
$$
$$
\dot{y} = g(x,y)
$$
- Where $f(x,-y) = -f(x,y)$ and $g(x,-y)=g(x,y)$

**Theorem 6.6.1**: Nonelinear centers for reversible systems, $\mathbf{x*=0}$ is a linear center for the continuously differentiable system:
$$
\dot{x}=f(x,y)
$$
$$
\dot{y}=g(x,y)
$$
and suppose that this system is reversible. Then sufficiently close to the origin all trajectories are closed curves.
- Notes from the text: Consider a trajectory that starts on the positive xaxis near the origin (Figure 6.6.2). Sufficiently near the origin, the flow swirls around the origin, thanks to the dominant influence of the linear center, and so the trajectory eventually intersects the negative x-axis. (This is the step where our proof lacks rigor, but the claim should seem plausible.) Now we use 182 Nonlinear Dynamics and Chaos Figure 6.6.2 reversibility. By reflecting the trajectory across the x-axis, and changing the sign of t, we obtain a twin trajectory with the same endpoints but with its arrow reversed (Figure 6.6.3). Figure 6.6.3 Together the two trajectories form a closed orbit, as desired. Hence all trajectories sufficiently close to the origin are closed

![[Pasted image 20260730200503.png]]


- Example 6.6.1 Shows the linearization of a system with a nonlinear center then using reversibility shows that it is such, also discusses **heteroclinic trajectories** which is when two saddle points are joined by a connection, these are much more common in reversible and conservative systems
- Example 6.6.2 Mentions a higher-order definition of reversibility which is defined as a mapping $R(x)$ which when applied to the phase plane twice will cause all points to stay invariant (like flipping over the x-axis twice)
- Example 6.6.3 Shows a reversible, but not conservative system by showing proving that the change of variables gives an invariant phase portrait when applied twice and that there exists an attracting fixed point, which cannot occur in a conservative system

---
Directly Related Subjects

- [[05_conservative_systems]] 


