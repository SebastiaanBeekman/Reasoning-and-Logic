# Proof by Contradiction
Suppose that we start with some set of assumptions and apply rules of logic to derive a sequence of statements that can be proved from those assumptions, and suppose that we derive a statement that we know to be false. When the laws of logic are applied to true statements, the statements that are derived will also be true. If we derive a false statement by applying rules of logic to a set of assumptions, then at least one of the assumptions must be false. This observation leads to a powerful proof technique, which is known as [[proof by contradiction]].

Suppose that you want to prove some proposition, *p*. To apply proof by
contradiction, assume that $\neg$*p* is true, and apply the rules of logic to derive
conclusions based on this assumption. If it is possible to derive a statement
that is known to be false, it follows that the assumption, $\neg$*p*, must be false. (Of course, if the derivation is based on several assumptions, then you only know that at least *one* of the assumptions must be false.) The fact that $\neg$*p* is
false proves that *p* is true. Essentially, you are arguing that *p* must be true,
because if it weren’t, then some statement that is known to be false could be proved to be true. Generally, the false statement that is derived in a proof by contradiction is of the form *q* ∧ $\neg$*q*. This statement is a contradiction in the sense that it is false no matter what the value of *q*. Note that deriving the contradiction *q* ∧ $\neg$*q* is the same as showing that the two statements, *q* and $\neg$*q*, both follow from the assumption that $\neg$*p*.

As a first example of proof by contradiction, consider the following theorem:

### Theorem 3.1
The number $\sqrt{3}$ is irrational.

*Proof*. Proof by contradiction:
- Assume for the sake of contradiction that $\sqrt{3}$ is rational
- Then $\sqrt{3}$ can be written as the ratio of two integers, $\sqrt{3}$ = $\frac{m′}{n′}$ for some integers *m*′ and *n*′.
- Furthermore, the fraction $\frac{m′}{n′}$ can be reduced to lowest terms by canceling all common factors of m′ and n′. So $\sqrt{3}$ = $\frac{m}{n}$ for some integers m and n which have no common factors.
- Squaring both sides of this equation gives 3 = $\frac{m^2}{n^2}$ and re-arranging gives 
  3$n^2$ = $m^2$.
- From this equation we see that $m^2$ is divisible by 3. Therefore m is divisible by 3 and we can write m = 3k for some integer k.
- Substituting m = 3k into the last equation above gives 3$n^2$ = $(3k)^2$ or $3n^2$ = $9k^2$, which in turn becomes $n^2$ = $3k^2$. From this we see that $n^2$ is divisible by 3, and again we know that this implies that n is divisible by 3.
- But now we have (i) m and n have no common factors, and (ii) m and n have a common factor, namely 3. It is impossible for both these things to be true, yet our argument has been logically correct.
- Therefore our original assumption, namely that $\sqrt{3}$ is rational, must be incorrect.
- Therefore $\sqrt{3}$ must be irrational.

One of the oldest mathematical proofs, which goes all the way back to Euclid, is a [[proof by contradiction]]. Recall that a prime number is an integer *n*, greater than 1, such that the only positive integers that evenly divide *n* are 1 and *n*. We will show that there are infinitely many primes. Before we get to the theorem, we need a [[lemma]]. 

### Lemma 3.2
If *N* is an integer and *N* > 1, then there is a prime number which evenly divides *N*.

*Proof*. Let *D* be the smallest integer which is greater than 1 and which evenly divides *N*. (*D* exists since there is at least one number, namely *N* itself, which is greater than 1 and which evenly divides *N*. We use the fact that any non-empty subset of *N* has a smallest member.) We claim that *D* is prime, so that *D* is a prime number that evenly divides *N*.

Suppose that *D* is not prime. We show that this assumption leads to a [[contradiction]]. Since *D* is not prime, then, by definition, there is a number *k* between 2 and *D* − 1, inclusive, such that *k* evenly divides *D*. But since *D* evenly divides *N*, we also have that *k* evenly divides *N*. That is, *k* is an integer greater than one which evenly divides *N*. But since *k* is less than *D*, this contradicts the fact that *D* is the smallest such number. This contradiction proves that *D* is a prime number.

### Theorem 3.3
There are infinitely many prime numbers.

*Proof*. Suppose that there are only finitely many prime numbers. We will show that this assumption leads to a contradiction.

Let *p1*, *p2*, …, *pn* be a complete list of all prime numbers (which exists under the assumption that there are only finitely many prime numbers). Consider the number *N* obtained by multiplying all the prime numbers together and adding one. That is,
<center>N = (p1 · p2 · p3 · · · pn) + 1</center>

Now, since *N* is larger than any of the prime numbers *px*, and since 
*p1*, *p2*, …, *pn* is a complete list of prime numbers, we know that *N* cannot be prime. By the [[lemma]], there is a prime number *p* which evenly divides *N*. Now, *p* must be one of the numbers *p1*, *p2*, …, *pn*. But in fact, none of these numbers evenly divides *N*, since dividing *N* by any *px* leaves a remainder of 1. This contradiction proves that the assumption that there are only finitely many primes is false.