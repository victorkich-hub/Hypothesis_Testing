# Hypothesis Testing Cheat Sheet

---

## What is Hypothesis Testing?

Hypothesis testing is a statistical method used to make decisions or inferences about a population parameter based on sample data.

---

## Key Terms

- **Population**: The entire group being studied.  
- **Sample**: A subset of the population used for analysis.  
- **Null Hypothesis (H₀)**: Assumes no effect or no difference.  
- **Alternative Hypothesis (H₁ or Ha)**: Assumes there is an effect or difference.  
- **Significance Level (α)**: Probability of rejecting H₀ when it is true (commonly 0.05).  
- **p-value**: Probability of observing the data (or something more extreme) assuming H₀ is true.  
- **Test Statistic**: A standardized value used to determine whether to reject H₀.  
- **Type I Error (α)**: Rejecting a true null hypothesis.  
- **Type II Error (β)**: Failing to reject a false null hypothesis.  

---

## Decision Rule

| Condition | Decision |
|------------|-----------|
| p-value ≤ α | Reject H₀ |
| p-value > α | Fail to reject H₀ |

---

## Types of Hypothesis Tests

### 1. **One-Sample t-Test**
Used to test whether the sample mean differs from a known or hypothesized population mean.

**Example:**  
> Is the average test score greater than 70?

**Hypotheses:**  
- H₀: μ = 70  
- H₁: μ > 70  

---

### 2. **Two-Sample t-Test (Independent Samples)**
Used to compare the means of two independent groups.

**Example:**  
> Do males and females have different average incomes?

**Hypotheses:**  
- H₀: μ₁ = μ₂  
- H₁: μ₁ ≠ μ₂  

---

### 3. **Paired t-Test**
Used when comparing two related samples (e.g., before and after a treatment).

**Example:**  
> Did a training program improve test scores?

**Hypotheses:**  
- H₀: μ_diff = 0  
- H₁: μ_diff ≠ 0  

---

### 4. **One-Way ANOVA**
Used to compare the means of three or more independent groups.

**Example:**  
> Do different teaching methods produce different average scores?

**Hypotheses:**  
- H₀: μ₁ = μ₂ = μ₃  
- H₁: At least one mean is different  

---

### 5. **Chi-Square Test of Independence**
Used to test whether two categorical variables are independent.

**Example:**  
> Is gender independent of survival on the Titanic?

**Hypotheses:**  
- H₀: The variables are independent  
- H₁: The variables are dependent  

---

### 6. **A/B Testing (Two-Proportion z-Test)**
Used to compare proportions between two groups.

**Example:**  
> Does version B of a webpage have a higher click-through rate than version A?

**Hypotheses:**  
- H₀: p₁ = p₂  
- H₁: p₁ ≠ p₂  

---

## Steps in Hypothesis Testing

1. **State the hypotheses (H₀ and H₁)**  
2. **Choose the significance level (α)**  
3. **Select the appropriate test**  
4. **Calculate the test statistic and p-value**  
5. **Compare p-value with α**  
6. **Make a decision (Reject or Fail to Reject H₀)**  
7. **Interpret the result in context**

---

## Common Mistakes to Avoid

- Interpreting “fail to reject H₀” as “accept H₀.”  
- Ignoring test assumptions (normality, equal variances, independence).    
- Treating p-value as the probability that H₀ is true.  
- Drawing conclusions without considering effect size or confidence intervals.  

---

## Quick Reference Table

| Test Type            | Data Type        | Groups | Typical Use Case |
|----------------------|------------------|---------|------------------|
| One-sample t-test    | Continuous       | 1       | Compare sample mean to a fixed value |
| Two-sample t-test    | Continuous       | 2       | Compare means of two independent groups |
| Paired t-test        | Continuous (paired) | 2 | Compare means of related samples (before–after) |
| ANOVA                | Continuous       | 3+      | Compare means across multiple groups |
| Chi-square test      | Categorical      | 2+      | Test independence of categorical variables |
| A/B test (z-test)    | Proportion       | 2       | Compare proportions between two groups |

---

## Interpretation Example

If **p-value = 0.03** and **α = 0.05**  
→ 0.03 < 0.05 ⇒ **Reject H₀**  
→ There is sufficient evidence to suggest a significant difference or effect.

---

## Additional Resources

- [Scipy.stats Documentation](https://docs.scipy.org/doc/scipy/reference/stats.html)  
- [Khan Academy: Hypothesis Testing](https://www.khanacademy.org/math/statistics-probability/significance-tests)  
- [StatQuest by Josh Starmer – YouTube](https://www.youtube.com/user/joshstarmer)

---
