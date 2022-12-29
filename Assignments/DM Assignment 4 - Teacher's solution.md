# Discrete Mathematics - Peergrade Solution 4

## 1. 
$A=\{1,2,3,4,5,6\}$ and $R$ is a relation on $A$,
$$
m R n \Leftrightarrow 2 \mid(m+n) \quad \text { for all } m, n \in A
$$

- (a) 
Directed graph:
![|400](https://cdn.mathpix.com/cropped/2022_11_09_ad82023e51ba683494bcg-1.jpg?height=510&width=1234&top_left_y=1218&top_left_x=384)

- (b)
The equivalence class $[5]_{R}=\{1,3,5\}$

- (c) 
We have 2 equivalence classes, one for even and one for odd numbers
$[1]_{R}=[3]_{R}=[5]_{R}=\{1,3,5\}$
$[2]_{R}=[4]_{R}=[6]_{R}=\{2,4,6\}$

## 2.
- (a)
Three strings that **are** in $S$ : 'b', 'aba', 'abba'
Three strings that **are not** in $S$ : 'a', 'ab', 'bba'
(anything with odd number of 'a' should not be in $S$ ) 

- (b)
$$
\begin{gathered}
a_{n}= \begin{cases}0 & \text { if } n=0 \\
a_{n-1}+2 n+3 & \text { if } n>0\end{cases} \\\\
a_{n}=n \cdot(n+4) \quad \text { for all integers } n \geq 0 .
\end{gathered}
$$
Proof by Induction:
Basis step: Prove for $n=0$
$$
a_{0}=0 \cdot(0+4)=0
$$
Inductive step: 
assume $a_{n}=n \cdot(n+4)$,
then prove $a_{n+1}=(n+1) \cdot((n+1)+4)$
$$
\begin{aligned}
a_{n+1} &=a_{n}+2 \cdot(n+1)+3 & \text { by def } \\
&=n \cdot(n+4)+2 \cdot(n+1)+3 & \text { substitute } a_{n} \\
&=n^{2}+4 n+2 n+2+3 & \text { remove parenthesis } \\
&=n^{2}+n+5 n+5 & \text { rearrange elements } \\
&=n \cdot(n+1)+5 \cdot(n+1) & \text { factorize out n and } 5 \\
&=(n+1) \cdot(n+5) & \text { factorize }(\mathrm{n}+1) \text { element } \\
&=(n+1) \cdot((n+1)+4) \quad \checkmark &
\end{aligned}
$$

## 3. 
If $R$ is a relation on $\mathbb{Z}$ defined:
$$
m R n \quad \Leftrightarrow \quad m^{2}-n^{2} \geq 0 \quad \text { for all } m, n \in \mathbb{Z}
$$

- (a) 
Yes, $R$ is reflexive:
Proof:
For $R$ to be reflexive, $n R n, \forall n \in \mathbb{Z}$.
Consider an arbitrary integer $n$, then:
$$
\begin{aligned}
& n^{2}-n^{2} \geq 0 \\
& 0 \geq 0 \quad \text { which is true } \forall n \in \mathbb{Z}
\end{aligned}
$$
Therefore $n R n$, for all $n \in \mathbb{Z}$

- (b) 
Yes, $R$ is transitive 
Proof:
For $R$ to be transitive, $m R n \wedge n R o \Longrightarrow m R o, \forall m, n, o \in \mathbb{Z}$. 
Consider arbitrary integers $n, m, o$, such that $m R n$ and $n R o$ 
Then:
$$
\begin{array}{rrr}
m^{2}-n^{2} & \geq 0 & \text { by def. of } m R n \\
m^{2} & \geq n^{2} & \\
n^{2}-o^{2} & \geq 0 & \\
n^{2} & \geq o^{2} & \text { by def. of } n R o \\
m^{2} & \geq n^{2} \geq o^{2} & \\
m^{2} & \geq o^{2} & \text { by the property of integers provided } \\
m^{2}-o^{2} & \geq 0 &
\end{array}
$$
Therefore if $m R n$ and $n R o$, then $m R o$, for all $m, n, o \in \mathbb{Z}$

- (c) 
$\mathbf{N o}, R$ is not symmetric:
For $R$ to be symmetric, if $n R m$, then $m R n, \forall n, m \in \mathbb{Z}$
Counterexample:
Let $m=1$ and $n=2$, then:
$n^{2}-m^{2} \geq 0 \Longrightarrow(n, m) \in R$
but $m^{2}-n^{2} \nsupseteq 0 \Longrightarrow(m, n) \notin R$

- (d) 
$\mathbf{N o}, R$ is not antisymmetric:
For $R$ to be antisymmetric, if $n R m \wedge m R n$, then $n=m, \forall m, n \in$
$\mathbb{Z}$
Counterexample:
Let $m=2$ and $n=-2$, then:
$n^{2}-m^{2} \geq 0 \Longrightarrow n R m$
$m^{2}-n^{2} \geq 0 \Longrightarrow m R n$
but $n \neq m$