---
title: Cryptography
---
# Public-Key Cryptosystems

## Okamoto-Uchiyama

The Okamoto-Uchiyama cryptosystem is homomorphic and malleable.
cryptosystem.

1.  Choose random primes $p$ and $q$
2.  Compute $n=p^2q$
3.  Choose $g\in\{2\ldots n-1\}$ such that
    $g^{p-1} \not\equiv 1\bmod p^2$
4.  Compute $h=g^n\bmod n$

### Encryption

1.  Choose message $m<p$
2.  Chose integer $r\in\{1\ldots n-1\}$ at random
3.  Compute ciphertext $c=g^mh^r\bmod n$

### Decryption

1.  Define $L(x)=\frac{x-1}{p}$
2.  $m=\frac{L(c^{p-1}\bmod p^2)}{L(g^{p-1}\bmod p^2)}\bmod p$

## RSA

Rivest-Shamir-Adleman

1.  Choose random primes $p$ and $q$
2.  Compute $n=pq$
3.  Compute [Euler\'s totient](algo.org::*Euler's Totient Function) of
    $n$, $\varphi(n)=(p-1)(q-1)$
4.  Choose $e$ such that $1<e<\varphi(n)$
5.  Compute $d$ such that $de \equiv 1\bmod \varphi(n)$
6.  Choose message $m$
7.  Compute ciphertext $c\equiv m^e \bmod n$
8.  $m\equiv c^d \bmod n$

# Symmetric-Key Cryptosystems

Symmetric cryptosystems are malleable.

## Stream Ciphers

Stream ciphers often produce correlated ciphertext. The initialization
vector used must be random and unique to prevent

### CTR

Counter mode

Counter mode is a method of using a block cipher as a stream cipher.

### RC4

Rivest Cipher 4

## Block Ciphers

### AES

Advanced Encryption Standard

### DES

Data Encryption Standard

# Hash Functions

## SHA

Secure Hash Algorithm
