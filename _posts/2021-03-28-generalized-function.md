---
title:  "Generalized funtions and normalizing flows"
date:   2021-03-28 14:00:00 -0400
categories: [Math, Algebra, Normalizing Flow]
math: true
header-includes:
  - \usepackage{mathrsfs}
  - \usepackage{amsbsy}
---

# **Functional**

[Functional](https://mathworld.wolfram.com/Functional.html) refers to a mapping from a space $\mathit{X}$ (usually of functions) into $\boldsymbol{R}$ (real numbers). (Or complex numbers, in a more general case.) 

# **Generalized Function**

## Definition

Let  \\(\varphi(x)\\)  be an *argument of the function*, which is a function where $x \in \boldsymbol{R}$, and $\forall x$, $\varphi(x) \in \mathscr{D}$. 

 * $\varphi(x)$ is *smooth*, if it has derivatives of all orders.

 * $\varphi(x)$ is *compact*, if it has a bounded *support*. The *support* of a function $\varphi(x)$ is written as $\text{supp}(\varphi)$,  $\text{supp}(\varphi) := \\{x \in \mathit{X} \mid \varphi(x) \ne 0 \\}$. 

Let $f(x) := \boldsymbol{R} \rightarrow \boldsymbol{R}$ be the kernel of $\varphi(x)$.

We have the following [*linear functional*](https://mathworld.wolfram.com/LinearFunctional.html):

$$T[\varphi] = \int f(x) \varphi(x) dx$$

* $T[\cdot]$ is *continuous*, if for any sequence $\\{\varphi_k\\}_{k = 1, \cdots, \infty}$, when the sequence converges to $\varphi$ at $k \rightarrow \infty$, the corresponding sequence $\\{T[\varphi_k]\\}$ converges to $T[\varphi]$.

* $T[\cdot]$ maps inputs from $\mathscr{D}$ (function space) to $\boldsymbol{R}$.

 <span style="color: green"> Any *linear functional* $T[\varphi]$, which is *continuous* on the set $\mathscr{D}$ of
*smooth compact functions*, is called a *generalized function*. A *generalized function* is a *linear functional*, but not a *function*.  </span> 

## Linearity of Generalized Function

$\forall \varphi(x), \psi(x) \in \mathscr{D}$, $\forall a, b \in \boldsymbol{R}$, we have:

$$T[a\varphi + b\psi] = a T[\varphi] + b T[\psi]$$

## Regular Generalized Function

If the kernal $f(x)$ is an everywhere continuous, bounded function, $T[\varphi]$ is called a *regular generalized function* identified with the kernal $f(x)$.

### Singular Generalized Function

A *singular generlized function* $T[\varphi]$ is still linear continuous, but its kernel is not continuous. 

The most important example is the function:

$$T[\varphi] =  \varphi(0)$$

Though the kernel is not continuous, we still give it a symbol $\delta(x)$ and write it as:

$$T[\varphi] = \int \delta(x) \varphi(x) dx = \varphi(0)$$

Although the above thing is well known as the delta function, according to [Wikipedia](https://en.wikipedia.org/wiki/Dirac_delta_function) and [Wolfram](https://mathworld.wolfram.com/DeltaFunction.html), given different contexts, the delta function can refer to different things. As a distribution, the delta function is $T[\cdot]$, the linear functional, and is written as $\delta[\varphi] =  \varphi(0)$. As a measure, or in the engineering context, the kernel $\delta(x)$ in  $\int \delta(x) \varphi(x) dx$ is the delta function. A very confusing expression is:

$$\delta [\varphi] = \int \delta(x) \varphi(x) dx = \varphi(0)$$

If $\varphi(x) = 1$:

$$\delta [1] = \int \delta(x) dx = 1$$

One personal thought: would it be better to have:

$$\Delta [\varphi] = \int \delta(x) \varphi(x) dx = \varphi(0)$$



