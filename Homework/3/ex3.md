# Group 1



**Problem 3.21.**

Use the equivalence axioms of Section 3.4.2 to convert the formula
$$
𝐴 \ \ 𝑋𝑂𝑅\ \ 𝐵\ 𝑋𝑂𝑅\ \  𝐶
$$
a)   .. to disjunctive (OR of AND’S) form, 

b)   .. to conjunctive (AND of OR’S) form.

---

- a)

Using

$$\text{A\ }\text{XOR}\ B \Leftrightarrow (A\ \text{AND}\ \overline{B})\ \text{OR}\ (\overline{A}\ \text{AND}\ B)$$

We have

$$\lbrack\ (\text{A\ }\text{XOR}\ B) \text{AND}\ \overline{C}\rbrack\ \text{OR}\ \lbrack\ \text{NOT}\ (\text{A\ }\text{XOR}\ B)\ \text{AND}\ C\rbrack$$



And,

1. $$\text{A\ }\text{XOR}\ B \Leftrightarrow (A\ \text{AND}\ \overline{B})\ \text{OR}\ (\overline{A}\ \text{AND}\ B) $$

2. $$
   \text{NOT}\ (\text{A\ }\text{XOR}\ B)\Leftrightarrow \text{NOT}\ ((A\ \text{AND}\ \overline{B})\ \text{OR}\ (\overline{A}\ \text{AND}\ B)) \\ \Leftrightarrow \text{NOT}\ (A\ \text{AND}\ \overline{B})\ \text{AND}\text{\:\:}\text{NOT}\ (\overline{A}\ \text{AND}\ B))\ \\ \Leftrightarrow (\overline{A}\ \text{OR}\ B)\ \text{AND}\ (A\ \text{OR}\ \overline{B})\
   $$

   

which becomes,

$$\lbrack((A\ \text{AND}\ \overline{B})\ \text{OR}\ (\overline{A}\ \text{AND}\ B))\ \text{AND}\ \overline{C}\rbrack\ \text{OR}\ \lbrack((\overline{A}\ \text{OR}\ B)\ \text{AND}\ (A\ \text{OR}\ \overline{B}))\ \text{AND}\ C\rbrack$$

$$\lbrack((A\ \text{AND}\ \overline{B}\ \text{AND}\ \overline{C})\ \text{OR}\ (\overline{A}\ \text{AND}\text{\:B\:}\text{AND}\ \overline{C}))\rbrack\ \text{OR}\ \lbrack((\overline{A}\ \text{OR}\ B)\ \text{AND}\ (A\ \text{OR}\ \overline{B}))\ \text{AND}\ C\rbrack$$



And,

3. $$((\overline{A}\ \text{OR}\ B)\ \text{AND}\ (A\ \text{OR}\ \overline{B})) \Leftrightarrow (\overline{A}\ \text{AND}\ (A\ \text{OR}\ \overline{B}))\ \text{OR}\ (B\ \text{AND}\ (A\ \text{OR}\ \overline{B})) \Leftrightarrow (\overline{A}\ \text{AND}\ \overline{B})\ \text{OR}\ (A\ \text{AND}\ B)$$

which becomes,

$$\lbrack((A\ \text{AND}\ \overline{B}\ \text{AND}\ \overline{C})\ \text{OR}\ (\overline{A}\ \text{AND}\text{\:B\:}\text{AND}\ \overline{C}))\rbrack\ \text{OR}\ \lbrack((\overline{A}\ \text{AND}\ \overline{B})\ \text{OR}\ (A\ \text{AND}\ B))\ \text{AND}\ C\rbrack$$

$$\lbrack((A\ \text{AND}\ \overline{B}\ \text{AND}\ \overline{C})\ \text{OR}\ (\overline{A}\ \text{AND}\text{\:B\:}\text{AND}\ \overline{C}))\rbrack\ \text{OR}\ \lbrack((\overline{A}\ \text{AND}\ \overline{B}\ \text{AND}\ C)\ \text{OR}\ (A\ \text{AND}\text{\:B\:}\text{AND}\ C))\rbrack$$

$$(A\ \text{AND}\ \overline{B}\ \text{AND}\ \overline{C})\ \text{OR}\ (\overline{A}\ \text{AND}\text{\:B\:}\text{AND}\ \overline{C})\ \text{OR}\ (\overline{A}\ \text{AND}\ \overline{B}\ \text{AND}\ C)\ \text{OR}\ (A\ \text{AND}\text{\:B\:}\text{AND}\ C)$$



- b)   

Using

$$A \oplus B \Leftrightarrow (A\ \text{OR}\ B)\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B})$$

We have

$$\lbrack\ (\text{A\ }\text{XOR}\ B) \text{OR}\ {C}\rbrack\ \text{AND}\ \lbrack\ \text{NOT}\ (\text{A\ }\text{XOR}\ B)\ \text{OR}\ \overline{C}\rbrack$$

And,

1. $$A \oplus B \Leftrightarrow (A\ \text{OR}\ B)\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B})$$

2. $$
   \text{NOT}\ (\text{A\ }\text{XOR}\ B)\Leftrightarrow \text{NOT}\ ((A\ \text{OR}\ B)\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B})) \\ \Leftrightarrow \text{NOT}\ (A\ \text{OR}\ {B})\ \text{OR}\text{\:\:}\text{NOT}\ (\overline{A}\ \text{OR}\ \overline{B}))\ \\ \Leftrightarrow (\overline{A}\ \text{AND}\ \overline{B})\ \text{OR}\ (A\ \text{AND}\ {B})\
   $$

   

which becomes,

$$\lbrack\ ((A\ \text{OR}\ B)\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B})) \text{OR}\ {C}\rbrack\ \text{AND}\ \lbrack\ ((\overline{A}\ \text{AND}\ \overline{B})\ \text{OR}\ (A\ \text{AND}\ {B}))\ \text{OR}\ \overline{C}\rbrack$$

$$\lbrack\ (A\ \text{OR}\ B \ \text{OR}\ {C})\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B} \ \text{OR}\ {C}) \rbrack\ \text{AND}\ \lbrack\ ((\overline{A}\ \text{AND}\ \overline{B})\ \text{OR}\ (A\ \text{AND}\ {B}))\ \text{OR}\ \overline{C}\rbrack$$

And,

3. $$ (\overline{A}\ \text{AND}\ \overline{B})\ \text{OR}\ (A\ \text{AND}\ {B}) \Leftrightarrow [\overline{A}\  \text{OR}\ (A\ \text{AND}\ {B})]\  \text{AND}\ [\overline{B} \ \text{OR}\ (A\ \text{AND}\ {B})]  \\ \Leftrightarrow 
   (\overline{A} \ \text{OR}\ {B})\  \text{AND}\  (\overline{B} \ \text{OR}\ {A}) $$

which becomes,

$$ \lbrack\ (A\ \text{OR}\ B \ \text{OR}\ {C})\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B} \ \text{OR}\ {C}) \rbrack\ \text{AND}\ \lbrack\ ((\overline{A} \ \text{OR}\ {B})\  \text{AND}\  (\overline{B} \ \text{OR}\ {A}))\ \text{OR}\ \overline{C}\rbrack$$ 

$$ \ (A\ \text{OR}\ B \ \text{OR}\ {C})\ \text{AND}\ (\overline{A}\ \text{OR}\ \overline{B} \ \text{OR}\ {C})\ \text{AND}\ \ (\overline{A} \ \text{OR}\ {B} \ \text{OR}\ \overline{C})\  \text{AND}\  ({A} \ \text{OR}\ \overline{B} \ \text{OR}\ \overline{C})\ $$ 

