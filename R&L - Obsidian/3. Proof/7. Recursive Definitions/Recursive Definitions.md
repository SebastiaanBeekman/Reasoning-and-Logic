# Recursive Definitions
Recursion occurs in programming when a subroutine is (partially) defined in terms of itself. But recursion also occurs outside of programming. A [[recursive definition]] is a definition that includes a reference to the term that is being defined. A recursive definition defines something at least partially in terms of itself. As in the case of recursive subroutines, mathematical induction can often be used to prove facts about things that are defined recursively.

As we already noted, there is a recursive definition for n!, for n in $\mathbb{N}$, and we can use this definition to prove facts about the factorials. We can define 0! = 1 and n! = n · (n − 1)! for n > 0. Do you see how the base case and the inductive case in an inductive proof can correspond to the two parts of the recursive definition?

Other sequences of numbers can also be defined recursively. For example, the famous Fibonacci sequence is the sequence of numbers $f_0$, $f_1$, $f_2$, …, defined recursively by
$$f_0 = 0$$
$$f_1 = 1$$
$$f_n = f_{n-1} + f_{n-2}$$
Using this definition, we compute that
$$f_2 = f_1 + f_0 = 0 + 1 = 1$$$$f3 = f_2 + f_1 = 1 + 1 = 2$$$$f4 = f3 + f_2 = 2 + 1 = 3$$$$f5 = f4 + f3 = 3 + 2 = 5$$$$f6 = f5 + f4 = 5 + 3 = 8$$$$f7 = f6 + f5 = 8 + 5 = 13$$
and so on. Based on this definition, we can use induction to prove facts about the Fibonacci sequence. We can prove, for example, that $f_n$ grows exponentially with n, even without finding an exact formula for $f_n$:

### Theorem 3.13
The Fibonacci sequence, $f_0$, $f_1$, $f_2$, …, satisfies $f_n$ > $\frac{3}{2}^{n−1}$, for n $\geq$ 6.

**Proof**. 
We prove this by induction on n. For n = 6, we have that $f_n$ = 8 while $1.5^{n−1}$ = $1.5^5$, which is about 7.6. So $f_n$ $\gt$ $1.5^{n−1}$ for n = 6. Similarly, for n = 7, we have $f_n$ = 13 and $1.5^{n−1}$ = $1.5^6$, which is about 11.4. So $f_n$ > $1.5^{n−1}$ for n = 7.

Now suppose that k is an arbitrary integer with k > 7. Suppose that we already know that fn > 1.5n−1 for n = k − 1 and for n = k − 2. We want to show that the inequality then holds for n = k as well. But
![[Pasted image 20220926131623.png]]
This string of equalities and inequalities shows that fk > $1.5^{k−1}$. This completes the induction and proves the theorem.