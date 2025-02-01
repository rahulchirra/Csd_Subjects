# Comprehensive Tutorial on Mathematics & Statistics Topics

## Unit I: Greatest Common Divisors, Prime Factorization, and Congruences

### 1.1 Greatest Common Divisors (GCD)
**Definition**: The GCD of two integers \( a \) and \( b \) is the largest integer that divides both \( a \) and \( b \).  
**Example**: GCD(12, 18) = 6.  
**Properties**:
- If \( d = \text{GCD}(a, b) \), then \( d \mid a \) and \( d \mid b \).
- \( \text{GCD}(a, b) = \text{GCD}(b, a \mod b) \).

---

### 1.2 Euclidean Algorithm
**Step-by-Step Process**:
1. Divide \( a \) by \( b \), get remainder \( r \).
2. Replace \( a \) with \( b \), \( b \) with \( r \).
3. Repeat until \( b = 0 \). The GCD is \( a \).  

**Example**:
- Find GCD(1071, 462):
  - 1071 ÷ 462 = 2, remainder 147
  - 462 ÷ 147 = 3, remainder 21
  - 147 ÷ 21 = 7, remainder 0 → **GCD = 21**.

---

### 1.3 Fundamental Theorem of Arithmetic
Every integer \( > 1 \) can be represented uniquely (up to order) as a product of primes.  
**Example**: \( 60 = 2^2 \times 3 \times 5 \).  
**Proof Sketch**: Use induction and contradiction to show existence and uniqueness.

---

### 1.4 Congruences
**Definition**: \( a \equiv b \mod m \) if \( m \mid (a - b) \).  
**Properties**:
- Reflexive, symmetric, transitive.
- If \( a \equiv b \mod m \), then \( a + c \equiv b + c \mod m \).

---

#### 1.4.1 Linear Congruences
Solve \( ax \equiv b \mod m \).  
**Solution**: Find modular inverse of \( a \) mod \( m \) if \( \text{GCD}(a, m) = 1 \).  
**Example**: Solve \( 3x \equiv 4 \mod 7 \):  
- \( 3^{-1} \mod 7 = 5 \) (since \( 3 \times 5 = 15 \equiv 1 \mod 7 \)).  
- \( x \equiv 4 \times 5 \mod 7 \equiv 20 \mod 7 \equiv 6 \).

---

### 1.5 Chinese Remainder Theorem (CRT)
If \( m_1, m_2, ..., m_k \) are pairwise coprime, the system:
\[
\begin{cases}
x \equiv a_1 \mod m_1 \\
x \equiv a_2 \mod m_2 \\
\vdots \\
x \equiv a_k \mod m_k
\end{cases}
\]
has a unique solution modulo \( M = m_1 \times m_2 \times ... \times m_k \).  
**Example**: Solve \( x \equiv 2 \mod 3 \), \( x \equiv 3 \mod 5 \):  
- \( M = 15 \), \( x = 8 \).

---

## Unit II: Simple Linear Regression & Probability Distributions

### 2.1 Simple Linear Regression
**Model**: \( Y = \beta_0 + \beta_1 X + \epsilon \).  
**Goal**: Estimate \( \beta_0 \) (intercept) and \( \beta_1 \) (slope).  
**Least Squares Method**:
\[
\hat{\beta}_1 = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sum (x_i - \bar{x})^2}, \quad \hat{\beta}_0 = \bar{y} - \hat{\beta}_1 \bar{x}
\]

---

### 2.2 Hypothesis Testing for Regression Coefficients
**Test for \( \beta_1 \)**:
- \( H_0: \beta_1 = 0 \) (no linear relationship).
- Test statistic: \( t = \frac{\hat{\beta}_1}{\text{SE}(\hat{\beta}_1)} \).

---

### 2.3 Discrete Probability Distributions
**Binomial Distribution**:  
PMF: \( P(X = k) = \binom{n}{k} p^k (1-p)^{n-k} \).  
**Poisson Distribution**:  
PMF: \( P(X = k) = \frac{e^{-\lambda} \lambda^k}{k!} \).

---

## Unit III: Continuous Distributions & Sampling

### 3.1 Normal Distribution
**PDF**: \( f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}} \).  
**Standard Normal (Z)**: \( \mu = 0 \), \( \sigma = 1 \).  
**Empirical Rule**: 68-95-99.7% within 1-2-3σ.

---

### 3.2 Central Limit Theorem (CLT)
If \( X_1, X_2, ..., X_n \) are iid with mean \( \mu \) and variance \( \sigma^2 \), then:
\[
\frac{\bar{X} - \mu}{\sigma/\sqrt{n}} \xrightarrow{d} N(0, 1)
\]
**Application**: Confidence intervals for population mean.

---

## Unit IV: Estimation & Hypothesis Testing

### 4.1 Maximum Likelihood Estimation (MLE)
**Steps**:
1. Write likelihood function \( L(\theta) \).
2. Take logarithm to get \( \ell(\theta) \).
3. Differentiate and solve for \( \theta \).

**Example**: MLE for \( \lambda \) in Poisson: \( \hat{\lambda} = \bar{X} \).

---

### 4.2 Hypothesis Testing for Proportions
**Z-test for proportion**:  
Test statistic: \( Z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}} \).

---

## Unit V: Stochastic Processes & Markov Chains

### 5.1 Markov Chains
**Definition**: A stochastic process where future states depend only on the present state.  
**Transition Matrix**: \( P = [p_{ij}] \), where \( p_{ij} = P(X_{n+1}=j \mid X_n=i) \).  
**Steady-State**: Solve \( \pi P = \pi \) with \( \sum \pi_i = 1 \).

---

### 5.2 Example: Weather Model
**States**: {Sunny, Rainy}.  
**Transition Matrix**:
\[
P = \begin{bmatrix}
0.8 & 0.2 \\
0.3 & 0.7
\end{bmatrix}
\]
**Steady-State Equations**:
\[
0.8\pi_1 + 0.3\pi_2 = \pi_1 \\
0.2\pi_1 + 0.7\pi_2 = \pi_2 \\
\pi_1 + \pi_2 = 1
\]
**Solution**: \( \pi_1 = 0.6 \), \( \pi_2 = 0.4 \).

---

# Summary & Exercises
**Key Takeaways**:
- GCD and CRT are foundational in number theory.
- Regression and distributions form the basis of statistical modeling.
- Markov chains model memoryless stochastic processes.

**Exercises**:
1. Compute GCD(270, 192) using the Euclidean algorithm.
2. Solve \( 5x \equiv 3 \mod 11 \).
3. Derive the MLE for \( \lambda \) in an exponential distribution.
