# Corrected Regression & Correlation Formula Sheet  
## With Explanations and Example Questions/Answers

---

## Corrections to the Previous Extraction

1. **Probable Error (PE)**  
   Correct formula:
   \[
   PE = 0.6745\left(\frac{1-r^2}{\sqrt{n}}\right)
   \]
   The denominator is \(\sqrt n\), not \(n\).

2. **Regression of \(x\) on \(y\)**  
   If \(\hat x_i = c + d y_i\), then:
   \[
   d = \frac{S_{xy}}{S_{yy}}, \qquad c = \bar x - d\bar y
   \]
   The intercept uses \(\bar x - d\bar y\), not \(\bar y - d\bar x\).

3. **Multiple Regression Standard Error (two predictors)**  
   \[
   s_e^2 = \frac{S_{yy} - b_1 S_{1y} - b_2 S_{2y}}{n-3}
   \]
   Denominator is \(n-3\).

4. **Logistic Regression**  
   In practice the error term \(\epsilon\) is often omitted from the logit equation. Use the form given in the notes.

---

# 1. Simple Linear Regression

### 1.1 Population Regression Function
\[
\mu_{y|x} = f(x)
\]
\[
\mu_{y|x} = \alpha + \beta x
\]
**Meaning:** The mean value of \(y\) for a given \(x\) is a linear function of \(x\).

### 1.2 Simple Linear Regression Model
\[
y = \mu_{y|x} + \epsilon = \alpha + \beta x + \epsilon
\]
\[
\epsilon = y - \mu_{y|x} = y - (\alpha + \beta x)
\]
**Meaning:** Observed \(y\) equals the conditional mean plus random error.

### 1.3 Fitted Regression Line
\[
\hat y_i = a + b x_i
\]
\[
b = \frac{S_{xy}}{S_{xx}}
\]
\[
a = \bar y - b\bar x
\]
where
\[
S_{xy} = \sum (x_i-\bar x)(y_i-\bar y), \qquad
S_{xx} = \sum (x_i-\bar x)^2
\]
**Computational slope:**
\[
b = \frac{\sum x_i y_i - \frac{\sum x_i \sum y_i}{n}}
{\sum x_i^2 - \frac{(\sum x_i)^2}{n}}
\]

**Example Q:**  
For \(x = 1,2,3\) and \(y = 2,4,5\), find the least-squares line.  
**Answer:**  
\[
n=3,\ \sum x=6,\ \sum y=11,\ \sum x^2=14,\ \sum xy=25
\]
\[
b = \frac{25 - (6)(11)/3}{14 - 36/3} = \frac{3}{2} = 1.5
\]
\[
a = \frac{11}{3} - 1.5(2) = 0.6667
\]
\[
\hat y = 0.6667 + 1.5x
\]

### 1.4 Residual Sum of Squares
\[
SSE = \sum e_i^2 = \sum (y_i-\hat y_i)^2
= \sum [y_i - (a+bx_i)]^2
\]
**Meaning:** Total squared prediction error.

### 1.5 Standard Error of Estimate
\[
s_e = \sqrt{\frac{\sum (y_i-\hat y_i)^2}{n-2}}
\]
**Alternative:**
\[
s_e = \sqrt{\frac{\sum y_i^2 - a\sum y_i - b\sum x_i y_i}{n-2}}
\]
**Example Q:**  
Using the data above, compute \(s_e\).  
**Answer:**  
\[
SSE = 0.1667,\quad n-2=1
\]
\[
s_e = \sqrt{0.1667} = 0.408
\]

### 1.6 Goodness of Fit
\[
SSR = \sum (\hat y_i-\bar y)^2
\]
\[
SST = \sum (y_i-\bar y)^2
\]
\[
SST = SSR + SSE
\]
\[
r^2 = \frac{SSR}{SST} = 1 - \frac{SSE}{SST}
\]
**Meaning:** Proportion of total variation explained by the regression.

**Example Q:**  
Compute \(r^2\) for the data above.  
**Answer:**  
\[
SST = 4.6667,\quad SSE = 0.1667
\]
\[
r^2 = 1 - \frac{0.1667}{4.6667} = 0.964
\]

### 1.7 Correlation Coefficient
\[
r = \frac{S_{xy}}{\sqrt{S_{xx}S_{yy}}}
\]
\[
r = \pm \sqrt{r^2}
\]
**Example Q:**  
Find \(r\) for the data above.  
**Answer:**  
\[
r = \sqrt{0.964} = 0.982
\]

### 1.8 Regression of \(x\) on \(y\)
\[
\hat x_i = c + d y_i
\]
\[
d = \frac{S_{xy}}{S_{yy}}, \qquad c = \bar x - d\bar y
\]

---

# 2. Multiple Linear Regression

### 2.1 Model
\[
y = \alpha + \beta_1 x_1 + \beta_2 x_2 + \epsilon
\]
\[
y = \alpha + \beta_1 x_1 + \beta_2 x_2 + \cdots + \beta_k x_k + \epsilon
\]

### 2.2 Estimated Equation
\[
\hat y = a + b_1 x_1 + b_2 x_2 + \cdots + b_k x_k
\]

### 2.3 Two-Predictor Normal Equations
\[
\sum y_i = n a + b_1 \sum x_{1i} + b_2 \sum x_{2i}
\]
\[
\sum x_{1i}y_i = a\sum x_{1i} + b_1\sum x_{1i}^2 + b_2\sum x_{1i}x_{2i}
\]
\[
\sum x_{2i}y_i = a\sum x_{2i} + b_1\sum x_{1i}x_{2i} + b_2\sum x_{2i}^2
\]

### 2.4 Reduced Normal Equations
\[
S_{1y} = b_1 S_{11} + b_2 S_{12}
\]
\[
S_{2y} = b_1 S_{12} + b_2 S_{22}
\]

### 2.5 Solutions for Two Predictors
\[
b_1 = \frac{S_{22}S_{1y} - S_{12}S_{2y}}{S_{11}S_{22} - S_{12}^2}
\]
\[
b_2 = \frac{S_{11}S_{2y} - S_{12}S_{1y}}{S_{11}S_{22} - S_{12}^2}
\]
\[
a = \bar y - b_1\bar x_1 - b_2\bar x_2
\]

**Example Q:**  
Given \(a=-5.462\), \(b_1=0.734\), \(b_2=0.855\), predict \(y\) when \(x_1=17\), \(x_2=6\).  
**Answer:**  
\[
\hat y = -5.462 + 0.734(17) + 0.855(6) = 12.15
\]

### 2.6 Multiple Regression Standard Error
\[
s_e^2 = \frac{S_{yy} - b_1 S_{1y} - b_2 S_{2y}}{n-3}
\]
\[
SSR = b_1 S_{1y} + b_2 S_{2y}
\]
\[
R^2 = \frac{SSR}{SST}
\]
\[
R^2_{adj} = 1 - (1-R^2)\frac{n-1}{n-k-1}
\]

---

# 3. Multiple Correlation

### 3.1 Three-Variable Multiple Correlation
\[
R_{1,23}^2 = \frac{r_{12}^2 + r_{13}^2 - 2r_{12}r_{23}r_{13}}{1-r_{23}^2}
\]
\[
R_{2,13}^2 = \frac{r_{12}^2 + r_{23}^2 - 2r_{12}r_{13}r_{23}}{1-r_{13}^2}
\]
\[
R_{3,12}^2 = \frac{r_{13}^2 + r_{23}^2 - 2r_{12}r_{13}r_{23}}{1-r_{12}^2}
\]
\[
R = \sqrt{R^2}
\]

**Example Q:**  
Given \(r_{12}=0.97\), \(r_{13}=0.99\), \(r_{23}=0.97\), find \(R_{1,23}\).  
**Answer:**  
\[
R_{1,23}^2 = \frac{0.97^2 + 0.99^2 - 2(0.97)(0.99)(0.97)}{1-0.97^2}
= \frac{0.058}{0.059} = 0.98
\]
\[
R_{1,23} = \sqrt{0.98} = 0.99
\]

---

# 4. Inference in Multiple Regression

### 4.1 Overall \(F\)-Test
\[
F = \frac{R^2/k}{(1-R^2)/(n-k-1)} = \frac{MSR}{MSE}
\]
\[
MSR = \frac{SSR}{k}, \qquad MSE = \frac{SSE}{n-k-1}
\]

**Example Q:**  
\(n=10\), \(k=2\), \(R^2=0.9801\). Compute \(F\).  
**Answer:**  
\[
F = \frac{0.9801/2}{(1-0.9801)/(10-2-1)}
= \frac{0.49005}{0.002842} = 172.4
\]

### 4.2 Test for Individual Slope
\[
t_{n-k-1} = \frac{b_j - \beta_j}{SE(b_j)}
\]
\[
b_j \pm t^*_{n-k-1} \times SE(b_j)
\]

**Example Q:**  
\(b_2=-1.1458\), \(SE(b_2)=0.3463\), test \(H_0:\beta_2=0\).  
**Answer:**  
\[
t = \frac{-1.1458 - 0}{0.3463} = -3.31
\]
Reject \(H_0\) at 5% if \(|t|>2.36\).

### 4.3 Adjusted \(R^2\)
\[
R^2_{adj} = 1 - (1-R^2)\frac{n-1}{n-k-1}
= 1 - \frac{SSE/(n-k-1)}{SST/(n-1)}
\]

**Example Q:**  
\(n=10\), \(k=2\), \(R^2=0.9801\). Find adjusted \(R^2\).  
**Answer:**  
\[
R^2_{adj} = 1 - (1-0.9801)\frac{9}{7} = 0.9744
\]

### 4.4 Standard Error of Residuals
\[
s_e = \sqrt{\frac{SSE}{n-k-1}}
= \sqrt{\frac{\sum (y-\hat y)^2}{n-k-1}}
\]

---

# 5. Logistic Regression

### 5.1 Model
\[
\ln\left(\frac{p}{1-p}\right)
= \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \cdots + \beta_k x_k + \epsilon
\]

### 5.2 Estimated Probability
\[
\ln\left(\frac{\hat p}{1-\hat p}\right)
= b_0 + b_1 x_1 + \cdots + b_k x_k
\]
\[
\hat p = \frac{\exp(b_0 + b_1 x_1 + \cdots + b_k x_k)}
{1 + \exp(b_0 + b_1 x_1 + \cdots + b_k x_k)}
\]
\[
= \frac{1}{1 + \exp[-(b_0 + b_1 x_1 + \cdots + b_k x_k)]}
\]

**Example Q:**  
Simple logistic: \(b_0=-10.25\), \(b_1=0.52\), \(x_1=17\). Find \(\hat p\).  
**Answer:**  
\[
\text{logit} = -10.25 + 0.52(17) = -1.41
\]
\[
\hat p = \frac{e^{-1.41}}{1+e^{-1.41}} = 0.196
\]

---

# 6. Correlation and Probable Error

### 6.1 Correlation Coefficient
\[
r = \frac{S_{xy}}{\sqrt{S_{xx}S_{yy}}}
\]
\[
r = \frac{n\sum x_i y_i - \sum x_i \sum y_i}
{\sqrt{n\sum x_i^2 - (\sum x_i)^2}
 \sqrt{n\sum y_i^2 - (\sum y_i)^2}}
\]

### 6.2 Probable Error
\[
PE = 0.6745\left(\frac{1-r^2}{\sqrt n}\right)
\]
\[
r - PE \le \rho \le r + PE
\]

**Example Q:**  
\(n=64\), \(r=0.6\). Find PE and interval for \(\rho\).  
**Answer:**  
\[
PE = 0.6745\left(\frac{1-0.36}{8}\right) = 0.054
\]
\[
0.546 \le \rho \le 0.654
\]

---

# 7. Polynomial Regression

### 7.1 Second-Degree Polynomial
\[
\mu_{y|x} = \alpha + \beta_1 x + \beta_2 x^2
\]
**Meaning:** Curvilinear regression with one predictor.

**Example Q:**  
If \(\hat y = 2 + 0.5x + 0.1x^2\), predict \(y\) at \(x=3\).  
**Answer:**  
\[
\hat y = 2 + 0.5(3) + 0.1(9) = 4.4
\]

---

# 8. Key Assumptions

- Linearity in parameters.
- Independent errors.
- Normal errors with mean zero.
- Constant variance (homoscedasticity).
- No perfect multicollinearity in multiple regression.

---

This sheet is corrected and ready to copy into a `.md` file.
