Tags: [[learning]] [[maths]]

![[Understanding Analysis.pdf]]

Written on 2025-11-10
## 1.1

How to conclude that the square root of 2 is irrational?

if we assume that $p$ and $q$ are integers without any common factors and if there are any common factors then they have been factored out.
$$
\left (\frac{p}{q} \right)^2 = 2 
$$
$$
\frac{p^2}{q^2} = 2
$$
$$
p^2 = 2q^2
$$
now this states that $p^2$ is an even number and as that square root of an even number is always even then that means that $p$ is also even. now if we write that
$$
p = 2r
$$
and we substitute $p$ into the former equation then we get.
$$
(2r)^2 = 2q^2
$$
$$
4r^2 = 2q^2
$$
$$
2r^2 = q^2
$$

now this proves that $q^2$ is even, even though at the start we said that there were no common factors between $p$ and $q$. according to the book this means that the square root of 2 is irrational but how??

the natural numbers are the normal numbers from  to $1$ to $\infty$
$$
\mathbb{N} = \{1,2,3,4,5,\dots\}
$$
now with the natural numbers math can be done perfectly well but in order to do subtraction you need to extend it to the integers which go from $-\infty$ to $\infty$. which are called the integers.
$$
\mathbb{Z} = \{\dots, -3, -2, -1, 0, 1, 2, 3,\dots\}
$$
now this allows you to do subtractions as you have the necessary additive inverses  and allows you to have an **additive identity(which means that any number added to this is equal to itself)** which is $0$ and $1$ can act as the **multiplicative identity(any number multiplied by this is equal to the number itself)**.  but in order to do division you need the necessary multiplicative inverses thus the numbers are extended to the rational numbers where:
$$

\mathbb{Q}=\{\text{all fractions }\frac{p}{q}\text{ where p an q are integers and }p \neq 0\}
$$
A field is any set where addition and multiplication are well-defined operations that are commutative, associative, and obey the familiar distributive property :
$$
a(b+c) = ab+ ac
$$
There must be an additive identity and every element must have an additive inverse and multiplicative inverses must exist for all nonzero elements of the field 

Set **Q** also has a natural order defined on it. Given any two rational numbers *r* and *s*, exactly one of the following is true:
$$
r < s, \space r = s, \space r>s
$$
now if:
$$
r<s \text{ and } s<t \text{ then }  r<t  
$$
given any 2 rational numbers $r<s$, the rational number $\frac{r+s}{2}$ sits halfway between them. 

$$
\mathbb{N} \subseteq \mathbb{Z} \subseteq \mathbb{Q}
$$
what is the definition of $\mathbb{R}$?

## 1.2

A *set* is any collection of objects.These objects are referred to as the *elements of a set*. Given a set $A$, we write $x \in A$ if $x$ is is an element of $A$. If $x$ is not an element of $A$, then we write $x \notin A$.

Given two sets $A$ and $B$ the *union* is written $A \cup B$. 
$$
x \in A \cup B \text{ provided that } x \in A \text{ or } x \in B \text{ (or potentially both.)} 
$$
The intersection $A \cap B$ is  a set defined by the rule
$$
x \in A \cap B \text{ provided } x \in A \text{ and } x \in B  
$$
There are many acceptable ways to assert the contents of a set:

1. It can be defined by listing the elements in the set: $\mathbb{N} = \{1,2,3,\dots\}$
2. Sets can also be defined in words. For instance, let the set $E$ be the collection of even natural numbers.
3. Sometimes it is more efficient to provide a kind of rule or algorithm for determining the elements of a set for example $S=\{r \in \mathbb{Q}:r^2<2\}$. Read aloud the definition of $S$ says "Let $S$ be the set of all rational numbers but whose squares are less then 2." It follows that $1 \in S
4. 
5. 