# Exercise 1
Prove that the language $L_1 = \{ab^nc^n\ |\ n ≥ 0\}$ is nonregular.

1. Pick some p
2. $w = ab^pc^p$
3. Pick $x, y, z$ s.t. $w = xyz\ y ≠ ε\ |xy|\ ≤ p$
4. Since the amount b's and c's have to be equal, and $xy$ consists of atleast one a and $p$ b's picking $i=0$ result in the removal of atleast one b.

# Exercise 2
Prove that the language $L_2 = \{0^n1^m0^n\ |\ n, m ≥ 0\}$ is nonregular.

1. Pick some p
2. $w=0^p10^p$
3. Pick $x, y, z$ s.t. $w = xyz\ y ≠ ε\ |xy|\ ≤ p$
4. Since the 0's either side of the 1 has to be of equal amount and $y ≠ ε$ picking $i=0$ result in the removal of atleast one 0.

# Exercise 3
Prove that the language $L_3 = \{a^nb^m\ |\ n, m ≥ 0$ and $n\ ≠ m\}$ is nonregular.

This language can be simplfied under the complement and intersection closures.

$\overline{L_3} ∩ L(a^∗b^∗) = {a^nb^n | n ≥ 0}$

Now we can prove by contradiction, if we assume that $L_3$ is regular then so must $\overline{L_3}$ also be, which we know it is not regular.

# Exercise 4
Prove that the language $L_4 = \{a^ib^jc^k\ |\ i, j, k ≥ 0$ and if $i = 1$  then $j = k\}$ is nonregular.

This can be proven in the same way as exercise 3

$L_4 ∩ L(ab^∗c^∗) = {ab^nc^n | n ≥ 0}$