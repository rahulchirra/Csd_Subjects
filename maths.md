# 📖 Mathematics & Statistics for B.Tech Students  
**Units I–V Simplified with Examples, Visuals, and Code**  

---

## **Unit I: Number Theory & Congruences**  
### **1. Greatest Common Divisors (GCD)**  
#### **What is GCD?**  
- **Definition**: The largest integer that divides two numbers without a remainder.  
- **Example**: GCD of 18 and 24 = 6.  

#### **Euclidean Algorithm**  
**Step-by-Step Calculation**:  
1. Divide the larger number by the smaller:  
   - 48 ÷ 18 = 2 (Remainder = 12)  
2. Replace the larger number with the smaller and repeat:  
   - 18 ÷ 12 = 1 (Remainder = 6)  
3. Repeat until remainder = 0:  
   - 12 ÷ 6 = 2 (Remainder = 0) → **GCD = 6**.  

**Python Code**:  
def gcd(a, b):
    while b != 0:
        a, b = b, a % b
    return a
print(gcd(48, 18))  # Output: 6
2. Prime Factorization & Fermat Numbers
Fundamental Theorem of Arithmetic
Every number >1 can be uniquely written as a product of primes.
Example:
60 = 2² × 3 × 5.
Fermat Numbers
Formula: ( F_n = 2^{2^n} + 1 ).
Why they matter: Used in cryptography.
Example: ( F_2 = 2^{2^2} + 1 = 17 ) (Prime), but ( F_5 = 4,294,967,297 ) is not prime (Euler proved it’s divisible by 641).
3. Congruences & Chinese Remainder Theorem
Congruences Basics
( a ≡ b \mod m ) means ( (a - b) ) is divisible by ( m ).
Example: 17 ≡ 2 mod 5 because 17 - 2 = 15 (which is divisible by 5).
Chinese Remainder Theorem
Problem: Solve:

( x ≡ 2 \mod 3 )
( x ≡ 3 \mod 5 )
Solution:

List numbers ≡ 2 mod 3: 2, 5, 8, 11, 14, 17, 20...
Find the one ≡ 3 mod 5: 17 (since 17 ÷ 5 = 3 rem 2 → Wait, that's 17 ≡ 2 mod 5. Oops! Let me correct that.
Actually, 17 ÷ 5 = 3 rem 2, so 17 ≡ 2 mod 5. Let me pick another number. Let's try 8: 8 ÷ 5 = 1 rem 3 → 8 ≡ 3 mod 5. So x = 8.
4. Practice Problems (Unit I)
Find GCD(56, 98).
Solution: 14.
Solve: ( x ≡ 4 \mod 7 ) and ( x ≡ 5 \mod 9 ).
Solution: x = 32.
Unit II: Regression & Probability
1. Simple Linear Regression
Equation: ( y = \beta_0 + \beta_1 x + \epsilon ).
Steps to Find β₁ (Slope):

Calculate means ( \bar{x} ) and ( \bar{y} ).
Compute ( \beta_1 = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sum (x_i - \bar{x})^2} ).
Example:

Hours Studied (x)	Marks (y)
1	40
2	50
3	70
( \bar{x} = 2 ), ( \bar{y} = 53.33 ).
( \beta_1 = \frac{(1-2)(40-53.33) + (2-2)(50-53.33) + (3-2)(70-53.33)}{(1-2)^2 + (2-2)^2 + (3-2)^2} = \frac{26.66}{2} = 13.33 ).
( \beta_0 = 53.33 - 13.33(2) = 26.67 ).
Final Equation: ( \hat{y} = 26.67 + 13.33x ).
2. Probability Distributions
Binomial Distribution
Formula: ( P(X=k) = C(n, k) p^k (1-p)^{n-k} ).
Example: Probability of 3 heads in 5 coin tosses:
( P(X=3) = C(5,3) (0.5)^3 (0.5)^2 = 10 × 0.125 × 0.25 = 0.3125 ).
Normal Distribution
Z-Score Example: If μ = 100, σ = 15, find P(X ≤ 115).
( Z = \frac{115 - 100}{15} = 1 ).
From Z-table, P(Z ≤ 1) = 0.8413 → 84.13%.
3. Practice Problems (Unit II)
For the regression example above, predict marks if x = 4 hours.
Solution: ( \hat{y} = 26.67 + 13.33(4) = 80 ).
Unit III: Normal Distribution & Sampling
Central Limit Theorem (CLT)
Example:

Population: [1, 2, 3, 4, 5] (μ = 3, σ = 1.58).
Take samples of size 2 and compute their means:
Sample 1: (1, 3) → Mean = 2.
Sample 2: (2, 5) → Mean = 3.5.
CLT in Action: The distribution of sample means will approximate normality as sample size increases.
Unit IV: Hypothesis Testing
Z-Test Example
Problem: Test if a sample mean ( \bar{x} = 105 ), n = 30, σ = 15 differs from μ = 100 (α = 0.05).

( H_0: \mu = 100 ), ( H_1: \mu \neq 100 ).
Compute ( Z = \frac{105 - 100}{15/\sqrt{30}} = 1.825 ).
Critical Z-value = ±1.96.
Since 1.825 < 1.96, fail to reject H₀.
Unit V: Markov Chains
Transition Matrix Example
Weather Model:

Today: Sunny (S) or Rainy (R).
Transition Matrix:
[
P = \begin{bmatrix}
0.7 & 0.3 \ # S → S: 70%, S → R: 30%
0.5 & 0.5 \ # R → S: 50%, R → R: 50%
\end{bmatrix}
]
Predict Tomorrow:

If today is 60% Sunny, 40% Rainy:
Tomorrow’s Sunny = ( 0.6×0.7 + 0.4×0.5 = 62% ).
📝 All Units Summary
Unit	Key Topics	Real-World Use
I	GCD, Primes, CRT	Cryptography
II	Regression, Probability	Stock Predictions
III	Normal Curve, CLT	Quality Control
IV	Hypothesis Testing	Drug Efficacy Tests
V	Markov Chains	AI Recommendation Systems
📂 GitHub Repository Files
Unit-1-Number-Theory.md (Full GCD examples, Fermat numbers).
Unit-2-Regression-Probability.md (Dataset templates, Python code).
Unit-3-Sampling.md (CLT simulations in Python).
Unit-4-Hypothesis-Testing.md (Z-test calculators).
Unit-5-Markov-Chains.md (Weather prediction code).
Need even more breakdowns? Want video links or spreadsheet templates? Let me know! 😊
