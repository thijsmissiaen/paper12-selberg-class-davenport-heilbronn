---
name: selberg-class-davenport-heilbronn
description: Canonical formulas, verified numerical diagnostics, and scope boundaries for Paper XII on Hecke theta-integral kernels, single-mode hyperbolic identities, multiplicativity defects, and four-layer off-line zero detection in the Davenport-Heilbronn counterexample.
---

# Skill: Hecke Kernels vs. Davenport–Heilbronn Off-Line Zero Diagnostics (Paper XII)

## 1. Canonical Wronskian & Wigner Normalization

For $\Xi _ f(z) = 8 \int _ 0^\infty \Phi _ f(u)\cos(2zu)\,\mathrm{d}u$ with $\Xi _ f(t - \mathrm{i}d) = R _ f(d,t) + \mathrm{i}I _ f(d,t)$ ($d = \sigma - 1/2 \ge 0$), the canonical transverse Wronskian is:

$$W_f(d,t) := \frac{1}{2}\,\partial_d \lvert\Xi_f(t - \mathrm{i}d)\rvert^2 = R_f\,\partial_t I_f - I_f\,\partial_t R_f = 16 \int_0^\infty y\sinh(2dy)\,I_f(y,t)\,\mathrm{d}y,$$

where $I _ f(y,t) = 2\int _ 0^\infty \Phi _ f\left(\frac{y+r}{2}\right)\Phi _ f\left(\frac{y-r}{2}\right)\cos(2tr)\,\mathrm{d}r$ and $\widetilde{W} _ f(d,t) = W _ f(d,t)/d$.

## 2. Verified Mathematical Results

1. **Hecke Theta-Integral Dilation & Tetragamma Branch Damping (Theorem 2.1):**
   * By Mellin inversion (Hecke 1936), $\varphi _ m^{(f)}(u) = a _ f(m)m^{-1/2}\varphi _ 1^{(f)}(u + \frac{1}{2}\ln m)$.
   * In the high-frequency regime $\lambda _ j t > \lambda _ j(\frac{1}{2}+d) + \lvert\mathrm{Re}\,\mu _ j\rvert + 1$, the second transverse derivative of $\mathcal{A} _ {\Gamma,f}^{\mathrm{sym}}(u,t) = g'(u) + g'(-u)$ is governed by the **tetragamma** function $\mathrm{Re}\,\psi _ 2(w _ j^\pm) > 0$ (not $\psi _ 1$; note $\psi _ 2(\sigma) < 0$ at $t = 0$), yielding $\rho _ {\Gamma,f}(d,t)n^{2d} < \mathrm{e}^{-2d\omega _ n(t)} \le 1$ for $1 \le n \le N _ f(t)$.
2. **Single-Mode Hyperbolic Identity (Proposition 3.1):**

$$\lvert T_n^{(f)}(d,t)\rvert^2 - \lvert T_n^{(f)}(0,t)\rvert^2 = 4\,\frac{\lvert a_f(n)\rvert^2}{n}\,\sinh^2\bigl(d\,\omega_n(t)\bigr) \ge 0.$$

   * Holds identically for $\zeta(s)$, $L(s,\Delta)$, and $\mathcal{D} _ {\mathrm{DH}}(s)$ right at $(d _ *,\gamma _ *)$, proving that single-mode growth and diagonal Wronskian positivity never prevent off-line zeros.
3. **Multiplicativity Defect & Complete 8-Mode + Remainder Accounting (Theorem 4.1):**
   * Note that $\zeta(s)$ and $\mathcal{D} _ {\mathrm{DH}}(s)$ both have unit-modulus composite coefficients $\lvert a(4)\rvert = \lvert a(6)\rvert = 1$; the Euler product does **not** make composite coefficients small in $\zeta(s)$. Instead, $\mathcal{D} _ {\mathrm{DH}}(s)$ has small prime coefficients $\lvert a _ {\mathrm{DH}}(2)\rvert = \lvert a _ {\mathrm{DH}}(3)\rvert = \kappa \approx 0.28407904$ while violating multiplicativity by $\delta _ {\mathrm{DH}}(m,n) = \pm(1 + \kappa^2) \approx \pm 1.08070090$ at $N \in \{4,6,9,14\}$.
   * At $(d _ *,\gamma _ *) = (0.3085171825, 85.6993484854)$ with $N _ 5(\gamma _ *) = 8$:
     * $\lvert T _ 1\rvert = 2.39194369$;
     * Primes $p \in \{2,3,5,7\}$: $0.92849988$ (38.81780% of $\lvert T _ 1\rvert$);
     * Composites $n \in \{4,6,8\}$: $1.29229533$ (54.02700% of $\lvert T _ 1\rvert$);
     * Riemann–Siegel remainder $\lvert\mathcal{R} _ 8\rvert = \lvert T _ {1..8}\rvert = 0.17344609$ (7.25126% of $\lvert T _ 1\rvert$), closing $T _ {1..8} + \mathcal{R} _ 8 = 0$.
4. **Four-Layer Zero-Detection Diagnostics (Proposition 5.1):**
   * At $z _ {\mathrm{c}} = 85.7472008265$, $c _ 1^{\mathrm{DH}}(z _ {\mathrm{c}}) = -6.47422 \times 10^{-57} < 0$ and $\mathrm{d}\lvert R _ {\mathrm{DH}}\rvert/\mathrm{d}s < 0$ along $\Gamma _ {\mathrm{false}}$; $\widetilde{W} _ {\mathrm{DH}}(d,\gamma _ *) < 0$ on $[0,d _ *)$; $\Phi _ {\mathrm{Had}}(d;d _ *) = \pi\,\Theta(d - d _ *)$; Pick–Nevanlinna inertia $\nu _ - : 0 \to 1$.

## 3. Scope Boundaries & Anti-Overclaim Rules

* **Detection, not prevention:** The four diagnostics in Section 5 are contrapositives of classical RH equivalences (Hinkkanen 1997, Lagarias 1999, de Branges 1968, Arias de Reyna 2003); they detect off-line zeros of any real-even entire function and do not prove zero-freeness for Euler-product $L$-functions.
* **Domain of convergence:** Infinite Euler products and Dirichlet logarithms $\sum \Lambda _ f(n)/(n^s\ln n)$ converge absolutely only on $\mathrm{Re}(s) > 1$; only finite prime-factor Dirichlet polynomials $E _ X^{(f)}(s)$ extend holomorphically without poles.
