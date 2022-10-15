# Discrete Mathematics - Assignment 3
## 1
### Description
**Let $f : \mathbb{Z} \rightarrow \mathbb{Z}$ be defined as $f(n) = 2 n - 5$ for all integers $n$.**

*Note: To justify your answers in (b) and (c), if the answer is positive you need to provide a proof, and if it is negative, give a counterexample.*

#### a) **List three elements that are in the range of $f$**
##### Solution
$$f(2)=2*2-5$$
$$=4-5$$
$$=-1$$

$$f(3)=2*3-5$$
$$=6-5$$
$$=1$$

$$f(4)=2*4-5$$
$$=8-5$$
$$=3$$


The elements -1, 1 and 3 are in the range of $f$ following that $f$ is a function from $\mathbb{Z}$ (the set of all integers) to $\mathbb{Z}$.

#### b) **Is $f$ one-to-one? Justify your answer**
##### Solution
If the function $f: \mathbb{Z} \rightarrow \mathbb{Z}$ is defined by the rule $f(n) = 2n - 5$ for each integer $n$, then $f$ is one-to-one.

**Proof:** 

Suppose $n_1$ and $n_2$ are integers such that $f(n_1) = f(n_2)$. 

By definition of $f$, we have $f(n_1) = 2n_1 - 5$ and $f(n_2) = 2n_2 - 5$.

Since $f(n_1) = f(n_2)$, we have $2n_1 - 5 = 2n_2 - 5$.

Simplifying (adding 5 to both sides), we have $2n_1 = 2n_2$.

Dividing both sides by 2, we have $n_1 = n_2$.

Therefore, $n_1$ and $n_2$ are equal, and $f$ is one-to-one. 

$\square$

---
**Definition of one-to-one:**

A function $f$ from a set $X$ to a set $Y$ is one-to-one (or injective) if, and only if, for all elements $x_1, x_2 \in X$
$$F(x_1) = F(x_2) \implies x_1 = x_2$$

Symbolically:
$F: X \rightarrow Y$ is one-to-one $\iff \forall x_1, x_2 \in X$, if $F(x_1) = F(x_2)$ then $x_1 = x_2$

---
#### c) **Is $f$ onto? Justify your answer**
##### Solution
If the function $f: \mathbb{Z} \rightarrow \mathbb{Z}$ is defined by the rule $f(n) = 2n - 5$ for each integer $n$, then $f$ is **not** onto.

**Counterexample:**

The co-domain of $n$ is $\mathbb{Z}$, and $0 \in \mathbb{Z}$.
But $f(n) \neq 0$ for any integer $n$.

For if $f(n) = 0$, then $2n - 5 = 0$, which implies $2n = 5$, which implies $n = 5/2$

But $5/2$ is not an integer. Hence there is no integer $n$ for which $f(n) = 0$, and thus $f$ is not onto.

$\square$

---
**Definition of onto:**

Let $F$ be a function from a set $X$ to a set $Y$. $F$ is onto (or surjective) if, and only if, given any element $y \in Y$, there exists an element $x \in X$ with the property $y = F(x)$.

Symbolically:
$F: X \rightarrow Y$ is onto $\iff \forall y \in Y, \exists x \in X \text{ such that } F(x) = y$

---
#### d) **Write an explicit formula for the composition $f \circ f$**
##### Solution
(Composing function $f$ with itself)

$$(f \circ f)(n) = f(f(n))$$
$$= f(2n - 5)$$
$$= 2(2n - 5) - 5$$
$$= 4n - 10 - 5$$
$$= 4n - 15$$

Thus, the explicit formula for the composition is the following:
$$f \circ f = 4n - 15$$

## 2
### Description
**Let $a_k = 2 k - 5$ and $b_k = 2 - k$.**

**Simplify each expression to only use a single summation ( $\sum$ ) or product ( $\prod$ ) using the properties of summations and products listed below. List intermediate steps.**

$\begin{aligned} \sum_{k=m}^{n} a_k - 3 \cdot \sum_{k=m}^{n} b_k \end{aligned}$

$\begin{aligned} \prod_{k=m}^{n} a_k  \cdot \prod_{k=m}^n b_k \end{aligned}$

---
Theorem 5.1.1
If $a_m, a_{m+1}, a_{m+2}, \ldots$ and $b_m, b_{m+1}, b_{m+2}, \ldots$ are sequences of real numbers and $c$ is any real number, then the following equations hold for any integer $n \geq m$ :
1. $\begin{aligned} \sum_{k=m}^n a_k+\sum_{k=m}^n b_k=\sum_{k=m}^n\left(a_k+b_k\right) \end{aligned}$
2. $\begin{aligned} c \cdot \sum_{k=m}^n a_k=\sum_{k=m}^n c \cdot a_k \quad \end{aligned}$ (generalized distributive law)
3. $\begin{aligned} \left(\prod_{k=m}^n a_k\right) \cdot\left(\prod_{k=m}^n b_k\right)=\prod_{k=m}^n\left(a_k \cdot b_k\right) \end{aligned}$

---
Example:
*Given sequences $a_k = k$ and $b_k = 2 k + 1$, simplifying an expression $\begin{aligned} \sum_{k=m}^{n} a_k + 2\cdot \sum_{k=m}^{n} b_k \end{aligned}$ could be done in the following way:*
$$\begin{aligned} \sum_{k=m}^n a_k+2 \cdot \sum_{k=m}^n b_k &=\sum_{k=m}^n k+2 \cdot \sum_{k=m}^n(2 k+1) \end{aligned}$$ by (substitution)

$$\begin{aligned} =\sum_{k=m}^n k+\sum_{k=m}^n 2 \cdot(2 k+1) \end{aligned}$$ by (2)

$$\begin{aligned} =\sum_{k=m}^n k+\sum_{k=m}^n(4 k+2) \end{aligned}$$
by (algebraic simplification)

$$\begin{aligned} =\sum_{k=m}^n(k+(4 k+2)) \end{aligned}$$
by (1)

$$\begin{aligned} =\sum_{k=m}^n(5 k+2) \end{aligned}$$
by (algebraic simplification)

---
##### Solution
$$\begin{aligned} \sum_{k=m}^{n} a_k - 3 \cdot \sum_{k=m}^{n} b_k \end{aligned}$$
by (substitution)
$$\begin{aligned} &= \sum_{k=m}^{n} 2k - 5 - 3 \cdot \sum_{k=m}^{n} 2 - k \end{aligned}$$
by (2)
$$\begin{aligned} &= \sum_{k=m}^{n} 2k - 5 \cdot \sum_{k=m}^{n} -3 \cdot (2 - k) \end{aligned}$$
by (algebraic simplification)
$$\begin{aligned} &= \sum_{k=m}^{n} 2k - 5 \cdot \sum_{k=m}^{n} -6 + 3k \end{aligned}$$
by (1)
$$\begin{aligned} &= \sum_{k=m}^{n} (2k - 5 + 3k-6) \end{aligned}$$
by (algebraic simplification)
$$\begin{aligned} &= \sum_{k=m}^{n} 5k - 11 \end{aligned}$$

---
$$\begin{aligned} \prod_{k=m}^{n} a_k  \cdot \prod_{k=m}^n b_k \end{aligned}$$
by (substitution)
$$\begin{aligned} &= \prod_{k=m}^{n} 2k - 5 \cdot \prod_{k=m}^n 2 - k \end{aligned}$$
by (3)
$$\begin{aligned} &= \prod_{k=m}^{n} (2k - 5) \cdot (2 - k) \end{aligned}$$
by (algebraic simplification)
$$\begin{aligned} &= \prod_{k=m}^{n} (9k-2k^2-10) \end{aligned}$$

## 3
### Description
**Prove, using mathematical induction, that $3$ divides $n^3 + 5n - 6$ for all integers $n\geq 0$.**

*Hint: You can use the fact that given $a \,| b$ and $a \,| c$, we can conclude $a \,| (b + c)$ for all integers $a,b,c$. Moreover, you can use the binomial theorem for exponent $3$, which states that $(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3$ for all real numbers $a, b$.*

##### Solution
...