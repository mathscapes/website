---
layout      : post
title       : Prime Numbers as Building Blocks
author      : "Gaurav Singh"
tags        : PrimeNumbers
cite        : true
---

For as long as I remember, I always had a deep interest in prime numbers. And that's why -- this -- in an attempt to document its vast literature and carry out my research on this subject.

Prime Numbers are the building blocks of the numbers and perhaps the processes in the Universe, as I like to think. While it may seem simple to understand what are prime numbers, its startling to find their presence in unusual places. From the prime-numbered life span of Cicada to ensuring security on your credit card, it has profound value in both nature and applied science. 

> Mathematicians have tried in vain to this day to discover some order in the sequence of prime numbers, and we have reason to believe that it is a mystery into which the mind will never penetrate". -- Euler

**The fundamental theorem of arithmetic states that every positive integer has a unique prime factorization. This theorem is thus also referred as unique factorization theorem.**

The theorem states that the factors of a number can be expressed uniquely only with prime numbers or its factors. While a number may have composite factors, but the combination of such numbers cannot be unique.

For example,

$$ 234 = 2 \times 3^2 \times 13 $$

This theorem in fact, is the reason why some numbers are called Prime and also why 1 is not referred as a prime number, so to avoid non-unique combinations of factors.

_Prime makes the composite numbers. But, what are primes made up of? Are prime numbers the result of how we framed the rules of Maths to be? Or did it always existed?_

Well whether or not if they are real, it has irrespectively awakened my curiosity to study it and perhaps define a formula. How can something that appears simple and yet not understood entirely?

Now that being said, I’m sometimes put down by imagining the incredible literature available on the Prime numbers, which have been studied for more than 2000 years. The earliest surviving records come from the Ancient Egypt and dates back to 1550 BC! Imagine what could be possibly appealing about these numbers for the ancient Egyptians? What might have been their motivations?

Intrinsically, I looked for the hidden visual model but never could able to get past any existing research. It is incredibly distracting as it appears to follow an unknown rule. Prime numbers have indisputably kept me occupied for many years now. And with the computers we have now, it is probably going to be the very exciting era for mathematical research and a significant leap is not so far away.

> There are two facts about the distribution of prime numbers of which I hope to convince you so overwhelmingly that they will be permanently engraved in your hearts. The first is that, despite their simple definition and role as the building blocks of the natural numbers, the prime numbers grow like weeds among the natural numbers, seeming to obey no other law than that of chance, and nobody can predict where the next one will sprout. The second fact is even more astonishing, for it states just the opposite: that the prime numbers exhibit stunning regularity, that there are laws governing their behaviour, and that they obey these laws with almost military precision". -- D. Zagier at a lecture (1975)

I began looking at the sequence and what a fantastic puzzle this is! The distribution despite following a rule does not let us pinpoint the next occurrence of prime. Is Mathematics advance enough to write the solution? Or it will remain in the class of hard problems which cannot be otherwise solved by non-brute force approach.

_Any number either is prime or is measured by some prime number. -- Euclid, Elements Book VII, Proposition 32_

A **Prime number** is a positive integer $p\>1$ that has no positive integer divisors other than 1 and p itself. And a method for determining whether a number is prime or not is called as **Primality Test**. Other integers which are not Prime numbers are referred as **Composite numbers**.

$$ n = p_1^{n_1} . p_2^{n_2} \dots p_k^{n_k} = \prod_{i=1}^k p_i^{n_i} $$

where $p_i$ are unique prime numbers, $n_i$ are the powers of prime factors and $k$ is the number of such factors.

This form is called as **Canonical representation** of $n$.

Such representation can be yielded by trial division. For example 32 can be expressed as --

	2 32
	2 16
	2  8
	2  4
	2  2
	   1

$$ 32 = 2 \times 2 \times 2 \times 2 \times 2 = 2^5 $$

Alternatively, prime numbers can be also defined as the natural numbers greater than one that are not products of two smaller natural numbers.

If you look at it, any number except Prime numbers can be reduced to Prime numbers through the canonical form. This is why it makes sense to call Prime numbers as the building blocks, which can be used to construct other numbers. _And if so, can prime numbers be used to encode information optimally?_

These are some of the few questions that incited me to pursue this subject and eventually start Mathscapes Research.

<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax: {inlineMath:[['$','$']]}});</script>
<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=default' async></script>
