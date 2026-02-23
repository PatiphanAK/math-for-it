# Vector Spaces

Vector spaces are one of the most fundamental structures in mathematics. They appear in Linear Algebra, Machine Learning, Physics, Computer Graphics, Signal Processing, and many other fields.

---

# 1. What is a Vector Space?

A **vector space** is a set equipped with two operations:

1. Vector addition
2. Scalar multiplication

These operations must satisfy specific rules (called axioms). Formally:

Let $V$ be a set and $F$ be a **field** (such as $\mathbb{R}$ or $\mathbb{C}$). We say that $V$ is a **vector space over $F$** if:

$$+ : V \times V \to V$$

$$\cdot : F \times V \to V$$

and the following properties hold.

---

# 2. The Axioms of a Vector Space

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

---

# 3. Standard Examples

## Example 1: $\mathbb{R}^n$

$$\mathbb{R}^n = \{ (x_1, x_2, \ldots, x_n) \mid x_i \in \mathbb{R} \}$$

**Addition:**

$$(x_1, \ldots, x_n) + (y_1, \ldots, y_n) = (x_1 + y_1, \ldots, x_n + y_n)$$

**Scalar multiplication:**

$$a(x_1, \ldots, x_n) = (ax_1, \ldots, ax_n)$$

This is the most familiar vector space.

---

## Example 2: Polynomial Space

Let $P_n(\mathbb{R})$ be the set of all polynomials of degree $\leq n$. Example:

$$p(x) = a_0 + a_1 x + a_2 x^2$$

Addition and scalar multiplication are defined normally. This is also a vector space.

---

## Example 3: Function Space

Let

$$V = \{ f : \mathbb{R} \to \mathbb{R} \}$$

Define:

$$(f + g)(x) = f(x) + g(x)$$

$$(af)(x) = a \cdot f(x)$$

This is an infinite-dimensional vector space.

---

# 4. Important Insight

A vector space is **NOT** just $\mathbb{R}^n$. It is any structure where:

- You can add elements
- You can multiply them by scalars
- The axioms hold

Vectors do not have to be arrows. They can be:

- Polynomials
- Functions
- Signals
- Matrices
- Feature representations in neural networks

---

# 5. Why This Matters

Vector spaces give us:

- Linear combinations
- Basis
- Dimension
- Linear transformations
- Eigenvalues
- Orthogonality
- Projection

All of Linear Algebra depends on this structure. Machine learning models operate in vector spaces. Neural network feature embeddings live in vector spaces. Signal processing uses vector spaces of functions. Understanding this definition deeply makes everything else easier.

---

# 6. Summary

A vector space over a field $F$ is a set $V$ with:

- Addition
- Scalar multiplication
- Satisfying 8 axioms

$$(V, +, \cdot)$$

If the axioms hold, you have a vector space. If not, you don't. Everything else in linear algebra builds from here.
