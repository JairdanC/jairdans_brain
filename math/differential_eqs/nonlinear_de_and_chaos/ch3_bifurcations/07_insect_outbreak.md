---
tags:
  - example
  - nonlinear_eqs
  - diff_eqs
  - population_dynamics
  - dimensionless_analysis
date: 2026-07-31
---

---
status: #complete 
class backlink: [[nonlinear_differential_equations_and_chaos_strogatz]]

# Insect Outbreak
Looking at spruce budworm dynamics where the population timescale of budworms $\gg$ forest growth, so the forest can be held constant or slowly drift (more complex).
$\dot{N} = RN\left(1 - \frac{N}{K}\right) - p(N)$
* $N(t)$: budworm population
* $R$: growth rate
* $K$: carrying capacity
* $p(N)$: predation rate $\implies p(N) = \frac{BN^2}{A^2 + N^2}$ (S-shaped curve approaching asymptote $B$, with inflection around $A$).

### Dimensionless Formulation
Use dimensionless analysis to better characterize our "outbreak" on a low $\to$ high jump.
Hint, from author's trial and error: push the variables out from the predation function and into the logistic part.
Dimensions:
* $N, K, A$: bud # (population)
* $R$: $t^{-1}$ (time inverse)
* $B$: bud increase per $t$ (is negative $\to$ predation)
Let $\frac{N}{A} = 1$ and $\frac{N}{K} = 1$. The hint says push out of predation function $\therefore x = \frac{N}{A}$.
$Ax = N \implies \frac{dx}{dt} = \frac{dN}{dt}\frac{dx}{dN} = \dot{N}\frac{1}{A}$
$\frac{d}{dt}(x) = \frac{d}{dt}\left(\frac{N}{A}\right) = \frac{\dot{N}}{A}$
$Ax = N \implies \dot{N} = A\dot{x}$
Substitute into the original equation:
$A\dot{x} = RAx\left(1 - \frac{Ax}{K}\right) - \frac{B(Ax)^2}{A^2 + (Ax)^2}$
$A\dot{x} = RAx\left(1 - \frac{A}{K}x\right) - B\left(\frac{x^2}{1+x^2}\right)$
Divide by $B$:
$\frac{A}{B}\dot{x} = \frac{RA}{B} \left(1 - \frac{A}{K}x\right) - \frac{x^2}{1+x^2}$
This eq still has dimensions in the logistic part of the eq so we create a dimensionless carrying capacity and growth rate 
$r = \frac{RA}{B} \quad k = \frac{K}{A}$ 
$\frac{A}{B}\dot{x} = rx\left(1 - \frac{x}{k}\right) - \frac{x^2}{1+x^2}$ $\to$ finally introduce a dimensionless time $\tau = \frac{B}{A}t \implies \frac{dx}{dt} = \frac{dx}{d\tau}\frac{d\tau}{dt} = \frac{dx}{d\tau}\frac{B}{A}$ $\frac{dx}{d\tau} = rx\left(1 - \frac{x}{k}\right) - \frac{x^2}{1+x^2} \checkmark$
Fixed points at $\underbrace{r\left(1 - \frac{x}{k}\right)}_{\text{linear}} = \underbrace{\frac{x}{1+x^2}}_{\text{curve}}$ 1, 2, or 3 intersections depending on $r$ & $k$ * 
![[Pasted image 20260731125919.png]]![[Pasted image 20260731125940.png]]
$a: \text{refuge}$ * $b: \text{threshold}$ * $c: \text{outbreak}$ 
- if (a) disappears from parameter change then jump to b (unstable) $\to$ outbreak 

### Bifurcation Curves Parameterize $r$ and $k$ in parameter space
$(r,k) \to (r(x), k(x))$
$\frac{d}{dx}\left[r\left(1 - \frac{x}{k}\right)\right] = \frac{d}{dx}\left[\frac{x}{1+x^2}\right]$
$-\frac{r}{k} = \frac{1-x^2}{(1+x^2)^2}$
$r = \frac{2x^3}{(1+x^2)^2} ; \quad k = \frac{2x^3}{x^2-1}$ 
![[Pasted image 20260731130000.png]]
![[Pasted image 20260731130019.png]]

**Comparison to Reality** 
Involves even more interesting variables and systems including
- Tree dynamics 
- Distribution
- Foliage 

---
Directly Related Subjects

- 