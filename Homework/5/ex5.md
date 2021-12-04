# Group 1



**Problem 6.3.**
A robot named Wall-E wanders around a two-dimensional grid. He starts out at $(0,0)$ and is allowed to take four different types of steps:

1. $(+2,-1)$
2. $(+1,-2)$
3. $(+1,+1)$
4. $(-3,0)$

Thus, for example, Wall-E might walk as follows. The types of his steps are listed above the arrows.
$$
(0,0) \stackrel{1}{\rightarrow}(2,-1) \stackrel{3}{\rightarrow}(3,0) \stackrel{2}{\rightarrow}(4,-2) \stackrel{4}{\rightarrow}(1,-2) \rightarrow \ldots
$$
Wall-E's true love, the fashionable and high-powered robot, Eve, awaits at $(0,2)$.

**(a)** Describe a state machine model of this problem.
**(b)** Will Wall-E ever find his true love? Either find a path from Wall-E to Eve, or use the Invariant Principle to prove that no such path exists.

- **(a)** 

  1. states $::=(x,y)$,
  2. start state :: $=(0,0)$,
  3. transitions are defined by the rule

  $$
  (x, y) \longrightarrow \{(x+2, y-1),(x+1,y-2),(x+1,y+1),(x-3,y)|x,y\in\mathbb{N}\}
  $$

- **(b)** 

  ​	$Proof.$ We assume that ( $a, b$ ) can attach from $(0,0)$ by these transitions .So we can get the equation group :


$$
\left\{\begin{array}{c}
2 x_{1}+x_{2}+x_{3}-3 x_{4}=a \\
-x_{1}-2 x_{2}+x_{3}=b
\end{array}\right.
$$

​		We can get the result by the linear algebra:
$$
\left\{\begin{array}{l}
x_{1}=2 k_{1}-k_{2}+\frac{2 a+b}{3} \\
x_{2}=-k_{1}+k_{2}- \frac{a+2 b}{3} \\
x_{3}=k_{2} \\
x_{4}=k_{1}
\end{array}\right.
$$
​		In the result, $k_{2}$ and $k_{1} \in \mathrm{R}$
​		As for every point, we can get by these transitions .But in this situation $x_{1}, \mathrm{x}_{2}, \mathrm{x}_{3}$ and $x_{4}$ are positive integer .So if these don't fit the condition ,the way is not existed .As for $(0,2)$, it don't fit the condition, so we can get the conclusion : Wall-E can't find his true love,


***

**Problem 6.4.**

​	A hungry ant is placed on an unbounded grid. Each square of the grid either con- tains a crumb or is empty. The squares containing crumbs form a path in which, except at the ends, every crumb is adjacent to exactly two other crumbs. The ant is placed at one end of the path and on a square containing a crumb. For example, the figure below shows a situation in which the ant faces North, and there is a trail of food leading approximately Southeast. The ant has already eaten the crumb upon which it was initially placed.

![image-20211110141724744](../../../../../../Users/jin/Library/Application Support/typora-user-images/image-20211110141724744.png)

​	The ant can only smell food directly in front of it. The ant can only remember a small number of things, and what it remembers after any move only depends on what it remembered and smelled immediately before the move. Based on smell and memory, the ant may choose to move forward one square, or it may turn right or left. It eats a crumb when it lands on it.
​	The above scenario can be nicely modelled as a state machine in which each state is a pair consisting of the “ant’s memory” and “everything else”—for example, information about where things are on the grid. Work out the details of such a model state machine; design the ant-memory part of the state machine so the ant will eat all the crumbs on any finite path at which it starts and then signal when it is done. Be sure to clearly describe the possible states, transitions, and inputs and outputs (if any) in your model. Briefly explain why your ant will eat all the crumbs.
​	Note that the last transition is a self-loop; the ant signals done for eternity. One could also add another end state so that the ant signals done only once.



$Proof.$

1. states $::=(x,y)$,

2. start state :: $=(0,0)$,

3. transitions are defined by the rule
   - Eat the the current grid food from.
   - Go one space ahead, when there is food in front of the grid.
   - Go one block to the left, when there is food on the left side of the grid.
   - Go one block to the right, when there is food on the right side of the grid.
   -  Jump out of the loop, when there is no food in front of the ant.

According to Statement of the Invariant Principle,ant will eat all the crumbs.



