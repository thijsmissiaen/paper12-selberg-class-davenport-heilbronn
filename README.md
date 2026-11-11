# Hecke Theta-Integral Kernels and Single-Mode Damping in General Degree $L$-Functions versus Off-Line Zero Diagnostics in the Davenport–Heilbronn Counterexample

**DOI (Zenodo / CERN):** [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24141091.svg)](https://doi.org/10.5281/zenodo.24141091) [`10.5281/zenodo.24141091`](https://doi.org/10.5281/zenodo.24141091) (v12.1.0: [`10.5281/zenodo.24141092`](https://doi.org/10.5281/zenodo.24141092))  
**Author:** Thijs Missiaen (Independent Researcher, Belgium · ORCID: [0009-0007-3678-0810](https://orcid.org/0009-0007-3678-0810))  
**Series:** Transverse Wronskian & Phase-Space Analysis of Riemann's $\Xi$-Function (Paper XII)  
**MSC 2020:** Primary 11M41, 11M26; Secondary 11F66, 30D15, 46E22

---

## Overview

In Section 10.25 of *The Theory of the Riemann Zeta-Function*, E. C. Titchmarsh highlights the classical litmus test of Davenport and Heilbronn (1936): the self-dual linear combination of Dirichlet $L$-functions modulo $5$,

$$
\mathcal{D}_{\mathrm{DH}}(s) := \frac{1 - \mathrm{i}\kappa}{2} L(s,\chi_5) + \frac{1 + \mathrm{i}\kappa}{2} L(s,\overline{\chi_5}), \qquad \kappa := \frac{\sqrt{10 - 2\sqrt{5}} - 2}{\sqrt{5} - 1} \approx 0.28407904,
$$

whose completed entire function $\Xi _ {\mathrm{DH}}(z)$ satisfies $\Xi _ {\mathrm{DH}}(z) = \Xi _ {\mathrm{DH}}(-z) = \overline{\Xi _ {\mathrm{DH}}(\bar{z})}$ yet has no Euler product and possesses infinitely many off-line zeros inside the critical strip, beginning at $(d _ {\ast},\gamma _ {\ast}) \approx (0.30851718, 85.69934849)$.

This paper separates identities that depend solely on the Archimedean functional equation from arithmetic multiplicativity defects and complex-analytic zero-detection contrapositives:

### 1. Hecke Theta-Integral Dilation and Tetragamma Branch Damping (Section 2)

Records Hecke's Mellin–theta dilation $\varphi _ m^{(f)}(u) = a _ f(m)m^{-1/2}\varphi _ 1^{(f)}(u + \frac{1}{2}\ln m)$ and proves that in the high-frequency regime $\lvert\tau _ j^\pm\rvert > \sigma _ j^\pm + 1$, tetragamma positivity ($\mathrm{Re} \psi _ 2 > 0$) enforces $\rho _ {\Gamma,f}(d,t)n^{2d} < \mathrm{e}^{-2d\omega _ n(t)} \le 1$ across $\zeta(s)$ ($d _ \zeta = 1$), Ramanujan's $L(s,\Delta)$ ($d _ \Delta = 2$), and $\mathcal{D} _ {\mathrm{DH}}(s)$ ($d _ {\mathrm{DH}} = 1$).

### 2. Single-Mode Hyperbolic Identity (Section 3)

Elementary trigonometric-hyperbolic cancellation gives

$$
\lvert T_n^{(f)}(d,t)\rvert^2 - \lvert T_n^{(f)}(0,t)\rvert^2 = 4 \frac{\lvert a_f(n)\rvert^2}{n} \sinh^2\bigl(d \omega_n(t)\bigr) \ge 0
$$

for every Dirichlet series, demonstrating explicitly why single-mode damping and diagonal Wronskian positivity hold even at $(d _ {\ast},\gamma _ {\ast})$ and cannot by themselves prevent off-line zeros.

### 3. Multiplicativity Defects and Complete 8-Mode + Remainder Balance (Section 4)

On $\mathrm{Re}(s) > 1$, Euler-product mollification $L(s,f)E _ X^{(f)}(s)$ clears composite indices $2 \le N \le X$, whereas $\mathcal{D} _ {\mathrm{DH}}(s)$ exhibits exact multiplicativity defects $\delta _ {\mathrm{DH}}(m,n) = \pm(1 + \kappa^2) \approx \pm 1.08070090$ at $N \in \lbrace 4,6,9,14\rbrace$. While $\zeta(s)$ and $\mathcal{D} _ {\mathrm{DH}}(s)$ both have $\lvert a(4)\rvert = \lvert a(6)\rvert = 1$, $\mathcal{D} _ {\mathrm{DH}}(s)$ has suppressed prime coefficients $\lvert a _ {\mathrm{DH}}(2)\rvert = \lvert a _ {\mathrm{DH}}(3)\rvert = \kappa$, amplifying $\lvert a _ {\mathrm{DH}}(4)\rvert/\kappa^2 \approx 12.39143$ relative to multiplicative scaling. At $(d _ {\ast},\gamma _ {\ast})$ with $N _ 5(\gamma _ {\ast}) = 8$, primes $p \in \lbrace 2,3,5,7\rbrace$ supply 38.81780% of $\lvert T _ 1\rvert$, composites $n \in \lbrace 4,6,8\rbrace$ supply 54.02700%, and the Riemann–Siegel remainder $\mathcal{R} _ 8$ supplies the remaining 7.25126% residual closing $T _ {1..8} + \mathcal{R} _ 8 = 0$.

### 4. Four-Layer Zero-Detection Contrapositives (Section 5)

Verifies around $(d _ {\ast},\gamma _ {\ast})$ four classical zero-detection diagnostics: (i) critical-line Laguerre defect $c _ 1^{\mathrm{DH}}(z _ {\mathrm{c}}) < 0$ at $z _ {\mathrm{c}} \approx 85.74720083$ with reversed nodal-wall derivative $\mathrm{d}\lvert R _ {\mathrm{DH}}\rvert/\mathrm{d}s < 0$; (ii) negative reduced Wronskian $\widetilde{W} _ {\mathrm{DH}}(d,\gamma _ {\ast}) < 0$ on $[0,d _ {\ast}){}$; (iii) quantized Poisson–Hadamard step $\pi\Theta(d - d _ {\ast})$; and (iv) Pick–Nevanlinna Sylvester jump $\nu _ - : 0 \to 1$. Section 6 explains why these criteria detect rather than prevent off-line zeros.

---

## Repository Structure & Reproducibility

* [`paper/paper12_selberg_davenport_heilbronn.tex`](paper/paper12_selberg_davenport_heilbronn.tex) – AMS-LaTeX manuscript.
* [`paper/paper12_selberg_davenport_heilbronn.pdf`](paper/paper12_selberg_davenport_heilbronn.pdf) – Compiled PDF (12 pages, AMS-LaTeX / pdfTeX).
* [`scripts/verify_paper12_selberg_davenport_heilbronn.py`](scripts/verify_paper12_selberg_davenport_heilbronn.py) – 60-decimal `mpmath` + 35-decimal `mpmath.iv` interval verification and figure generation script.
* [`figures/`](figures/) – Vector PDF and 300-DPI PNG figures (`fig1_davenport_heilbronn_chladni_bifurcation`, `fig2_prime_gauge_purity_vs_hadamard_flux`).
* [`.agents/skills/selberg-class-davenport-heilbronn/SKILL.md`](.agents/skills/selberg-class-davenport-heilbronn/SKILL.md) – Self-contained mathematical knowledge skill.

```bash
python scripts/verify_paper12_selberg_davenport_heilbronn.py
```
