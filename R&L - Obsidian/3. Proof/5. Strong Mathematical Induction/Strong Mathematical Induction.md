# Strong mathematical Induction
There is a second form of the principle of mathematical induction which is useful in some cases. To apply the first form of induction, we assume P(k) for an arbitrary natural number k and show that P(k +1) follows from that assumption. In the second form of induction, the assumption is that P(x) holds for all x between 0 and k inclusive, and we show that P(k+1) follows from this. This gives us a lot more to work with when deducing P(k + 1). We will need this second, stronger form of induction in the next two sections. A proof will be given in the next chapter.

### Theorem 3.9
Let P be a one-place predicate whose domain of discourse includes the natural numbers. Suppose that P(0) is true and that
$$(P(0) \wedge P(1) \wedge ... \wedge P(k)) \rightarrow P(k + 1)$$
is true for each natural number k $\geq$ 0. Then P(n) is true for every antural number n.

For example, we can use this theorem to prove that every integer greater than one can be written as a product of prime numbers (where a number that is itself prime is considered to be a product of one prime number). The proof illustrates an important point about applications of this theorem: When proving P(k + 1), you don’t necessarily have to use the assumptions that P(0), P(1), …, and P(k) are true. If P(k+1) is proved by any means, then the statement (P(0) $\wedge$ P(1) $\wedge$ · · · $\wedge$ P(k)) $\rightarrow$ P(k + 1) has been shown to be true. It follows from this observation that several numbers, not just zero, can be ‘base cases’ in the sense that P(x + 1) can be proved independently of P(0) through P(x). In this sense, 0, 1, and every prime number are base cases in the following theorem.

### Theorem 3.10
Every natural number greater than one can be written as a product of prime numbers.

**Proof**. 
Let P(n) be the statement “if n $\gt$ 1, then n can be written as a product of prime numbers”. We will prove that P(n) is true for all n by applying the second form of the principle of induction.

Note that P(0) and P(1) are both automatically true, since n = 0 and n = 1 do not satisfy the condition that n $\gt$ 1, and P(2) is true since 2 is the product of the single prime number 2. Suppose that k is an arbitrary natural number with k $\gt$ 1, and suppose that P(0), P(1), …, P(k) are already known to be true; we want to show that P(k + 1) is true. In the case where k + 1 is a prime number, then k + 1 is a product of one prime number, so P(k + 1) is true.

Consider the case where k+1 is not prime. Then, according to the definition of prime number, it is possible to write k + 1 = ab where a and b are numbers in the range from 2 to k inclusive. Since P(0) through P(k) are known to be true, a and b can each be written as a product of prime numbers. Since k +1 = ab, k +1 can also be written as a product of prime numbers. We have shown that P(k + 1) follows from P(0) $\wedge$ P(1) $\wedge$ · · · $\wedge$ P(k), and this completes the induction.