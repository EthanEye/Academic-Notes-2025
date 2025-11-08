# Counting 9.2

## **<ins>The bijection rule:</ins>** 

Method of solving difficult counting problems by showing that the cardinality of the set to be counted is equal to the cardinality of a set that is easy to count. 

The function f that maps a set S to T is a function g that maps T to S such that for every s ∈ S and every t ∈ T, f(s) + t if and only if g(t) = s. The inverse function is denoted by f^-1.

Ex: let S and T be two finite sets. If there is a bijection from S to T then |S| = |T|. Every person in a theater must submit a ticket to an usher in order to enter. One way to count the number of people in the theater is to count the number of tickets submitted. In this case, the bijection is from the set of submitted tickets to the set of people in the theater. Each ticket is mapped to the person who submits the ticket to the usher. The inverse function maps each person to a ticket.

Reminder: The powerset denoted P(X) is the set of all subsets of X. {0,1}^3 the super script here means Cartesian power or repeated concatenation in the context of strings. It means the set of all strings with length 3 of the alphabet.

> x= {a,b,c}
> P(x) = {Ø, {a}, {b}, {c}, {a,b}, {a,c}, {b,c}, {a,b,c}}
> {0,1}^3 = {000,100,010,001,110,101,011,111}
> f → |P(x)| = |{0,1}^3|
> f is the bijection between the set {a,b,c} and {0,1}

2^3 = 8 subsets for P(x) & {0,1}^3 also has 8 subsets (The cardinality of a power set is the number of subsets).

**What is f({1,4})?**

>f({1,4}) = 1001

**Which element is not in f^-1({1101})?**

> f^-1({1101}) = 3

**How many elements in f^-1({0000})?**

>f^-1{0000} = 0 elements

## **<ins>The k-to-1 rule:</ins>** 

A group of kids at a slumber party leave their shoes in a pile at the door. One way to count the number of kids at the party is to count the number of shoes and divide by 2. One must establish that each kid has exactly one pair of shoes in the pile. Counting kids by counting shoes and dividing by 2 is an example of the k-to-2 rule with k = 2.Applying the k-to-1 rule requires a well-defined function from objects one can count to objects one wants to count. In the example with the shoes, the function maps each shoe to the kid who owns it. Below is a definition of the kind of function that is required:

If a function $f: A \to B$ is **k-to-1**, meaning that **each element of $B$ has exactly $k$ preimages in $A$**, then:

$$
|A| = k \cdot |B|
$$

#### Explanation
- For every $y \in B$, there are exactly $k$ distinct $x \in A$ such that $f(x) = y$.
- So the size of the domain $A$ is $k$ times the size of the codomain $B$.

#### Example
If $f: \{1,2,3,4,5,6\} \to \{a,b\}$ is 3-to-1:
- Each element in $\{a,b\}$ has 3 preimages.
- So $|A| = 6$ and $|B| = 2$, and indeed $6 = 3 \cdot 2$.















