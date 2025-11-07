**Discrete Structures Notes**

**Ethan Eye**

**Fall 2025**

**[Propositions/ Predicates/ Sets]{.underline}**

**Number sets:**

[Natural numbers (N)]{.underline} -- counting numbers (1,2,3,4...)

[Integers (ℤ)]{.underline} -- All whole numbers including zero
(-3,-2,-1,0,1,2,3...)

[Rational numbers]{.underline} (ℚ) -- Numbers that can be written as
fraction a,b ∈ ℤ, b ≠0

(1/2, -3, 0.25,7...)

[Real numbers (ℝ)]{.underline} -- All rational and irrational numbers
(-5,0,2.5, √2​,π)

**Propositions:** a statement that can be true or false but not both. We
can represent these with propositional variables.

  -----------------------------------------------------------------------
  Variable                Meaning                 Truth value
  ----------------------- ----------------------- -----------------------
  *p*                     "It is raining"         T or F

  *q*                     "It is cold"            T or F

  *r*                     "I will stay inside"    T or F
  -----------------------------------------------------------------------

**Operators:**

  ----------------------------------------------------------------------------
  Operator        Name           Symbol          Example        Meaning
  --------------- -------------- --------------- -------------- --------------
  Negation        NOT            ¬ or \~         ¬p             "It is **not**
                                                                raining."

  Conjunction     AND            ∧               p ∧ q          "It is raining
                                                                **and** cold."

  Disjunction     OR             ∨               p ∨ q          "It is raining
                                                                **or** cold."

  Implication     IF...THEN      ⇒ or            p ⇒ q          "**If** it
                                 $\rightarrow$                  rains,
                                                                **then** it is
                                                                cold."

  Biconditional   IF AND ONLY IF ⇔               p ⇔ q          "It rains **if
                                                                and only if**
                                                                it is cold.
  ----------------------------------------------------------------------------

**Predicates:** are logical statements or expressions that contain one
or more variables and become a proposition when specific values are
assigned to those variables.

**Ex: P(x): "x is greater than 5"**

**P(7): "7 is greater than 5" is true**

**P(3): "3 is greater than 5" is false**

  ----------------------------------------------------------------------------------------
  **Rule Name**        **Form**               **Explanation**
  -------------------- ---------------------- --------------------------------------------
  **Modus Ponens**     1.$P \rightarrow Q$\   If P implies Q, and P is true, then Q must
                       2.$P$\                 be true.
                       ∴ $Q$                  

  **Modus Tollens**    1.$P \rightarrow Q$\   If P implies Q, and Q is false, then P must
                       2.$\neg Q$\            be false.
                       ∴ $\neg P$             

  **Hypothetical       1.$P \rightarrow Q$\   If P implies Q and Q implies R, then P
  Syllogism**          2.$Q \rightarrow R$\   implies R.
                       ∴ $P \rightarrow R$    

  **Disjunctive        1.$P \vee Q$\          If either P or Q is true, and P is false,
  Syllogism**          2.$\neg P$\            then Q must be true.
                       ∴ $Q$                  

  **Addition**         1.$P$\                 If P is true, then "P or Q" is also true (no
                       ∴ $P \vee Q$           matter what Q is).

  **Simplification**   1.$P \land Q$\         If both P and Q are true, then P (or Q)
                       ∴ $P$                  individually is true.

  **Conjunction**      1.$P$\                 If P is true and Q is true, then "P and Q"
                       2.$Q$\                 is true.
                       ∴ $P \land Q$          

  **Resolution**       1.$P \vee Q$\          Used in propositional logic to eliminate
                       2.$\neg P \vee R$\     variables (common in AI).
                       ∴ $Q \vee R$           
  ----------------------------------------------------------------------------------------

**Rules of Inference**

**[Sets]{.underline}**

**Set:** is a well-defined collection of distinct objects, called
elements, or members. They are represented with capital letters. **Ex: A
= {1,2,3,4}**

Set builder form: B = {x \| x is even and 1 ≤ x ≤10 } In English - B is
the set of all numbers x such that x is even and x is between 1 and 10,
inclusive.

+-----------------------+-----------------------+------------------------+
| Type                  | Symbol                | Example                |
+:======================+=======================+:=======================+
| Empty                 |   --                  | {}                     |
|                       |                       |                        |
|                       |   --                  |                        |
|                       |                       |                        |
|                       |   -----------------   |                        |
|                       |   $$\varnothing$$     |                        |
|                       |   -----------------   |                        |
|                       |                       |                        |
|                       |   -----------------   |                        |
+-----------------------+-----------------------+------------------------+
| Subset                | ⊆                     | {1,2}⊆{1,2,3}          |
+-----------------------+-----------------------+------------------------+
| Proper subset         | ⊂                     | {1,2}⊂{1,2,3}          |
+-----------------------+-----------------------+------------------------+
| Universal subset      |   --                  |   --                   |
|                       |                       |                        |
|                       |   --                  |   --                   |
|                       |                       |                        |
|                       |   -------             |   -------------------- |
|                       |   $$U$$               |   All elements under   |
|                       |   -------             |   consideration        |
|                       |                       |   -------------------- |
|                       |   -------             |                        |
|                       |                       |   -------------------- |
+-----------------------+-----------------------+------------------------+

**Important set operations:**

  -----------------------------------------------------------------------
  Operation         Symbol            Meaning           Example
  ----------------- ----------------- ----------------- -----------------
  Union             ∪                 All elements no   
                                      duplicates        

  Intersection      ∩                 Elements common   
                                      in both sets      

  Difference        −                 Elements that are 
                                      in one set but    
                                      not the other     

  Complement        A^c^              All elements not  
                                      in the set        

  Cartesian product ×                 All ordered pairs 
  -----------------------------------------------------------------------

**[Big O Notation]{.underline}**

**[Proofs 1]{.underline}**

**Theorem:** is a statement that can be proven to be true. A **proof**
is a series of steps that follow logically from assumptions from
previously proven statements.

**Assertion:** A statement or claim declared to be true. Like an assert
in JUnit, it is a condition that must hold at a specific point in a
program. It can be thought of as a statement that **"claims"** or
**"states as true"**.

**6.1.1**

A integer x is even if there is an integer k such that x = 2k

A integer x is odd if there is an integer k such that x = 2k + 1

(k is just a integer that makes the equation true)

**6.1.3**

An integer x divides an integer y if and only if x ≠ 0 and y = kx, for
some integer k. The fact that x divides y is denoted x \| y. The fact
that x does not divide y is denoted x ∤ y.

Most theorems are assertions about all elements in a set and are
therefore universal statements. A universal statement does not
necessarily explicitly use words associated with a universal quantifier,
"for all", or "for every".

**Domain:** in logic and math this is the set of input values x.

**Range:** is the set of output values from the domain.

**6.2.1**

**Proof by exhaustion:** if the domain of the universal statement is
small proving each statement by checking each element may be the
easiest.

Ex: if n ∈ {-1,0,1}, then n^2^ = \|n\|

**Proof by universal generalization:** if the domain of a universal
statement is large or a infinite set it becomes unreasonable to prove
the statement individually for each element in the domain. This method
names a arbitrary object in the domain and proves the statement for that
object.

We can disprove universal generalization by providing one counter
example.

**Existence proof:** Is a proof that shows a existential statement is
true. The most common type of existence proof is **constructive proof of
existence**. Which proves that there is one element in the domain that
makes the domain true. **A non-constructive proof of existence** proves
that an element with the required properties exists without giving a
specific example.

**Important symbols for proofs:**

  -----------------------------------
  **Symbol**        **Meaning**
  ----------------- -----------------
  ∈                 Is an element

  ∉                 Is not an element

  ∀x P(x)           For all of x P(x)
                    is true

  ∃x P(x)           There exists x
                    such that P(x) is
                    true

  A \| B            B is divisible by
                    A or A divides B
  -----------------------------------

**[Common keywords for proofs:]{.underline}**

**Thus** and **Therefore:** A statement that follows form the previous
statement or previous few statements can be started with "thus" or
"therefore".

**Let** and **There is:** New variable names are introduced with the
word let. *Ex: "Let x be a positive integer". Ex: "since x divides y , x
is non zero and there is a integer k such that y = kx".*

**Suppose:** The word suppose can also be used to introduce a new
variable. It can also be used to introduce a new assumption. *Ex:
"Suppose x is odd".*

**Since:** If a statement depends on a fact that appeared earlier in the
proof or in the assumptions of the theorem, reminds the reader of the
fact before the statement.

**We will prove** and **We will show:** Important to show the reader
where the proof is leading, by saying what will be proven in the
upcoming steps of the proofs.

**By definition:** A fact that is known because of a definition, can be
started with the phrase "By definition". *Ex:* *The integer m is even.
By definition, m = 2k for some integer k.*

**By assumption:** A fact that is known because of an assumption, can be
started with the phrase "By assumption". *Ex: By assumption x is
positive. Therefore, x \> 0.* **An assumption is basically a given fact
that you take as true at the start.**

**In other words:** Used when you want to rephrase a statement in a more
specific way. Ex: We must show that the average of x and y is positive.
In other words x+y/2 \> 0.

**Gives** and **Yields:** When using algebra in a proof, you can justify
a step made with gives or yields. *Ex: multiply both side of a
inequality x \> y by 2 gives 2x \> 2y.*

**[Best practices:]{.underline}**

**Indicate where proof starts and ends:** Proof: indicates when the
proof starts and the symbol ■ shows when it ends.

**Write proofs in complete sentences:** A proof should read like English
text.

**Give reader a road map:** Begging should always state what facts are
assumed and ideally inform the reader on what is being proven in the
proof. It is helpful to indicate at one or more points in the middle
what has been proven and what has yet to be proven. *Ex: \"We have shown
that  is a positive integer. Now we must establish that  is
composite.\"*

**Introduce each variable when the variable is used for the first time**

*Ex: Let x be a positive integer. -\>Use the variable -\>Introducing
more variables to continue proof*

**Existential instantiation:** If we know something exists, that is
∃xP(x)is true. Then we can introduce a new symbol (like c) to represent
on specific object that makes P(x) true. ∃xP(x)⇒P(c) where c is the new
constant that some unspecified value which P(x) holds true.

**Direct Proof:** A logical argument in which you start from known facts
or given hypothesis and use valid rules of inference to show that a
conclusion is true.

**[Proofs 2]{.underline}**

**Proof by contrapositive:** proves that a condition theorem of the form
p ⇒ c by showing that the contrapositive ¬c ⇒ ¬p is true. In other
words, ¬c is assumed to be true, and ¬p is proven as a result of ¬c.

- Starts with the negation of the conclusion and derives the negation of
  the hypothesis. While a direct proof would start by assuming the
  hypothesis in the conditional statement.

- In proofs by contra positive with multiple hypothesis is only
  necessary to prove that one of the hypotheses is false.

**Proof by contradiction:** Assumes the statement you want to prove is
false. Us logic and known facts to deduce consequences from that
assumption. Eventually reach a contradiction -- a statement that is
impossible or always false. (Also sometimes called a **indirect**
proof).

A contradiction is an argument of the form **¬p** $\mathbf{\rightarrow}$
**c therefore, p**

+------------------+------------------------------+----------------------------+
| **Rule**         | **Form**                     | **Meaning**                |
+:=================+:=============================+:===========================+
| **Universal      | From                         | If something is true for   |
| Instantiation    | $\forall x\text{ }P(x)$,     | all x, it's true for any   |
| (UI)**           | infer $P(a)$                 | specific x.                |
+------------------+------------------------------+----------------------------+
| **Universal      | From $P(a)$(for arbitrary    | If it's true for an        |
| Generalization   | a), infer                    | arbitrary case, it's true  |
| (UG)**           | $\forall x\text{ }P(x)$      | for all.                   |
+------------------+------------------------------+----------------------------+
| **Existential    |   --                         | If something exists, we    |
| Instantiation    |                              | can name one example.      |
| (EI)**           |   --                         |                            |
|                  |                              |                            |
|                  |   -------------------------- |                            |
|                  |   From                       |                            |
|                  |   $\exists x\text{ }P(x)$,   |                            |
|                  |   infer $P(a)$               |                            |
|                  |   -------------------------- |                            |
|                  |                              |                            |
|                  |   -------------------------- |                            |
+------------------+------------------------------+----------------------------+
| **Existential    | From $P(a)$, infer           | If it's true for a         |
| Generalization   | $\exists x\text{ }P(x)$      | specific thing, something  |
| (EG)**           |                              | like it exists.            |
+------------------+------------------------------+----------------------------+

**The main logical forms (for conditional statements/ implication).**

**Original (Conditional statement):** "If P then Q" Symbolically:
$P \Rightarrow Q$

(For comparison)

**Converse:** "If Q then P" Symbolically: $Q \Rightarrow P$

(Swap hypothesis and conclusion)

**Inverse:** "If not P, then not Q" Symbolically:
$\neg P \Rightarrow \neg Q$

(Negates both parts)

**Contrapositive:** "If not Q, then, not P" Symbolically:
$\neg P \Rightarrow \neg Q$

(Negates and swaps both parts)

**Contradiction:** [Negate the entire conclusion.]{.underline} Not a
proof form but technique

You assume the entire statement you want to prove is false, and show
this lead to an impossible situation.

  -----------------------------------------------------------------------------
  **Type of        **What you assume**    **What you     **What you conclude**
  Proof**                                 manipulate**   
  ---------------- ---------------------- -------------- ----------------------
  Direct proof     The hypothesis (the    That           The conclusion ("then"
                   "if" part)             assumption     part)

  Contradiction    The negation of what   That false     The original statement
                   you want to prove      assumption     is true

  Contrapositive   Assume the negation of Work from that Conclude the negation
                   the conclusion                        of the hypothesis
  -----------------------------------------------------------------------------

**Proof by cases:** When you divide a problem into distinct scenarios
(cases) and prove the statement holds true for each one. If all cases
are covered and the statement is true in each, the overall proof is
valid.

**Without loss of generality (WLOG):** is used in mathematical proofs to
narrow the scope of a proof to one special case in situations when the
proof can be easily adapted to apply a general case.

**[Counting]{.underline}**

You have 6 pairs of pants and 10 shirts. An outfit consists of a pair of
pants and a shirt.\
How many different outfits does this give?

*6 x 10 = 60 unique outfits*

**Enumerating:** listing out all elements of a set or a collection,
often in a specific order or for the purpose of counting.

Express the set of all outfits as 𝑂 = { P (𝑝, 𝑠) ∶ 𝑝 ∈ 𝑃, 𝑠 ∈ 𝑆 } ,
where 𝑃 is the set of 6 pairs of pants and 𝑆 is the set of 10 shirts.\
*Note that 𝑂 = 𝑃 × 𝑆, and so from set theory we have \|𝑂\| = \|𝑃 \|
\|𝑆\| = 60.*

Suppose you need to pick a password that has length 6-8 characters,
where each character is an uppercase letter. How many possible passwords
are there?

*26^6^ + 26^7^ + 26^8^*

How many license plates can be made which. Start with 2 or 3 uppercase
letters. Then have 2 or 3 digits from 0-9?

*26^2^ + 26^3^ + 10^2^ + 10^3^*

In a race with 20 runners there are trophies for 1st, 2nd, 3rd place.
The podium is defined\
by who wins each of the three trophies. How many different podiums are
possible?

*20 \* 19 \* 18*
