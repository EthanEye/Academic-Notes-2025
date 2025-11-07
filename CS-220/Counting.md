# Counting 9.1

**You have 6 pairs of pants and 10 shirts. An outfit consists of a pair of
pants and a shirt.
How many different outfits does this give?**

>6 x 10 = 60 unique outfits

**<ins>Enumerating:</ins>** listing out all elements of a set or a collection,
often in a specific order or for the purpose of counting.

## **<ins>Product rule:</ins>**

**A burrito stand sells burritos with different choices of stuffing. The set of choices for each category are:**

>Filling choices {chicken,beef,pork}
>Bean choices {black,pinto}
>Salsa choices {mild,medium,hot}

**Formal Product Rule:**

$$
\text{If } A \text{ and } B \text{ are independent events, then: } \\
P(A \cap B) = P(A) \times P(B)
$$

**If every burrito has a filling, beans, and salsa, then how many possible burrito combinations are there?**
> 3 x 2 x 3 = 18

**Express the set of all outfits as 𝑂 = { P (𝑝, 𝑠) ∶ 𝑝 ∈ 𝑃, 𝑠 ∈ 𝑆 } ,
where 𝑃 is the set of 6 pairs of pants and 𝑆 is the set of 10 shirts.
Note that 𝑂 = 𝑃 × 𝑆, and so from set theory we have 𝑂 = 𝑃**
>𝑆 = 60.

**Suppose you need to pick a password that has length 6-8 characters,
where each character is an uppercase letter. How many possible passwords
are there?**

>26^6 + 26^7 + 26^8

**How many license plates can be made which. Start with 2 or 3 uppercase
letters. Then have 2 or 3 digits from 0-9**

>26^2 + 26^3 + 10^2 + 10^3

In a race with 20 runners there are trophies for 1st, 2nd, 3rd place.
The podium is defined by who wins each of the three trophies. How many different podiums are
possible**

>20  19  18

**<ins>Σ (Sigma):</ins>** In set theory and formal language theory Sigma is used to represent an alphabet,
which is a finite set of symbols.

>Σ^n is the set of all string of length n containing characters that come from the set >Σ. For example, if Σ = {1,0}, then Σ^6 is the set of all binary strings with 6 bits.
>The product rule can also be used to determine the number of strings in a set of a >specific combination. 9.1.2

**How many six bit binary strings begin with "01"?**
>{0} x {1} x {0,1}^4 = 1 x 1 x 2^4 = 16 Σ = {0,1}

**How strings of length 4 are there over the alphabet {a,b,c}**
> {a,b,c}^4 = 81

## **<ins>The sum rule:</ins>** 

**The sum rule is applied when multiple choices are available but only one selection is made.**

Ex: A customer just orders a drink. The customer selects a hot drink or a cold drink. The hot drink selections are {coffe, hot cocoa, tea}. The cold drink selections are {milk, orange juice}. The total number of choices = 5, 3 hot drink choices plus 2 cold drink choices.

**Formal Sum Rule:**

$$\text{If } A_1, A_2, \dots, A_k \text{ are mutually exclusive events, then: } \\
P(A_1 \cup A_2 \cup \dots \cup A_k) = P(A_1) + P(A_2) + \dots + P(A_k)$$

**Sum & product rule:**

>Ex: Laptop customization choices:
>Screen Size: {14in, 15in, 17in}
>Processor Speed: {2.0 GHz, 2.7 Ghz}
>Storage: SSD OR HDD
>SSD - {126G, 256G, 512G}
>HDD - {256G, 512G}

>> Laptop selection = 3 x 2 (3 + 2)
