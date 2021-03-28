---
title:  "Generalized funtions and normalizing flows"
date:   2021-03-28 14:00:00 -0400
categories: [Math, Algebra, Normalizing Flow]
math: true
header-includes:
  - \usepackage{mathrsfs}
  - \usepackage{amsbsy}
---

# Definition

**Generalized Function**

Let  \\(\varphi(x)\\)  be an *argument of the functional*, which is a function where $\forall x$, $\varphi(x) \in \mathscr{D}$. 

$\varphi(x)$ is *compact*, if it has a bounded *support*. The *support* of a function $\varphi(x)$ is written as $\text{supp}(\varphi)$,  $\text{supp}(\varphi) := \\{x \in \mathit{X} \mid \varphi(x) \ne 0 \\}$

$\varphi(x)$ is *smooth*, if it has derivatives of all orders.

Let $f(x)$ be the kernel of $\varphi(x)$.

We have the following *linear functional*:

$$T[\varphi(x)] = \int f(x) \varphi(x) dx$$

$T[\cdot]$ maps inputs from $\mathscr{D}$ to $\boldsymbol{R}$ (real numbers).

Any *linear functional* $T[\varphi]$, which is continuous on the set $\mathscr{D}$ of
*smooth compact functions*, is called a *generalized function*.

**Linearity of Generalized Function**

$\forall \varphi(x), \psi(x) \in \mathscr{D}$, $\forall \alpha, \beta \in \boldsymbol{R}$, we have:

$$T[\alpha \varphi(x) + \beta \psi(x)] = \alpha T[\varphi(x)] + \beta T[\psi(x)]$$