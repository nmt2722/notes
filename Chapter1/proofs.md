## Methods of Proof
In arithmetic and mathematics in general, there are several methods to prove or verify statements. Some of the most common methods of proof, using simple examples are presented below:-.

### 1. **Direct Proof**

A **direct proof** is when we show that a statement is true by directly using definitions, facts, and known theorems. This is the most straightforward method, where we start with the given information and logically deduce the result.

#### Example:
Let's prove that the sum of two even numbers is always even.

- **Statement**: If \(a\) and \(b\) are even numbers, then \(a + b\) is also even.
  
- **Proof**: 
  - By definition, an even number is any number that can be written as \(2k\), where \(k\) is an integer.
  - So, let \(a = 2k\) and \(b = 2m\), where \(k\) and \(m\) are integers.
  - Now, add \(a\) and \(b\):
    \[
    a + b = 2k + 2m = 2(k + m)
    \]
  - Since \(k + m\) is an integer, the sum \(a + b\) is a multiple of 2, which means it is even.
  - Hence, the sum of two even numbers is even.

### 2. **Proof by Contradiction**

In a **proof by contradiction**, we assume that the opposite of what we are trying to prove is true. Then, we show that this assumption leads to a contradiction (something that doesn’t make sense). This contradiction means that the original statement must be true.

#### Example:
Let's prove that \(\sqrt{2}\) is irrational (it cannot be expressed as a fraction of two integers).

- **Statement**: \(\sqrt{2}\) is irrational.
  
- **Proof by Contradiction**:
  - Assume, for the sake of contradiction, that \(\sqrt{2}\) is rational. This means \(\sqrt{2} = \frac{p}{q}\), where \(p\) and \(q\) are integers with no common factors (i.e., \(\frac{p}{q}\) is in its simplest form).
  - Now, square both sides:
    \[
    2 = \frac{p^2}{q^2}
    \]
    Multiply both sides by \(q^2\) to get rid of the denominator:
    \[
    2q^2 = p^2
    \]
  - This shows that \(p^2\) is an even number because it's two times something. So, \(p\) must also be even (because the square of an odd number is odd).
  - Let \(p = 2k\) for some integer \(k\).
  - Substitute \(p = 2k\) into the equation:
    \[
    2q^2 = (2k)^2 = 4k^2
    \]
    Divide both sides by 2:
    \[
    q^2 = 2k^2
    \]
  - This shows that \(q^2\) is also even, which means \(q\) must be even.
  - But we initially assumed that \(p\) and \(q\) had no common factors, but now we know both are even, meaning they share a factor of 2. This is a contradiction.
  - Therefore, our assumption that \(\sqrt{2}\) is rational must be false, and \(\sqrt{2}\) is irrational.

### 3. **Proof by Induction**

**Mathematical induction** is a method of proving statements that are usually formulated for all integers greater than or equal to a certain number. The idea is to prove the base case and then show that if the statement holds for one number, it holds for the next one.

#### Example:
Let's prove that the sum of the first \(n\) odd numbers is \(n^2\).

- **Statement**: The sum of the first \(n\) odd numbers is \(n^2\). In other words, 
  \[
  1 + 3 + 5 + \dots + (2n - 1) = n^2
  \]

- **Proof by Induction**:

  - **Step 1: Base Case** (n = 1)
    - When \(n = 1\), the sum of the first \(n\) odd numbers is just \(1\). And \(1^2 = 1\), so the base case holds.
  
  - **Step 2: Inductive Step**
    - Assume that the formula holds for some integer \(k\), i.e.,
      \[
      1 + 3 + 5 + \dots + (2k - 1) = k^2
      \]
    - Now, we need to prove that the formula also holds for \(k + 1\), i.e., we need to show that
      \[
      1 + 3 + 5 + \dots + (2k - 1) + (2(k+1) - 1) = (k+1)^2
      \]
    - By the inductive hypothesis, we know that
      \[
      1 + 3 + 5 + \dots + (2k - 1) = k^2
      \]
    - So, we add the next odd number, \(2(k+1) - 1 = 2k + 1\), to both sides:
      \[
      k^2 + (2k + 1) = (k+1)^2
      \]
    - Simplifying the right-hand side:
      \[
      k^2 + 2k + 1 = (k+1)^2
      \]
    - This is exactly what we needed to prove.
  
  - Since the base case holds, and the inductive step holds, the formula is true for all positive integers \(n\).

### 4. **Proof by Exhaustion**

In **proof by exhaustion**, we prove a statement by checking every possible case. This method is usually used when there are only a limited number of cases to check.

#### Example:
Let's prove that the sum of any two numbers, one even and one odd, is odd.

- **Statement**: The sum of an even number and an odd number is always odd.

- **Proof by Exhaustion**:
  - We know that an even number can be written as \(2k\), where \(k\) is an integer.
  - An odd number can be written as \(2m + 1\), where \(m\) is an integer.
  - There are two cases to consider:
    - Case 1: If we add an even number \(2k\) and an odd number \(2m + 1\):
      \[
      2k + (2m + 1) = 2(k + m) + 1
      \]
      This is of the form \(2n + 1\), which is odd.
    - Case 2: If we add an odd number \(2m + 1\) and an even number \(2k\), we get:
      \[
      (2m + 1) + 2k = 2(m + k) + 1
      \]
      This is also of the form \(2n + 1\), which is odd.
  - In both cases, the sum is odd. Thus, the statement is true.

### Summary

- **Direct Proof**: Show the statement is true using definitions and logical steps.
- **Proof by Contradiction**: Assume the opposite of what we want to prove, and show it leads to a contradiction.
- **Proof by Induction**: Prove a statement for a base case, then show that if it holds for \(n\), it holds for \(n + 1\).
- **Proof by Exhaustion**: Check all possible cases and prove the statement for each case.

These methods help mathematicians establish the truth of statements and are widely used in arithmetic and other areas of math!

### When to use what method

Each proof method is most useful in different scenarios. Here’s a breakdown of where each proof method is typically applied, with examples to help you understand when to use them:

### 1. **Direct Proof**
- **When to use it**: When the statement you're proving can be logically deduced directly from definitions, axioms (basic truths), or known theorems without any need to assume the opposite or use multiple cases.
  
- **Typical Scenarios**:
  - Proving basic properties, like the sum or product of certain types of numbers.
  - Verifying properties of numbers, such as even and odd numbers, prime numbers, or divisibility.

- **Example**: Proving the sum of two even numbers is even (as we saw earlier). This is a direct proof because we just used the definition of even numbers and showed that adding two even numbers results in another even number.

---

### 2. **Proof by Contradiction**
- **When to use it**: When proving something by directly assuming the opposite of what you're trying to prove leads to a contradiction. This method is often useful for proving statements about existence or irrationality.

- **Typical Scenarios**:
  - Proving that a number is irrational (like \(\sqrt{2}\)).
  - Proving that no solutions exist for certain equations (e.g., showing that an equation has no integer solutions).
  - Proving that certain assumptions lead to logical contradictions.

- **Example**: Proving that \(\sqrt{2}\) is irrational. We assume it’s rational and show that this assumption leads to a contradiction (i.e., we find that both \(p\) and \(q\) must be even, which violates the assumption that they have no common factors).

---

### 3. **Proof by Induction**
- **When to use it**: When the statement involves all integers greater than or equal to a certain number (usually positive integers). Induction is great for proving formulas or properties that work for an infinite number of cases.

- **Typical Scenarios**:
  - Proving formulas for sums or products of numbers, like the sum of the first \(n\) odd numbers or the sum of integers.
  - Proving divisibility statements for all integers.
  - Establishing inequalities that hold for all numbers in a certain set.

- **Example**: Proving that the sum of the first \(n\) odd numbers is equal to \(n^2\). In this case, induction allows us to show that if the formula holds for one number, it holds for the next number, and therefore, it holds for all numbers.

---

### 4. **Proof by Exhaustion**
- **When to use it**: When there are a small, finite number of possibilities to check, so you can prove each case individually. This method is useful when you can easily list all cases.

- **Typical Scenarios**:
  - Proving something for small values of \(n\) (like \(n = 1, 2, 3\), etc.).
  - Verifying a statement for all possible combinations or small cases.
  - Checking the validity of a condition for all specific cases (such as properties for numbers with a limited number of factors).

- **Example**: Proving that the sum of an even number and an odd number is always odd. Since there are only two cases (adding an even number to an odd one or vice versa), we can check both cases and confirm the result.

---

### **Summary of Where to Use Each Method**

- **Direct Proof**: Use it when you can logically deduce the result from known facts.
  - Example: Proving \(a + b\) is even if both \(a\) and \(b\) are even.
  
- **Proof by Contradiction**: Use it when assuming the opposite of the statement leads to a contradiction, especially for irrationality or non-existence problems.
  - Example: Proving \(\sqrt{2}\) is irrational.
  
- **Proof by Induction**: Use it for statements involving all integers or for mathematical formulas that hold for all natural numbers.
  - Example: Proving a formula for the sum of the first \(n\) odd numbers.
  
- **Proof by Exhaustion**: Use it when there are only a limited number of cases to check and you can easily verify each one.
  - Example: Proving the sum of an even and odd number is odd by checking both cases.

Each proof method has its own strengths and is suited for different types of problems, depending on the structure and nature of the statement you're trying to prove!

When it comes to proving a number is **irrational**, **proof by contradiction** is the most commonly used method, but it is not the only method. However, other methods are usually quite specific or less commonly used for this purpose. Let’s explore these methods in more detail!

### 1. **Proof by Contradiction (The Most Common Method)**

The **proof by contradiction** method is the standard and most effective way to prove that a number is irrational. The basic idea is to **assume** that the number is **rational**, and then show that this assumption leads to a contradiction. Here's how this works:

#### General Process:
1. **Assume** the number is rational. That is, assume it can be written as a fraction \(\frac{p}{q}\), where \(p\) and \(q\) are integers with no common factors (i.e., the fraction is in simplest form).
2. **Derive a contradiction** from this assumption, usually by manipulating the equation in such a way that you end up with a result that contradicts known properties (e.g., the assumption that the numbers have no common factors or that certain values must be integers).
3. **Conclude that the assumption is false**, meaning the number **cannot be rational**, and therefore, it must be **irrational**.

#### Example: Proving \(\sqrt{2}\) is irrational

- **Assume** \(\sqrt{2}\) is rational. So, \(\sqrt{2} = \frac{p}{q}\), where \(p\) and \(q\) are integers with no common factors (in simplest form).
- **Square both sides** to get: \(2 = \frac{p^2}{q^2}\).
- **Multiply both sides by \(q^2\)**: \(2q^2 = p^2\).
- Now, \(p^2\) is even (since it's 2 times something), so \(p\) must also be even.
- Let \(p = 2k\), where \(k\) is an integer.
- Substitute \(p = 2k\) into \(2q^2 = p^2\), getting \(2q^2 = (2k)^2 = 4k^2\).
- Simplify: \(q^2 = 2k^2\), so \(q^2\) is even, meaning \(q\) must also be even.
- But if both \(p\) and \(q\) are even, they share a factor of 2, which contradicts the assumption that \(\frac{p}{q}\) is in simplest form.
- Therefore, \(\sqrt{2}\) **cannot** be rational, so it is **irrational**.

This proof by contradiction is the most common approach because it is both simple and powerful.

---

### 2. **Algebraic Proofs (Using Algebraic Properties)**

Although **proof by contradiction** is the most common method, there are some situations where **algebraic manipulation** (or number-theoretic properties) can directly show irrationality, particularly in special cases.

#### Example: Proving \(\sqrt{3}\) is irrational (directly using algebraic properties)

1. **Assume** \(\sqrt{3}\) is rational, so it can be written as \(\frac{p}{q}\) where \(p\) and \(q\) are integers with no common factors.
2. **Square both sides**: \(3 = \frac{p^2}{q^2}\).
3. Multiply both sides by \(q^2\): \(3q^2 = p^2\).
4. The right-hand side of the equation is \(p^2\), which means it’s a multiple of 3. This implies that **\(p\) itself must be divisible by 3**.
5. Let \(p = 3k\) for some integer \(k\).
6. Substitute \(p = 3k\) into the equation: 
   \[
   3q^2 = (3k)^2 = 9k^2
   \]
   Simplify: \(q^2 = 3k^2\).
7. This shows that \(q^2\) is divisible by 3, meaning \(q\) must also be divisible by 3.
8. But if both \(p\) and \(q\) are divisible by 3, they share a common factor of 3, which contradicts the assumption that \(\frac{p}{q}\) is in simplest form.
9. Thus, \(\sqrt{3}\) **cannot** be rational, so it is **irrational**.

This is another example where algebraic reasoning can show irrationality, and although it's similar to a proof by contradiction, it's a more direct approach because it avoids using the assumption that leads to a full contradiction. However, this is still fundamentally a **contradiction** method, even if we don't frame it in those terms.

---

### 3. **Using Decimal Expansions (Rare)**

Another way to show a number is irrational is by proving that its decimal expansion is non-repeating and non-terminating. If the decimal form of a number does not repeat or terminate, the number cannot be expressed as a fraction, and therefore, it is irrational.

#### Example: Proving \(\pi\) is irrational (via decimal expansion)

- The decimal expansion of \(\pi\) starts as \(3.14159265358979\ldots\) and continues without repeating or terminating.
- Since rational numbers have decimal expansions that either terminate or eventually repeat, the non-repeating, non-terminating nature of \(\pi\)'s decimal expansion shows that \(\pi\) is irrational.
  
However, **proving irrationality via decimal expansions** is more theoretical and often harder to apply directly without an understanding of advanced techniques in real analysis.

---

### 4. **Using Properties of Algebraic Numbers (Advanced)**

Another advanced approach, often used in higher mathematics (like Galois theory or algebraic number theory), involves classifying numbers as **algebraic** or **transcendental**:

- **Algebraic numbers** are numbers that are roots of polynomials with integer coefficients. A number that is **not algebraic** is called **transcendental**.
- If we can show that a number is not a root of any polynomial with integer coefficients, then it must be transcendental and, therefore, irrational.
  
For example, **\(\pi\) and \(e\)** (Euler's number) are transcendental numbers and thus irrational. But proving that a number is transcendental requires advanced tools beyond basic algebra and is not typically done by high school-level students.

---

### Conclusion

- **Proof by contradiction** is by far the most common and efficient method for proving that a number is irrational, particularly for numbers like \(\sqrt{2}\), \(\sqrt{3}\), and others.
- **Algebraic approaches** (like showing divisibility or using properties of squares) can also be used, but they still often rely on a form of contradiction.
- **Decimal expansion** and **transcendental number theory** are more advanced and less commonly used for basic proofs in arithmetic but can be helpful in certain cases.

So while **contradiction** is the go-to method for irrationality, other methods exist, especially when dealing with more complex or transcendental numbers.
