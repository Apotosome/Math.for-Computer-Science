# Group 1



**Problem 4.3.**

​	**(a)** *Verify that the propositional formula $(P$ AND $\bar{Q})$ OR $(P$ AND $Q)$ is equivalent to $P$.*
​	**(b)** *Prove that*
$$
A=(A-B) \cup(A \cap B)
$$
​	*for all sets, $A, B$, by showing*
$$
x \in A \text { IFF } x \in(A-B) \cup(A \cap B)
$$
​	*for all elements $x$ using the equivalence of part (a) in a chain of IFF's.*



- **(a)** 

  ​	$Proof.$  The equality  is equivalent to the assertion that

$$
x \in (P \text { AND } \bar{Q}) \text { OR } (P \text { AND } {Q}) \text { iff } x \in P
$$

​			for all $x$. Now we'll prove by a chain of iff's.
​			Now we have
$$
\begin{aligned} x &
\in (P \text { AND } \bar{Q}) \text { OR } (P \text { AND } {Q}) &  \\
&\text { iff } x\in (P \text { OR } (P \text { AND } {Q})) \text { AND } (\bar{Q} \text { OR } {(P \text { AND } {Q})}) &  \\
&\text { iff } x\in P \text { AND } (P \text { AND } {Q} \text { AND } \bar{Q}) &  \\
&\text { iff } x\in P  &  \\
\end{aligned}
$$

- **(b)** 

  ​	$Proof.$  The equality  is equivalent to the assertion that

$$
x \in A \text { iff } x \in(A-B) \cup(A \cap B)
$$
​			for all $x$. Now we'll prove by a chain of iff's.
​			Now we have
$$
\begin{aligned} x &
\in(A-B) \cup(A \cap B) &  \\
&\text { iff }  (x \in A-B) \text { OR }(x \in A \cap B)  &  \\
&\text { iff }  (x \in A \text { AND } x\notin B) \text { OR }(x \in A \text { AND } x\in B)  &  \\
&\text { iff }  (x \in A \text { OR } (x \in A \text { AND } x\in B)) \text { AND }(x \notin B \text { OR } (x \in A \text { AND } x\in B))  &  \\
&\text { iff }  x \in A \text { AND } (x \in A \text { OR } (x\in B \text{ AND } x \notin B)) &  \\
&\text { iff }  x \in A \text { AND } (x \in A  ) &  \\
&\text { iff }  x \in A &  \\
\end{aligned}
$$




***

**Problem 4.5.**
*Prove De Morgan's Law for set equality*
$$
\overline{A \cap B}=\bar{A} \cup \bar{B}
$$
*by showing with a chain of IFF's that $x \in$ the left-hand side of $(4.9)$ iff $x \in$ the right-hand side. You may assume the propositional version (3.14) of De Morgan's Law.*
$$
\operatorname{NOT}(A \text { AND } B) \longleftrightarrow \bar{A} \text { OR } \bar{B} \quad \text { (De Morgan for AND) }(3.14)
$$


- $Proof.$  The equality  is equivalent to the assertion that

$$
x \in \overline{A \cap B} \text { iff } x \in \bar{A} \cup \bar{B}
$$

​			for all $x$. Now we'll prove by a chain of iff's.
​			Now we have
$$
\begin{aligned} x &
\in{\overline{A \cap B}} & \\
&\text { iff }  (x \notin A \cap B)  &  \\
&\text { iff }  (x \notin {A}  \text{ OR }  x \notin {B})  &    (De\ Morgan\ for\ AND(3.14))\\
&\text { iff }  (x \in \overline{A}  \text{ OR }  x \in {B})  &  \\
&\text { iff }  ( \overline{A}  \cup   \overline{B})  &  \\

\end{aligned}
$$




***

**Problem 4.6.**
*Powerset Properties.
	Let $A$ and $B$ be sets.*
	**(a)** *Prove that*
$$
\text{pow}(A \cap B)=\text{pow}(A) \cap \text{pow}(B)
$$
​	**(b)** *Prove that*
$$
(\text{pow}(A) \cup \text{pow}(B)) \subseteq \text{pow}(A \cup B)
$$
​	*with equality holding iff one of $A$ or $B$ is a subset of the other.*



- **(a)** 

  ​		$Proof.$  The equality  is equivalent to the assertion that

$$
x \in \text{pow}(A \cap B) \text { iff } x \in \text{pow}(A) \cap \text{pow}(B)
$$

​					for all $x$. Now we'll prove by a chain of iff's.
​					Now we have
$$
\begin{aligned} x &
\in \text{pow}(A \cap B) & \\
&\text { iff }  (x \subseteq A \cap B)  &  \\
&\text { iff }  (x \subseteq A \text{ AND } x \subseteq B)  &  \\
&\text { iff }  (\text{pow}(A) \text{ AND } \text{pow}(B))  &  \\
&\text { iff }  (\text{pow}(A) \cap \text{pow}(B))  &  \\
\end{aligned}
$$

- **(b)** 

  ​			$Proof.$  The equality  is equivalent to the assertion that
  $$
  x \in (\text{pow}(A) \cup \text{pow}(B))  \text { iff } x \in \text{pow}(A \cup B)
  $$
  ​			for all $x$. Now we'll prove by a chain of iff's.
  ​			Now we have
  $$
  \begin{aligned} x &
  \in \text{pow}(A) \cup \text{pow}(B) & \\
  &\text { iff }  x \subseteq A \text{ OR } x \subseteq B  &  \\
  &\text { iff }  x \subseteq A\cup B  \text{ OR } x \subseteq B\cup A  &  \\
  &\text { iff }  x\in \text{pow}(A\cup B) \cup \text{pow}(B\cup A)  &  \\
  &\text { iff }  x\in \text{pow}(A\cup B)  &  \\
  \end{aligned}
  $$





***

**Problem 5.4.**
*Prove by induction on $n$ that*
$$
1+r+r^{2}+\cdots+r^{n}=\frac{r^{n+1}-1}{r-1}
$$
*for all $n \in \mathbb{N}$ and numbers $r \neq 1$.*



$Proof.$ 

- $P(0)$ is true, because both sides of equation this equal one when $n=0$

- Assume that $P(n)$​ is true, that is equation  holds for some nonnegative integer $n$​. Then adding $r^{n+1}$​ to both sides of the equation implies that
  $$
  \begin{aligned} 1+r+r^{2}+\cdots+r^{n}+r^{n+1} &
  =\frac{r^{n+1}-1}{r-1}+r^{n+1}\\ 
  &=\frac{r^{n+1}-1+r^{n+1}(r-1)}{r-1} \\
  &=\frac{r^{n+1}-1+r^{n+2}-r^{n+1}}{r-1} \\
  &=\frac{r^{n+2}-1}{r-1} \\
  \end{aligned}
  $$
  which proves $P(n+1)$
  So it follows by induction that $P(n)$ is true for all nonnegative $n$​.





***

**Problem 5.5.**
*Prove by induction:*
$$
1+\frac{1}{4}+\frac{1}{9}+\cdots+\frac{1}{n^{2}}<2-\frac{1}{n}
$$
*for all $n>1$.*



$Proof.$ 

- $P(2)$ is true, because left side of equation is less than right side  when $n=2$ 
  $$
  1+\frac{1}{4}=\frac{5}{4}<2-\frac{1}{4}=\frac{7}{4}
  $$
  

- Assume that $P(n)$​ is true, that is equation  holds for some nonnegative integer $n$​. Then adding $\frac{1}{(n+1)^2}$​ to both sides of the equation implies that
  $$
  \begin{aligned} 1+\frac{1}{4}+\frac{1}{9}+\cdots+\frac{1}{n^{2}}+\frac{1}{(n+1)^2} &
  <2-\frac{1}{n}+\frac{1}{(n+1)^2}\\ 
  &=2-\left(\frac{1}{n}-\frac{1}{(n+1)^2} \right)\\
  &=2-\left(\frac{n^2+1+n}{n(n+1)^2} \right)\\
  &=2-\left(\frac{n^2+n}{n(n+1)^2}+\frac{1}{n(n+1)^2} \right)\\
  &=2-\left(\frac{1}{n+1}+\frac{1}{n(n+1)^2} \right)\\
  &=2-\frac{1}{n+1}-\frac{1}{n(n+1)^2} \\
  &<2-\frac{1}{n+1} \\
  \end{aligned}
  $$
  which proves $P(n+1)$

- So it follows by induction that $P(n)$ is true for for all $n>1$.

