---
title:  "Notes on Convex Analysis - Day 1"
date:   2021-06-25 14:00:00 -0400
categories: [Math, Optimization]
math: true
header-includes:
  - \usepackage{mathrsfs}
  - \usepackage{amsbsy}
---
# Interriors of  Convex Sets

We first define the *Euclidean distance* between two points $x$ and $y$ in $R^n$ :

$$
\begin{equation} \label{e-distance}
d(x, y) = |x - y| = <x - y, x - y> ^\frac{1}{2}
\end{equation}
$$

And naturally we denote by $B$ the *Euclidean unit ball* from $\eqref{e-distance}$

$$
\begin{equation} \label{e-ball}
B = \{x | |x| \le 1\} = \{x | d(x, 0) \le 1\}
\end{equation}
$$

For any set $C$ in $R^n$, the set of points $x$ whose distance from $C$ does not exceed $\epsilon$ (note there $x$ is not necesarrily in $C$) is called

$$
\begin{equation} 
C +  \epsilon B = \{x| \exists y \in C, d(x, y) \le \epsilon \}
\end{equation} = \cup \{y + \epsilon B | y \in C \}
$$

We can now define the *closure* (cl $C$) and *interior* (int $C$) of $C$

$$
\begin{equation} \label{closure}
\text{cl } C = \cap_{\forall \epsilon} \{C + \epsilon B | \epsilon  > 0\}
\end{equation}
$$

$$
\begin{equation} \label{interior}
\text{int } C = \{x | \exists \epsilon > 0, x + \epsilon B \subset C \}
\end{equation}
$$

The closure of $C$ may equivalently be defined as the union of $C$ and its boundary, and also as the intersection of all closed sets containing $C$.

Relative interior of $C$ is defined as the interior which results when $C$ is regarded as a subset of its affine hull aff $C$. It is often more useful when dealing with low-dimensional sets placed in higher-dimensional spaces.

$$
\begin{equation} \label{ri}
\text{ri } C = \{x \in \text{aff }C | \exists \epsilon > 0, (x + \epsilon B) \cap (\text{aff }C) \subset C \}
\end{equation}
$$

# Closures of Convex Functions


