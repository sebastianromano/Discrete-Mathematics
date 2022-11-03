# Discrete Mathematics - Assignment 4 - Description
- PDF [[DM 2022 - Assignment 4.pdf]]

---

## 1
Let $A = \{1, 2, 3, 4, 5, 6\}$ and let $R$ be a relation on $A$ defined as follows:

$$m\,R\,n \quad \Leftrightarrow \quad 2 \mid (m+n) \qquad \text{for all } m,n \in A$$

### 1a)
Draw the directed graph of $R$


### 1b)
Find the equivalence class $[5]_R$


### 1c)
How many distinct equivalence classes does the relation $R$ have?


---

## 2
### 2a)
(page 364)

Let $S$ be a set of strings over the set $\{a,b\}$ defined recursively as follows:

I BASE 
> statement that certain objects belong to the set

$b \in S$

II.RECURSION 
> collection of rules indicating how to form new objects from those already known to be in the set

If $s \in S$ then
- II(a) $sb \in S$
- II(b) $asa \in S$

III. RESTRICTION
> statement that no objects belong to the set other than those generated from (I) and (II)

Nothing is in $S$ other than objects defined in I and II above.

List three strings that are in $S$ and three strings that are not in $S$.


### 2b)
Let the sequence $a_0, a_1, a_2,\dots$ be recursively defined as follows:

$$
a_{n} = \begin{cases} 0 & \text { if } n=0 \\
a_{n-1}+2 n+3 & \text{ if } n>0 \\
\end{cases}
$$

Using mathematical induction, prove that this sequence satisfies the following equation: 

$$
a_{n} = n(n+4) \qquad \text{ for all integers } n \ge 0
$$

---

## 3
Let $R$ be a relation on $\mathbb{Z}$ defined as follows:

$$
m\,R\,n\quad \Leftrightarrow \quad m^2 - n^2 \geq 0 \qquad \text{for all } m,n \in \mathbb{Z}
$$

### 3a)
Is $R$ reflexive?

### 3b)
Is $R$ transitive?

### 3c)
Is $R$ symmetric?

### 3d)
Is $R$ antisymmetric?

Justify each of your answers by providing either a proof or a counterexample.

You may use the following property of integers: 

$$\text{For all } a, b, c \in \mathbb{Z} \text{if } a \geq b \text{ and } b \geq c \text{ then } a \geq c$$

