---
title: Algorithms
---
# Modulo Function

-   Written as % or $\mod x$

The modulo function is the equivalent of taking the remainder of two
numbers.

## Modular Equivalence

A common way to express modular equivalence by a number $n$ is
$x\equiv y\pmod
  n$

# Greatest Common Divisor

-   Written as $gcd(x,y)$

The greatest common divisor of two or more integers is the largest
positive integer that divides each of the integers.

# Least Common Multiple

-   Written as $lcm(x,y)$

# Euler\'s Totient Function

-   A.k.a. Euler\'s phi function
-   Written as $\varphi(n)$ or $\phi(n)$

Euler\'s totient function returns the number of positive integers less
than $n$ that are [*relatively prime*]{.spurious-link
target="Greatest Common Divisor"} to $n$.

$\varphi(n)$ is the number of $k\in\mathbb{N}$ such that $k\le n$ and
$gcd(k,n)=1$.

# Carmichael\'s Totient Function

-   A.k.a. the reduced totient function or the least universal exponent
    function
-   Written as $\lambda(n)$

Carmichael\'s totient function returns the exponent of the
multiplicative group of positive integers modulo $n$.

For every $a\in\mathbb{N}$, $\lambda(n)$ is the smallest
$m\in\mathbb{N}$ such that $a^m\equiv1\bmod n$, $a\le n$, and
$gcd(a,n)= 1$
