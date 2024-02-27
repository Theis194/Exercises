# Exercise 1
Prove that the language $L_1 = \{ab^nc^n\ |\ n ≥ 0\}$ is nonregular.

1. Pick some p
2. $w = ab^pc^p$
3. Pick $x, y, z$ s.t. $w = xyz\ y ≠ ε\ |xy|\ ≤ p$
4. Since the amount b's and c's have to be equal, and $xy$ consists of atleast one a and $p$ b's picking $i=0$ result in the removal of atleast one b.

# Exercise 2
Prove that the language $L_2 = \{0^n1^m0^n\ |\ n, m ≥ 0\}$ is nonregular.

1. Pick some p
2. $w=0^p1^10^p$
3. Pick $x, y, z$ s.t. $w = xyz\ y ≠ ε\ |xy|\ ≤ p$
4. Since the 0's either side of the 1 has to be of equal amount and $y ≠ ε$ picking $i=0$ result in the removal of atleast one 0.

# Exercise 3
Prove that the language $L_3 = \{a^nb^m\ |\ n, m ≥ 0$ and $n\ ≠ m\}$ is nonregular.

1. Pick some p
2. $w=a^pb^{2p}$
3. Pick $x, y, z$ s.t. $w = xyz\ y ≠ ε\ |xy|\ ≤ p$
4. Since the amount of a and b cannot be equal, and $xy$ only can contain a's, choosing $i=2$ would result in $a^{2p}$ equalling the amount of b's.

# Exercise 4
Prove that the language $L_4 = \{a^ib^jc^k\ |\ i, j, k ≥ 0$ and if $i = 1$  then $j = k\}$ is nonregular.

1. Pick some p
2. $w=a^1b^pc^p$
3. Pick $x, y, z$ s.t. $w = xyz\ y ≠ ε\ |xy|\ ≤ p$
4. Picking $i=2$ would result in a larger amount of b's than c's, or putting an a after the first set of b's.
