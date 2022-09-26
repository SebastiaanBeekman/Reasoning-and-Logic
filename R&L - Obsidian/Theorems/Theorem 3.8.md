# Theorem 3.8
$\sum^n_{i=1}i2^i-1 = (n - 1) * 2^n + 1$ for any natural number n > 0.

**Proof**. Let P(n) be the statement $\sum^n_{i=1}i2^i-1 = (n - 1) * 2^n + 1$. We use induction
to show that P(n) is true for all n > 0.
**Base case**: Consider the case n = 1. P(1) is the statement that $\sum^1_{i=1}i2^i-1 = (1 - 1) * 2^1 + 1$. Sinse each side of this equiation is equal to one, this is true.
**Inductive case**: Let k $\geq$ 1 be arbitrary, and assume that P(k) is true. We want to show that P(k + 1) is true. P(k + 1) is the statement $\sum^{k+1}_{i=1}i2^i-1 = ((k + 1) - 1) * 2^{k+1} + 1$. But, we can compute that
![[Pasted image 20220925151934.png]]
which is what we wanted to show. This completes the induction.