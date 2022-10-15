# Discrete Mathematics
Peergrade Solution 3

## 1
Let $f : \mathbb{Z} \rightarrow \mathbb{Z}$ be defined as $f(n) = 2 n - 5$ for all integers $n$.

(a)
Examples of elements in the range of $f$ are -5, -3, and 1. In general, all odd numbers are in the range of $f$.

(b)
Yes, $f$ one-to-one. To justify that $f$ is one-to-one, we must show that for all elements $n_1$, $n_2$ in $\mathbb{Z}$, if $f(n_1) = f(n_2)$, then $n_1 = n_2$.
We have $f(n_1)= 2n_1 - 5$ and  $f(n_2)= 2n_2 - 5$. Then,

$$\eqalign{
2n_1 -5 &= 2n_2 - 5 &\implies \\
2n_1 &= 2n_2 &\implies\\
n_1 &= n_2 &\text{, as was to be shown.}\\
}$$

(c) 
No, $f$ is not onto. $f$ is by definition onto, iff for all elements $y$ in the co-domain $\mathbb{Z}$, there exists an element $n$ in the domain $\mathbb{Z}$, such that $f(n)= y$. Any even number can be used as a counterexample to disprove this claim. 

Proof by contradiction: 
Assume that $f$ is onto, that is for every $y \in \mathbb{Z}$, there exists an element $n \in \mathbb{Z}$ s.t. $f(n)= y$
Take $y = 4$. By assumption, there exists an element n in the domain $\mathbb{Z}$, such that $f(n) = 4$

$$\eqalign{
2n -5 &= 4 &\implies \\
2n &= 4+5 & \implies\\
2n &= 9 & \implies\\
n &= \frac{9}{2} \\
}$$

Since $\frac{9}{2}$ is not in the domain of $f$, and it is the only possible such $n$, we have reached a contradiction. Therefore, we have shown that $f$ is not onto.

Alternative: direct proof.
To show that $f$ is not onto, we need to show that it is not the case that for all elements $y\in\mathbb{Z}$ there is an $n\in\mathbb{Z}$ such that $f(n) = y$. That is, that there exists an element $y\in\mathbb{Z}$ such that for all $n\in\mathbb{Z}$, $f(n) \neq y$. Take $y=4$. For $f(n)=4$ it must be that $2n - 5=4$. We will solve the equation for $n$:

$$\eqalign{
2n -5 &= 4 &\implies \\
2n &= 4+5 &\implies\\
2n &= 9 &\implies\\
n &= \frac{9}{2} \\
}$$

Since $\frac{9}{2}$ is not in $\mathbb{Z}$, and it is the only value $n$ for which $f(n) = 4$, it is the case that for all $n\in\mathbb{Z}, f(n) \neq 4$. Therefore, there exists an element in the co-domain $y\in\mathbb{Z}$ such that for all $n\in\mathbb{Z}, f(n) \neq y$.

(d)

$$\eqalign{
f \circ f &= f(2n-5)\\
&= 2(2n-5) -5\\
&= 4n-10-5\\
&= 4n-15\\
}$$

## 2
(a)
$$\eqalign{
\sum_{k=m}^{n} a_k - 3\cdot \sum_{k=m}^{n} b_k &= \sum_{k=m}^{n} (2k -5) -3\cdot \sum_{k=m}^{n} (2-k) & \text{by substitution}\\
&= \sum_{k=m}^{n} (2k-5) + \sum_{k=m}^{n} -3 \cdot (2-k) &\text{by (2)}\\
&= \sum_{k=m}^{n} (2k-5) + \sum_{k=m}^{n} (-6+3k) &\text{by algebraic simplification}\\
&= \sum_{k=m}^{n} ((2k-5) + (-6+3k))&\text{by (1)}\\
&= \sum_{k=m}^{n} (5k-11) &\text{by algebraic simplification}\\
}$$

(b)
$$\eqalign{
\prod_{k=m}^{n}a_k \cdot \prod_ {k=m}^{n}b_k&= \prod_{k=m}^{n}(2-5) \cdot \prod_ {k=m}^{n}(2-k) & \text{by substitution}\\
& = \prod_{k=m}^{n} (2k-5)(2-k) & \text{by (3)}\\
& = \prod_{k=m}^{n} (4k-2k^2-10+5k) & \text{by algebraic simplification} \\
& = \prod_{k=m}^{n} (-2k^2+9k-10) & \text{by algebraic simplification} \\
}$$

## 3
Proof by mathematical induction: Let property $P(n)$ be the sentence
$$n^3 + 5n - 6 \text{ is divisible by 3}$$
We will prove that $P(n)$ is true for all integers $n\geq 0$.
1. Base case: Show that $P(0)$ is true.
	$$P(0) \text{ is true because } 0^3+5\cdot0-6 = -6 \text{ and -6 is divisible by 3}$$
2. Inductive step: 
	Show that for every integer $k \geq 0$, if  $P(k)$ is true, then $P(k+1)$ is true. Let k be any integer with $k \geq 0$, and suppose $k^3 + 5k - 6$ is divisible by 3 (this is the inductive hypothesis). By the definition of divisibility, this means that $k^3 + 5k - 6 = 3r$ for some integer r. We must show that $(k+1)^3 + 5(k+1) -6$ is divisible by 3. We can use the binomial theorem for exponent 3 and rewrite $P(k+1)$ as
	$$\eqalign{
	(k+1)^3 + 5(k+1) -6 & = k^3 + 3k^2 + 3k +1 + 5k + 5 -6 \\
    &= k^3 + 5k - 6 + 3k^2 + 3k + 6
    }$$
    
    (Option 1:) 
    We can rewrite the expression as:
    $$k^3 + 5k - 6 + 3k^2 + 3k + 6 = k^3 + 5k - 6 + 3(k^2+k+2)$$
    
    From our inductive hypothesis we know that $k^3 + 5k - 6$ is divisible by 3. Using the definition of divisibility (if $3|b$, then $b=3r$), we can conclude that 3 divides $3(k^2+k+2)$. Using the fact that given $a \,| b$ and $a \,| c$, we can conclude $a \,| (b + c)$ for all integers $a,b,c$, we see that 3 divides the sum $k^3 + 5k - 6 + 3(k^2+k+2)$.
    
    (Option 2:) 
    By the inductive hypothesis, we know that $k^3 + 5k - 6 = 3r$, hence, we can use this to rewrite the expression above as
    $$\eqalign{
    k^3 + 5k - 6 + 3k^2 + 3k + 6 &= 3r + 3k^2 + 3k + 6 \\
    &= 3(r + k^2 + k + 2)
    }$$
    
    By the definition of divisibility (if $3|b$, then $b=3r$), we have shown that $P(k) \implies P(k+1)$.
