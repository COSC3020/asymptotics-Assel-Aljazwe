[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/tk_2Q3XR)
# The O, Omega, and Theta

Each row in the table below specifies two functions $f(n)$ and $g(n)$.
Fill in the *number* from this list that best describes their relationship:

1. $f(n)\in O(g(n))$, but $f(n)\not \in \Omega(g(n))$
1. $f(n)\in \Omega(g(n))$, but $f(n)\not \in O(g(n))$
1. $f(n)\not\in O(g(n))$, and $f(n)\not \in \Omega(g(n))$
1. $f(n)\in \Theta (g(n))$

I have done the first one for you, as an example.

| $f(n)=\ldots$              | compared to | $g(n)=\ldots$          |
|----------------------------|:-----------:|------------------------|
| $f(n)=n$                   | 1           | $g(n)=2n^2 + n$        |      // f(n) gorws slower than g(n) and will never overtake it.
| $f(n)= 10n + 3\log_{15} n$ | 4           | $g(n)= 4n - 2\log_2 n$ |      // both functions are linearly dependent on n, hence they are in big theta (g(n))
| $f(n) = 2n^5$              | 2            | $g(n) = 5n^2$          |     // f(n) grows much faster than g(n) due to its higher power of n.
| $f(n)=\log_{10} \left(n^{10}\right)$ | 1  | $g(n)=n$ |                   //  After simplification, we find that f(n) grows slower than g(n)
| $f(n)= 4n^5 $ | 2  | $g(n)= 5n^4$ |                                      // f(n) grows faster due to the higher power of n 
| $f(n) = 10^{256}$ | 1  | $g(n) = \log n$ |                               // f(n) is a constant that doesn't grow, meanwhile g(n) grows very slowly. So f(n) is both big O and big Omega but not big theta of g(n)
| $f(n)= n^2 $ | 1  | $g(n)= 2^n$ |                                        // f(n) grows polynomially, meanwhile g(n) grows exponentially.
