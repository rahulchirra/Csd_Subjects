# 📝 Mathematics & Statistics Class Notes  
**For B.Tech Students**  
*Units I-V | Definitions, Theorems, Handwritten-Style Problems*  

---

## **UNIT I: Greatest Common Divisors & Congruences**  

### **1. Greatest Common Divisors (GCD)**  
**Definition**:  
- The largest integer that divides two integers without leaving a remainder.  
- **Notation**: GCD(a, b).  

**Example**:  
- Find GCD(48, 18):  
  - Divisors of 48: 1, 2, 3, 4, 6, 8, 12, 16, 24, 48  
  - Divisors of 18: 1, 2, 3, 6, 9, 18  
  - Common divisors: 1, 2, 3, 6 → **GCD = 6**.  

**Euclidean Algorithm**:  
- *Step 1*: Divide 48 by 18 → Quotient = 2, Remainder = 12  
- *Step 2*: Divide 18 by 12 → Quotient = 1, Remainder = 6  
- *Step 3*: Divide 12 by 6 → Remainder = 0  
- **GCD = 6**.  

---

### **2. Fundamental Theorem of Arithmetic**  
**Definition**:  
- Every integer >1 can be expressed **uniquely** as a product of prime numbers.  

**Example**:  
- Prime factorization of 120:
120 → 2 × 60 → 2 × 2 × 30 → 2 × 2 × 2 × 15 → 2³ × 3 × 5.

markdown
---

### **3. Congruences**  
**Definition**:  
- \( a ≡ b \mod m \) if \( m \) divides \( (a - b) \).  

**Linear Congruence**:  
- Solve \( 3x ≡ 6 \mod 9 \):  
- Simplify: \( x ≡ 2 \mod 3 \).  
- Solutions: \( x = 2, 5, 8, 11, ... \).  

**Chinese Remainder Theorem**:  
- Solve:
x ≡ 2 mod 3
x ≡ 3 mod 5

markdown
- *Step 1*: Let \( x = 3k + 2 \).  
- *Step 2*: Substitute into 2nd congruence:  
\( 3k + 2 ≡ 3 mod 5 → 3k ≡ 1 mod 5 → k ≡ 2 mod 5 \).  
- *Step 3*: \( k = 5m + 2 → x = 3(5m + 2) + 2 = 15m + 8 \).  
- **Smallest positive solution**: \( x = 8 \).  

---

### **4. Practice Problems (Unit I)**  
1. **Problem (GCD)**: Use the Euclidean algorithm to find GCD(270, 192).  
 **Solution**:  
 - 270 ÷ 192 = 1, Remainder = 78  
 - 192 ÷ 78 = 2, Remainder = 36  
 - 78 ÷ 36 = 2, Remainder = 6  
 - 36 ÷ 6 = 6, Remainder = 0 → **GCD = 6**.  

2. **Problem (Congruence)**: Solve \( 5x ≡ 10 \mod 15 \).  
 **Solution**:  
 - Divide by 5: \( x ≡ 2 mod 3 \).  
 - Solutions: \( x = 2, 5, 8, 11, ... \).  

---

## **UNIT II: Simple Linear Regression & Probability**  

### **1. Simple Linear Regression Model**  
**Definition**:  
- \( y = \beta_0 + \beta_1 x + \epsilon \), where:  
- \( \beta_0 \): Intercept.  
- \( \beta_1 \): Slope.  
- \( \epsilon \): Error term.  

**Least Squares Method**:  
- Minimize \( \sum (y_i - \hat{y}_i)^2 \).  

**Formula**:  
- \( \beta_1 = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sum (x_i - \bar{x})^2} \)  
- \( \beta_0 = \bar{y} - \beta_1 \bar{x} \).  

**Example**:  
| Hours Studied (x) | Marks (y) |  
|--------------------|-----------|  
| 1                  | 40        |  
| 2                  | 50        |  
| 3                  | 70        |  

- \( \bar{x} = 2 \), \( \bar{y} = 53.33 \).  
- Calculations:  
- \( \sum (x_i - \bar{x})(y_i - \bar{y}) = (1-2)(40-53.33) + (2-2)(50-53.33) + (3-2)(70-53.33) = 13.33 + 0 + 16.67 = 30 \).  
- \( \sum (x_i - \bar{x})^2 = 1 + 0 + 1 = 2 \).  
- \( \beta_1 = 30 / 2 = 15 \).  
- \( \beta_0 = 53.33 - 15 \times 2 = 23.33 \).  
- **Regression Equation**: \( \hat{y} = 23.33 + 15x \).  

---

### **2. Random Variables & Distributions**  
**Discrete Random Variable**:  
- Takes countable values (e.g., number of heads in 3 coin tosses).  

**Continuous Random Variable**:  
- Takes uncountable values (e.g., height of students).  

**Binomial Distribution**:  
- **Definition**: \( P(X = k) = C(n, k) p^k (1-p)^{n-k} \).  
- **Example**: Probability of 2 heads in 3 tosses (p = 0.5):  
\( C(3, 2) (0.5)^2 (0.5)^1 = 3 × 0.25 × 0.5 = 0.375 \).  

**Normal Distribution**:  
- **Z-Score**: \( Z = \frac{X - \mu}{\sigma} \).  
- **Example**: If \( \mu = 100 \), \( \sigma = 15 \), find \( P(X ≤ 115) \):  
\( Z = (115 - 100)/15 = 1 → P(Z ≤ 1) = 0.8413 \).  

---

### **3. Practice Problems (Unit II)**  
1. **Problem (Regression)**: For the example above, predict marks if \( x = 4 \).  
 **Solution**: \( \hat{y} = 23.33 + 15(4) = 83.33 \).  

2. **Problem (Binomial)**: Find \( P(X = 3) \) for \( n = 5 \), \( p = 0.4 \).  
 **Solution**: \( C(5, 3)(0.4)^3(0.6)^2 = 10 × 0.064 × 0.36 = 0.2304 \).  

---

## **UNIT III: Normal Distribution & Sampling**  

### **1. Central Limit Theorem (CLT)**  
**Definition**:  
- When sampling from any distribution with mean \( \mu \) and variance \( \sigma^2 \), the sample mean (\( \bar{X} \)) follows a normal distribution for large \( n \).  

**Example**:  
- Population: [1, 2, 3, 4, 5] (μ = 3, σ = 1.58).  
- Take samples of size 2:  
- Sample 1: (1, 3) → Mean = 2.  
- Sample 2: (2, 5) → Mean = 3.5.  
- Sample 3: (3, 4) → Mean = 3.5.  
- **Distribution of means** will approximate normality.  

---

### **2. Sampling Distribution of Means**  
**Formula**:  
- \( \bar{X} \sim N\left(\mu, \frac{\sigma}{\sqrt{n}}\right) \).  

**Example**:  
- Population: \( \mu = 50 \), \( \sigma = 10 \).  
- For \( n = 25 \): \( \sigma_{\bar{X}} = 10 / \sqrt{25} = 2 \).  
- **Probability** \( P(48 ≤ \bar{X} ≤ 52) = P(-1 ≤ Z ≤ 1) = 0.6826 \).  

---

### **3. Practice Problems (Unit III)**  
1. **Problem (CLT)**: A population has \( \mu = 80 \), \( \sigma = 12 \). Find \( P(\bar{X} ≤ 82) \) for \( n = 36 \).  
 **Solution**:  
 - \( \sigma_{\bar{X}} = 12 / 6 = 2 \).  
 - \( Z = (82 - 80)/2 = 1 → P(Z ≤ 1) = 0.8413 \).  

---

## **UNIT IV: Hypothesis Testing**  

### **1. Z-Test for Single Mean**  
**Steps**:  
1. **Null Hypothesis (\( H_0 \))**: \( \mu = \mu_0 \).  
2. **Alternate Hypothesis (\( H_1 \))**: \( \mu ≠ \mu_0 \).  
3. **Test Statistic**:  
 \( Z = \frac{\bar{X} - \mu_0}{\sigma / \sqrt{n}} \).  
4. **Decision**: Reject \( H_0 \) if |Z| > Z-critical.  

**Example**:  
- \( H_0: \mu = 100 \), \( \bar{X} = 105 \), \( \sigma = 15 \), \( n = 30 \).  
- \( Z = \frac{105 - 100}{15 / \sqrt{30}} = 1.825 \).  
- **Z-critical** (α = 0.05): ±1.96 → **Fail to reject \( H_0 \)**.  

---

### **2. Practice Problems (Unit IV)**  
1. **Problem (Z-test)**: Test \( H_0: \mu = 50 \) vs \( H_1: \mu > 50 \) with \( \bar{X} = 52 \), \( \sigma = 5 \), \( n = 25 \).  
 **Solution**:  
 - \( Z = (52 - 50) / (5/5) = 2 \).  
 - **Z-critical** (α = 0.05) = 1.645 → **Reject \( H_0 \)**.  

---

## **UNIT V: Stochastic Processes**  

### **1. Markov Chains**  
**Definition**:  
- A stochastic process where the future state depends only on the present state.  

**Transition Matrix**:  
- Example (Weather):  
\[
P = \begin{bmatrix}
0.7 & 0.3 \\  # Sunny → Sunny: 70%, Rainy: 30%  
0.5 & 0.5 \\  # Rainy → Sunny: 50%, Rainy: 50%  
\end{bmatrix}
\]  

**Steady-State Probabilities**:  
- Solve \( \pi P = \pi \):  
- Let \( \pi = [\pi_1, \pi_2] \).  
- Equations:  
  \( 0.7\pi_1 + 0.5\pi_2 = \pi_1 \)  
  \( 0.3\pi_1 + 0.5\pi_2 = \pi_2 \)  
- Solve: \( \pi_1 = \frac{5}{8} \), \( \pi_2 = \frac{3}{8} \).  

---

### **2. Practice Problems (Unit V)**  
1. **Problem**: If today is 60% Sunny, predict tomorrow’s weather.  
 **Solution**:  
 - Sunny: \( 0.6 \times 0.7 + 0.4 \times 0.5 = 62\% \).  
 - Rainy: \( 38\% \).  

---

## **📚 Handwritten-Style Problem Sheet (All Units)**  

### **Unit I**  
**Problem 1**: Find GCD(270, 192).  
**Solution**:
270 = 192 × 1 + 78
192 = 78 × 2 + 36
78 = 36 × 2 + 6
36 = 6 × 6 + 0 → GCD = 6 ✔️

markdown
---

**Problem 2**: Solve \( x ≡ 3 \mod 7 \) and \( x ≡ 4 \mod 9 \).  
**Solution**:
Let x = 7k + 3 → Substitute into 2nd congruence:
7k + 3 ≡ 4 mod 9 → 7k ≡ 1 mod 9 → k ≡ 4 mod 9 (since 7×4=28 ≡1 mod 9).
Thus, x = 7(9m + 4) + 3 = 63m + 31.
Smallest positive solution: x = 31. ✔️

markdown
---

### **Unit II**  
**Problem**: For \( \hat{y} = 10 + 2x \), predict \( y \) at \( x = 3 \).  
**Solution**:
y = 10 + 2(3) = 16 ✔️

markdown
---

**Need more problems or corrections? Let me know!** 🎯
This version provides:
✅ Full definitions for all terms.
✅ Handwritten-style problem solving with step-by-step breakdowns.
✅ Complete coverage of all topics in your original list.
✅ Exam-ready practice problems.
