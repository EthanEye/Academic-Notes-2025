# Propositions & Predicates

## Number sets:

**[Natural numbers (ℕ)] -- Counting numbers (1, 2, 3, 4...)**

**[Integers (ℤ)] -- All whole numbers including zero (-3, -2, -1, 0, 1, 2, 3...)**

**[Rational numbers (ℚ)] -- Numbers that can be written as fraction a,b ∈ ℤ, b ≠ 0 (1/2, -3, 0.25, 7...)**

**[Real numbers (ℝ)] -- All rational and irrational numbers (-5, 0, 2.5, √2, π)**

### Propositions: A statement that can be true or false but not both. We can represent these with propositional variables.**

| Variable | Meaning | Truth value |
|----------|---------|-------------|
| *p*      | "It is raining" | T or F |
| *q*      | "It is cold"    | T or F |
| *r*      | "I will stay inside" | T or F |

## Logical Operators

| **Operator**      | **Name**           | **Symbol**       | **Example**   | **Meaning**                                      |
|-------------------|--------------------|------------------|--------------|--------------------------------------------------|
| **Negation**      | NOT               | ¬ or ~          | ¬p           | "It is **not** raining."                        |
| **Conjunction**   | AND               | ∧               | p ∧ q        | "It is raining **and** cold."                   |
| **Disjunction**   | OR                | ∨               | p ∨ q        | "It is raining **or** cold."                    |
| **Implication**   | IF...THEN         | ⇒ or →          | p → q        | "**If** it rains, **then** it is cold."         |
| **Biconditional** | IF AND ONLY IF    | ⇔               | p ⇔ q        | "It rains **if and only if** it is cold."       |

### Predicates: are logical statements or expressions that contain oneor more variables and become a proposition when specific values areassigned to those variables.

**Ex: P(x): "x is greater than 5"**

**P(7): "7 is greater than 5" is true**

**P(3): "3 is greater than 5" is false**

## Rules of Inference

| **Rule Name**        | **Form**                                   | **Explanation**                                                                 |
|----------------------|-------------------------------------------|---------------------------------------------------------------------------------|
| **Modus Ponens**     | 1. P → Q <br> 2. P <br> ∴ Q              | If P implies Q, and P is true, then Q must be true.                            |
| **Modus Tollens**    | 1. P → Q <br> 2. ¬Q <br> ∴ ¬P            | If P implies Q, and Q is false, then P must be false.                          |
| **Hypothetical Syllogism** | 1. P → Q <br> 2. Q → R <br> ∴ P → R | If P implies Q and Q implies R, then P implies R.                              |
| **Disjunctive Syllogism** | 1. P ∨ Q <br> 2. ¬P <br> ∴ Q         | If either P or Q is true, and P is false, then Q must be true.                 |
| **Addition**         | 1. P <br> ∴ P ∨ Q                        | If P is true, then "P or Q" is also true (no matter what Q is).                |
| **Simplification**   | 1. P ∧ Q <br> ∴ P                        | If both P and Q are true, then P (or Q) individually is true.                  |
| **Conjunction**      | 1. P <br> 2. Q <br> ∴ P ∧ Q              | If P is true and Q is true, then "P and Q" is true.                            |
| **Resolution**       | 1. P ∨ Q <br> 2. ¬P ∨ R <br> ∴ Q ∨ R     | Used in propositional logic to eliminate variables (common in AI).             |

  ----------------------------------------------------------------------------------------
