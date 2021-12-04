# Group 1



**Problem 2.7.**

*Use the Well Ordering Principle to prove that any integer greater than or equal to 8 can be represented as the sum of nonnegative integer multiples of 3 and 5.*



$Proof.$  Let $S(n)$ for all integer $n≥8$, exists $x,y$ such that $n=3x+5y$

By contradiction. Assume that $S(n)$ is false. Then, some  integers serve as counterexamples to it. The collection of counterexamples is:
$$
D::=\left\{n \in \mathbb{N}, n≥8 \mid NOT(S(n))\right\}
$$
Assuming  $D$  is a nonempty set of  integers. Then, by the Well Ordering Principle, $D$ has a minimum element, which we can call $d$.  And $d$ is the smallest counterexample among the integers. 

Since $d$ is the smallest counterexample, we know $d$ will not equal to $3x+5y$  for any integer $x,y$.

Then, We can check $S(8), S(9), S(10)$ are holds.So $d$ must be greater than 10 to be a counterexample. But then,  $S(d-3)$ is greater than or equal to 8 and less than $d$, so $S(d-3)$ is hold.

So. exists $x_0,y_0$​ such that 
$$
d-3=3x_0+5y_0 \\ d=3(x_0+1) + 5y_0
$$
which means this $S(n)$ does hold for $d$, after all. Thus,$D$ is in empty, and we are done.





***

**Problem 2.8.**
*We'll use the Well Ordering Principle to prove that for every positive integer $n$, the sum of the first $n$ odd numbers is $n^{2}$, that is,*
$$
\sum_{i=0}^{n-1}(2 i+1)=n^{2}
$$
*for all $n>0$.*



$Proof.$    By contradiction. Assume that this theorem is false. Then, some positive integers serve as counterexamples to it. The collection of counterexamples is:
$$
M::=\left\{n \in \mathbb{N^*} \mid \sum_{i=0}^{n-1}(2 i+1) \neq n^{2} \right\}
$$
Assuming  $M$  is a nonempty set of postive integers. Then, by the Well Ordering Principle, $M$ has a minimum element, which we can call $m$.  And $m$ is the smallest counterexample among the postive integers. 

Since $m$ is the smallest counterexample, we know the theorem is false for $n=m$ but true for all postive integers $n<m$. But the theorem  is true for $n=1$, so $m>1$.Thus, $m≥2$. This  means $m-1$ is a positive integer. That is,
$$
\sum_{i=0}^{m-1}(2 (i-1))+1)=(m-1)^{2}
$$
But then, adding $2m-1$ to both sides, we get
$$
\sum_{i=0}^{m}(2 (i-1))+1)=(m-1)^{2}+2m-1=m^2
$$
which means this theorem does hold for $m$, after all. This is a contradiction, and we are done.

