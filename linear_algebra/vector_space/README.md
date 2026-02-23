# Vector Spaces

Vector spaces are one of the most fundamental structures in mathematics.
They appear in:

- Linear Algebra
- Machine Learning
- Physics
- Computer Graphics
- Signal Processing

Understanding vector spaces clearly makes everything in linear algebra much easier.

---

## 0. A Quick Review of Sets

Before defining vector spaces, we recall the idea of a **set**.

In mathematics, a set is a collection of elements defined within a formal system (usually based on axioms such as ZFC set theory).

Examples:

- The set of natural numbers

$$\mathbb{N} = \{1,2,3,4,5,\ldots\}$$

- The set of real numbers

$$\mathbb{R}$$

- The set of complex numbers

$$\mathbb{C}$$

---

> **⚠️ Imaginary Numbers**
>
> The complex number system introduces the imaginary unit
>
> $$i = \sqrt{-1}$$
>
> so that
>
> $$\mathbb{C} = \{ a + bi \mid a, b \in \mathbb{R} \}$$

---

## <img src="badges/sec1.svg" alt="1. What is a Vector Space?" height="40"/>

A **vector space** is a set equipped with two operations:

1. Vector addition
2. Scalar multiplication

These operations must satisfy specific rules (called axioms).

---

### Formal Definition

Let $V$ be a set and let $F$ be a **field** (such as $\mathbb{R}$ or $\mathbb{C}$).

We say that $V$ is a **vector space over $F$** if:

$$+ : V \times V \to V$$

$$\cdot : F \times V \to V$$

and the following axioms hold.

---

## 2. The Axioms of a Vector Space

<details>
<summary>Click to expand all 8 axioms</summary>

For all $u, v, w \in V$ and all scalars $a, b \in F$:

### (1) Associativity of Addition

$$(u + v) + w = u + (v + w)$$

### (2) Commutativity of Addition

$$u + v = v + u$$

### (3) Existence of Zero Vector

There exists a vector $\mathbf{0} \in V$ such that:

$$v + \mathbf{0} = v$$

### (4) Existence of Additive Inverse

For each $v \in V$, there exists $-v$ such that:

$$v + (-v) = \mathbf{0}$$

### (5) Compatibility of Scalar Multiplication

$$a(bv) = (ab)v$$

### (6) Identity Element of Scalar Multiplication

$$1 \cdot v = v$$

### (7) Distributivity Over Vector Addition

$$a(u + v) = au + av$$

### (8) Distributivity Over Scalar Addition

$$(a + b)v = av + bv$$

If all these properties hold, then $V$ is a vector space.

</details>

---

Standard Examples

### Example 1: $\mathbb{R}^n$

$$\mathbb{R}^n = \{ (x_1, x_2, \ldots, x_n) \mid x_i \in \mathbb{R} \}$$

**Addition**

$$(x_1, \ldots, x_n) + (y_1, \ldots, y_n) = (x_1 + y_1, \ldots, x_n + y_n)$$

**Scalar multiplication**

$$a(x_1, \ldots, x_n) = (ax_1, \ldots, ax_n)$$

This is the most familiar finite-dimensional vector space.

---

### Example 2: Polynomial Space

Let $P_n(\mathbb{R})$ be the set of all polynomials of degree $\leq n$.

Example:

$$p(x) = a_0 + a_1 x + a_2 x^2$$

Addition and scalar multiplication are defined coefficient-wise. This is also a vector space.

---

### Example 3: Function Space

Let

$$V = \{ f : \mathbb{R} \to \mathbb{R} \}$$

Define:

$$(f + g)(x) = f(x) + g(x)$$

$$(af)(x) = a \cdot f(x)$$

This is an infinite-dimensional vector space.

---

4. Important Insight"

A vector space is **not just** $\mathbb{R}^n$.

It is any structure where:

- Addition is defined
- Scalar multiplication is defined
- The axioms are satisfied

Vectors do not have to be arrows. They can be:

- Polynomials
- Functions
- Signals
- Matrices
- Feature representations in neural networks

---

5. Why This Matters

Vector spaces allow us to define:

- Linear combinations
- Basis
- Dimension
- Linear transformations
- Eigenvalues
- Orthogonality
- Projection

All of linear algebra is built on this structure.

Machine learning models operate in vector spaces.
Neural network embeddings live in vector spaces.
Signal processing studies vector spaces of functions.

---

6. Summary

A vector space over a field $F$ is a set $V$ equipped with:

- Addition
- Scalar multiplication
- The eight axioms

We often denote this structure as:

$$(V, +, \cdot)$$

If the axioms hold, you have a vector space. Everything else in linear algebra builds from here.
