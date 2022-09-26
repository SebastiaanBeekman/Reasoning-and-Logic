# Examples
### Example 1
We set out to prove that the sum of any two rational numbers is rational.

*Proof*. We start by assuming that x and y are arbitrary rational numbers.
Here’s a formal proof that the inference rule
- x is rational
- y is rational
- $\therefore$ x + y is rational

is a valid rule of interence:
![[Pasted image 20220919175224.png]]
![[Pasted image 20220919175242.png]]
So the rule of inference given above is valid. Since x and y are arbitrary
rationals, we have proved that the rule is valid for all rationals, and hence
the sum of any two rationals is rational.

Again, a more informal presentation that we expect from you during the
course would look like:

*Proof*. [[proof by generalisation|Proof by generalisation]]:
- Let *x* and *y* be arbitrary rational numbers
- By the definition of rational, there are integers *a*, *b* $\neq$ 0, *c*, *d* $\neq$ 0 such that *x* = $\frac{a}{b}$ and *y* = $\frac{c}{d}$
- Then x + y = $\frac{ad + bc}{bd}$;
- We know *ad* + *bc* and *bd* are integers since the sum and product of integers are integers, and we also know *bd* $\neq$ 0 since neither *b* nor *d* is 0
- So we have written x + y as the ratio of two integers, the denominator being non-zero
- Therefore, by the definition of rational numbers, x + y is rational
- Since x and y were arbitrary rationals, the sum of any two rationals is rational

### Example 2
we will prove that any 4-digit number wxyz is divisible by 3 [[iff]] the sum of the four digits is divisible by 3.

*Proof*. This statement is of the form p ↔ q; recall that p ↔ q is logically equivalent to (p → q) ∧ (q → p). So we need to prove for any 4-digit number wxyz that (1) if wxyz is divisible by 3 then w + x + y + z is divisible by 3, and (2) if w + x + y + z is divisible by 3 then wxyz is divisible by 3. So let wxyz be an arbitrary 4-digit number.

(1) Assume wxyz is divisible by 3, i.e., wxyz = 3k for some integer k. The number wxyz is actually w ×1000+x ×100+y ×10+z, so we have the equation
<center>w × 1000 + x × 100 + y × 10 + z = 3k</center>
Since 1000 = 999 + 1, 100 = 99 + 1, and 10 = 9 + 1, this equation can be rewritten
<center>999w + w + 99x + x + 9y + y + z = 3k</center>
Rearranging gives
<center>w + x + y + z = 3k − 999w − 99x − 9y</center>
<center>= 3k − 3(333w) − 3(33x) − 3(3y)</center>
We can now factor a 3 from the right side to get
<center>w + x + y + z = 3(k − 333w − 33x − y)</center>
Since (k − 333w − 33x − y) is an integer, we have shown that w + x + y + z is divisible by 3.

(2) Assume w + x + y + z is divisible by 3. Consider the number wxyz. As remarked above,
<center>wxyz = w × 1000 + x × 100 + y × 10 + z</center>
so
<center>wxyz = 999w + w + 99x + x + 9y + y + z</center>
<center>= 999w + 99x + 9y + (w + x + y + z)</center>
We assumed that w + x + y + z = 3k for some integer k, so we can substitute into the last equation to get
<center>wxyz = 999w + 99x + 9y + 3k = 3(333w + 33x + 3y + k)</center>
Since the quantity in parentheses is an integer, we have proved that wxyz is divisible by 3.

In (1) and (2) above, the number wxyz was an arbitrary 4-digit integer, so we have proved that for all 4-digit integers, wxyz is divisible by 3 [[iff]] the sum of the four digits is divisible by 3.


### Example 3
Now suppose we wanted to prove the statement “For all integers n, $n^2$ is even if and only if n is even.” We have already proved half of this statement
(“For all integers n, if n is even then $n^2$ is even”), so all we need to do is prove the statement “For all integers n, if $n^2$ is even then n is even” and we’ll be done. Unfortunately, this is not as straightforward as it seems: suppose we started in our standard manner and let n be an arbitrary integer and assumed that $n^2$ = 2k for some integer k. Then we’d be stuck! Taking the square root of both sides would give us n on the left but would leave a $\sqrt{2k}$ on the right. This quantity is not of the form 2k′ for any integer k′; multiplying it by $\frac{\sqrt{2}}{\sqrt{2}}$ would give 2$\frac{\sqrt{k}}{\sqrt{2}}$ but there is no way for us to prove that $\frac{\sqrt{k}}{\sqrt{2}}$ is an integer. So we’ve hit a dead end. What do we do now?

The answer is that we need a different proof technique. The proofs we have written so far are what are called [[direct proofs]]: to prove p → q you assume p is true and prove that the truth of q follows. Sometimes, when a direct proof of p → q fails, an [[indirect proof]] will work. Recall that the [[contrapositive]] of the implication p → q is the implication $\neg$q → $\neg$p, and that this proposition is logically equivalent to p → q. An indirect proof of p → q, then, is a direct proof of the contrapositive $\neg$q → $\neg$p. In our current example, instead of proving “if $n^2$ is even then n is even” directly, we can prove its contrapositive “if n is not even (i.e., n is odd) then $n^2$ is not even (i.e., $n^2$ is odd)”. We call this method a [[proof by contrapositive]]. 

Alternatively we sometimes need a [[proof by division into cases]]. Consider for instance that we want to prove that 3 | (n3 + 3n2 + 2n) for all integers n. What we can do is split our proof into three different case based on the divisibility by 3. Recall from the definition of divisibility that every number can be written as either n = 3k, n = 3k + 1, or n = 3k + 2. In a proof by division into cases, we prove that the claim holds for all of these cases and thereby prove the claim holds for all numbers.