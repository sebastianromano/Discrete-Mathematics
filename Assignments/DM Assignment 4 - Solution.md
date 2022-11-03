# Discrete Mathematics - Assignment 4 - Solution

---

![[DM Assignment 4 - Description#1)]]

### 1a)


### 1b)


### 1c)

---

![[DM Assignment 4 - Description#2)]]

### 2a)


### 2b)

Basis step
Let $n=0$. It is known that the sequence can be recursively defined as $a_0=0$. Finding out if the above equation holds for $a_n$ when $n=0$ is the base step: 

$$
\begin{align*}
a_{n} & = n(n+4)\\
a_{0} & = 0(0+4) = 0
\end{align*}
$$

Inductive step
Let $n > 0$. Let's assume that the equation $a_n=n(n+4)$ is true for $n=n$.

$$
a_n=n(n+4)
$$

In order to prove this by mathematical induction, it's necessary to prove that it holds for $n=n+1$

$$
a_{n+1}=(n+1)((n+1)+4)
$$

Step-by-step transformation

$$
\begin{array}{rlr}
a_{n+1} & =a_n+2(n+1)+3 & \text { (by the recurrence relation) } \\
& =n(n+4)+2n(n+1)+3 & \text { (inductive hypothesis) } \\
& =n^2+4n+2n+2+3 & \text { (distributivity) } \\
& =n^2+6n+5 & \text { (associativity and commutativity)}
\end{array}
$$

Now simplifying both sides of the equation to confirm that they do indeed come to the same expression

$$
\begin{array}{rlr}
(n+1)((n+1)+4) & = (n+1)(n+5) & \text{ (by distributivity)}\\
& = n^{2}+5n+n+5 & \text{ (by distributivity)}\\
& = n^{2}+6n+5
\end{array}
$$

Thus, by mathematical induction, the above proof shows that the sequence satisfies the equation: 

$$a_n = n(n+4) \qquad \text{for all integers } n \ge 0$$

---

![[DM Assignment 4 - Description#3]]

### 3a)
$R$ is reflexive. 
In order to prove this, the definition (page 495, DM)

$$
R \text{ is reflexive } \iff \forall x \in \mathbb{Z},  x R x
$$

---
---

proof from other assignment
So to show a proof that $R$ is reflexive, let's assume some $x \in \mathbb{Z}$ and then show that $x R x$. Any $x \in \mathbb{Z}$ would by definition of equality of integers be equal to itself. 
Therefore, by definition, $m R n$ is reflexive.

(b) $R$ is transitive. 
$R$ is transitive iff $\forall x, y, z \in \mathbb{Z}$, if $x R y$ and $y R z$ then $x R z$.
To prove that $R$ is transitive, we assume some $x, y, z \in \mathbb{Z}$, such that $x R y$ and $y R z$ hold, and then show that $x R z$ holds.
Let $x, y, z \in \mathbb{Z}$, such that $x R y$ and $y R z$. By definition (of $R$ ) this means that $|x| \leq|y|$ and $|y| \leq|z|$. Since $\leq$ is transitive, we can conclude that $|x| \leq|z|$. Hence, by definition (of $R$ ), we have that $x R z$.
This shows that $R$ is transitive.
(c) $R$ is not symmetric. Let's look at the definition:
$R$ is symmetric iff $\forall x, y \in \mathbb{Z}$, if $x R y$ then $y R x$.
We give a counterexample for this property. Set $x=1$ and $y=2$. Then we have that $1 R 2$ (because $|1| \leq|2|$ ), but we do not have that $2 R 1$ (because $|2| \leq|1|$ ). This shows that $R$ is not symmetric.

---
---

### 3b)


### 3c)


### 3d)

