# Discrete Mathematics - Assignment 3
## 1
### Description
**Let $f : \mathbb{Z} \rightarrow \mathbb{Z}$ be defined as $f(n) = 2 n - 5$ for all integers $n$.**

*Note: To justify your answers in (b) and (c), if the answer is positive you need to provide a proof, and if it is negative, give a counterexample.*

#### a) **List three elements that are in the range of $f$**

#### b) **Is $f$ one-to-one? Justify your answer**

#### c) **Is $f$ onto? Justify your answer**

#### d) **Write an explicit formula for the composition $f \circ f$**

## 2
### Description
**Let $a_k = 2 k - 5$ and $b_k = 2 - k$.**

**Simplify each expression to only use a single summation ($\Sigma$) or product ($\Pi$) using the properties of summations and products listed below. List intermediate steps.**

$\begin{aligned} \sum_{k=m}^{n} a_k - 3 \cdot \sum_{k=m}^{n} b_k \end{aligned} $

$\begin{aligned} \prod_{k=m}^{n} a_k  \cdot \prod_{k=m}^n b_k \end{aligned} $

---
Theorem 5.1.1
If $a_m, a_{m+1}, a_{m+2}, \ldots$ and $b_m, b_{m+1}, b_{m+2}, \ldots$ are sequences of real numbers and $c$ is any real number, then the following equations hold for any integer $n \geq m$ :
1. $\begin{aligned} \sum_{k=m}^n a_k+\sum_{k=m}^n b_k=\sum_{k=m}^n\left(a_k+b_k\right) \end{aligned}$
2. $\begin{aligned} c \cdot \sum_{k=m}^n a_k=\sum_{k=m}^n c \cdot a_k \quad \end{aligned}$ (generalized distributive law)
3. $\begin{aligned} \left(\prod_{k=m}^n a_k\right) \cdot\left(\prod_{k=m}^n b_k\right)=\prod_{k=m}^n\left(a_k \cdot b_k\right) \end{aligned}$.

---
*For instance, given sequences $a_k = k$ and $b_k = 2 k + 1$, simplifying an expression $\begin{aligned} \sum_{k=m}^{n} a_k + 2\cdot \sum_{k=m}^{n} b_k \end{aligned}$ could be done in the following way:*

$\begin{aligned} \sum_{k=m}^n a_k+2 \cdot \sum_{k=m}^n b_k &=\sum_{k=m}^n k+2 \cdot \sum_{k=m}^n(2 k+1) --- by (substitution) \\
&=\sum_{k=m}^n k+\sum_{k=m}^n 2 \cdot(2 k+1) --- by(2) \\
&=\sum_{k=m}^n k+\sum_{k=m}^n(4 k+2) --- by(algebraic simplification) \\
&=\sum_{k=m}^n(k+(4 k+2)) --- by (1) \\
&=\sum_{k=m}^n(5 k+2) --- by (algebraic simplification)\end{aligned}\\$

## 3
### Description
**Prove, using mathematical induction, that $3$ divides $n^3 + 5n - 6$ for all integers $n\geq 0$.**

*Hint: You can use the fact that given $a \,| b$ and $a \,| c$, we can conclude $a \,| (b + c)$ for all integers $a,b,c$. Moreover, you can use the binomial theorem for exponent $3$, which states that $(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3$ for all real numbers $a, b$.*