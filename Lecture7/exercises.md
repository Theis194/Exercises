# Pumping lemma for context-free languages

## Ecercise 1

Consider the following three languages over the alphabet $Σ = \{a, b, c\}$

- $L_1 = \{ a^ib^jc^k\ |\ i, j, k ≥ 0,\ i = j ≤ k\}$

  1. Pick some p
  2. $w = a^pb^pc^p$
  3. Pick $u, v, x, y, z$ such that $w = uvxyz,\ vy ≠ ε$ and $|vxy| ≤ p$
  4. Case 1
     1. $vy$ only contains c's, $uv^0xy^0z$ then $i,j>k$
     1. $vy$ contains both b's and c's, $uv^0xy^0z$ would result in $i≠j$ and $k<i$
     1. $vy$ does contains a's, $uv^ixy^iz$ for $i≥2$ would result in $i,j>k$

- $L_2 = \{a^ib^jc^k\ |\ i, j, k ≥ 0,\ i = j\}$

  1. $L_2 \cap L(a^*b^*)=\{a^nb^n|n≥0\}$ this language, as seen in lecture 06 is recognized by a PDA, making it context-free.

- $L_3 = \{a^ib^jc^k\ |\ i, j, k ≥ 0,\ j ≤ k\}$
  1. $L_3 \cap L(b^*c^*)=\{b^nc^m\ |\ n,m≥0,\ n≤m\}$ this language, as seen in lecture 05 can be recognized in example 1 on slide 17, replacing 0's for b's, 1's for c's, and ≥ with ≤, making it context-free.

Which of the above languages is context-free and which is not? Justify your answer by providing formal proofs of your claims. (Hint: only two of the above are context-free)

## Exercise 2

Consider the language

$L_4 = \{u\#w\ |\ u, w ∈ \{0, 1\}∗, u$ is a prefix of $w\}$

is $L_4$ context-free? Justify your answer by providing a formal proof of your claim.

Since no minimum length is provided, $w=10$ is possible a word recognized by $L_4$ where $u=\epsilon$ and $w=10$.

## Exercise 3

Here is a wrong attempt to show that a language is not context-free.

Consider the language

- $L5 = \{uu | u ∈ {a, b}∗\}$

We use the pumping lemma to show that $L_5$ is not context-free. Choose $w = aabbaabb$. So we can split it into $u = aa$, $v = b$, $x = baa$, $y = bb$ and $z = ε$. But then we have that $uv^2xy^2z \notin L_5$

result = aabbbaabbbb

Explain the main reasons why the above attempt of proof is wrong.

It only considers one case of u, v, x, y, and z. The case where $v=bb$ and $x=aa$ would be recognized by $L_5$.
