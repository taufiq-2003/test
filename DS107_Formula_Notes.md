# DS 107 — Statistics: Complete Formula Reference Notes

> Every formula explained symbol-by-symbol with worked examples.  
> Covers: Descriptive Statistics · Central Tendency · Dispersion · Moments · Skewness & Kurtosis · Correlation · Regression · Multiple Regression · CLT · Quartiles / Deciles / Percentiles

---

## Table of Contents

1. [Organizing & Summarizing Data](#1-organizing--summarizing-data)
2. [Measures of Central Tendency](#2-measures-of-central-tendency)
3. [Measures of Dispersion](#3-measures-of-dispersion)
4. [Quartiles, Deciles & Percentiles](#4-quartiles-deciles--percentiles)
5. [Moments, Skewness & Kurtosis](#5-moments-skewness--kurtosis)
6. [Central Limit Theorem (CLT)](#6-central-limit-theorem-clt)
7. [Correlation Analysis](#7-correlation-analysis)
8. [Simple Linear Regression](#8-simple-linear-regression)
9. [Multiple Regression & Correlation](#9-multiple-regression--correlation)
10. [Quick Reference Table](#10-quick-reference-table)

---

## 1. Organizing & Summarizing Data

### 1.1 Relative Frequency & Percentage

> **Definition:** Relative frequency tells you what *fraction* of the total observations fall in a particular category or class.

$$\text{Relative Frequency} = \frac{f}{n}$$

| Symbol | Meaning |
|--------|---------|
| **f** | Frequency of that class — how many times that value/category appears |
| **n** | Total number of observations in the entire dataset (sum of all frequencies) |

$$\text{Percentage} = \text{Relative Frequency} \times 100$$

**Example:**  
A class of 40 students was asked their favourite subject.  
Math: 16, Science: 12, English: 8, History: 4

- Relative Frequency of Math = 16 ÷ 40 = **0.40**
- Percentage of Math = 0.40 × 100 = **40%**
- This means 40% of students prefer Math.

> 📝 **Note:** All relative frequencies must add up to **1.0**, and all percentages must add up to **100%**.

---

### 1.2 Class Width & Class Midpoint

> **Definition:** When grouping large datasets into intervals (classes), we need to decide how wide each interval is and what its centre value is.

#### Exact Class Width

$$\text{Class Width} = \text{Upper Boundary} - \text{Lower Boundary}$$

| Symbol | Meaning |
|--------|---------|
| **Upper Boundary** | The upper real boundary of the class (e.g. 69.5 for class 60–69) |
| **Lower Boundary** | The lower real boundary of the class (e.g. 59.5 for class 60–69) |
| **Class Width** | How wide the interval is — the "size" of each group |

#### Approximate Class Width (for deciding how many classes to use)

$$\text{Approx. Class Width} = \frac{\text{Largest value} - \text{Smallest value}}{\text{Number of classes}}$$

| Symbol | Meaning |
|--------|---------|
| **Largest value** | The maximum (biggest) value in the entire dataset |
| **Smallest value** | The minimum (smallest) value in the entire dataset |
| **Number of classes** | How many groups/intervals you want (chosen by analyst, typically 5–20) |
| **Approx. Class Width** | Raw estimate of interval size — usually rounded UP to a convenient number |

**Example:**  
30 students scored between 5 and 29. Use 5 classes.

```
Largest value  = 29
Smallest value = 5
Number of classes = 5

Approx. Class Width = (29 - 5) / 5 = 24 / 5 = 4.8
→ Round up to 5 (convenient whole number)
Classes: 5–9, 10–14, 15–19, 20–24, 25–29
```

> 📝 **Note:** Always round UP to a convenient number. This prevents data from falling outside your last class.

#### Class Midpoint (Class Mark)

$$m = \frac{\text{Lower limit} + \text{Upper limit}}{2}$$

| Symbol | Meaning |
|--------|---------|
| **Lower limit** | The smallest value that belongs to the class (e.g. 10 for class 10–14) |
| **Upper limit** | The largest value that belongs to the class (e.g. 14 for class 10–14) |
| **m** | The centre of the class — represents ALL values in that class in grouped calculations |

**Example:**  
Midpoint of class 10–14:  m = (10 + 14) / 2 = **12**

---

### 1.3 Cumulative Relative Frequency & Cumulative Percentage

$$\text{Cumulative Relative Frequency} = \frac{\text{Cumulative frequency}}{n}$$

$$\text{Cumulative Percentage} = \text{Cumulative Relative Frequency} \times 100$$

**Example:**  
iPod sales over 30 days, grouped into 5 classes:

| Class | f | Cum. f | Cum. Rel. Freq | Cum. % |
|-------|---|--------|----------------|--------|
| 5–9   | 2 | 2      | 2/30 = 0.067   | 6.7%   |
| 10–14 | 6 | 8      | 8/30 = 0.267   | 26.7%  |
| 15–19 | 8 | 16     | 16/30 = 0.533  | 53.3%  |

→ 53.3% of days had sales of **19 or fewer** iPods.

---

## 2. Measures of Central Tendency

### 2.1 Arithmetic Mean (x̄ or μ)

> **Definition:** The mean is the "balance point" of the data — sum of all values divided by the count. Uses every single value.

#### Ungrouped Data

$$\mu = \frac{\sum x_i}{N} \quad \text{(Population Mean)}$$

$$\bar{x} = \frac{\sum x_i}{n} \quad \text{(Sample Mean)}$$

| Symbol | Meaning |
|--------|---------|
| **x_i** | Each individual value in the dataset (x₁, x₂, ..., xₙ) |
| **Σ x_i** | Summation — add up ALL values: x₁ + x₂ + ... + xₙ |
| **N** | Total number of values in the **POPULATION** (entire group of interest) |
| **n** | Total number of values in the **SAMPLE** (a subset taken from the population) |
| **μ** (mu) | Population mean — used when you have ALL population data |
| **x̄** (x-bar) | Sample mean — used when you have only a sample |

**Example:**  
Ages of 8 employees: 53, 32, 61, 27, 39, 44, 49, 57

```
Σ x_i = 53+32+61+27+39+44+49+57 = 362
N = 8  (all employees = population)
μ = 362 / 8 = 45.25 years
```
→ On average, an employee is **45.25 years** old.

#### Grouped Data (frequency table)

$$\mu = \frac{\sum m_i f_i}{N} \qquad \bar{x} = \frac{\sum m_i f_i}{n}$$

| Symbol | Meaning |
|--------|---------|
| **m_i** | Midpoint of class i — represents all values in that class |
| **f_i** | Frequency of class i — how many observations fall in that class |
| **m_i × f_i** | Weighted contribution of each class |
| **Σ(m_i f_i)** | Total of all weighted midpoints |
| **N or n** | Total observations = Σf_i |

> 📝 **Note:** The mean is sensitive to outliers. One very large or small value can pull it away from centre. In that case, the **median** is better.

---

### 2.2 Geometric Mean (GM)

> **Definition:** The n-th root of the product of all values. Correct average for growth rates, ratios, and percentages.

$$GM = \sqrt[n]{x_1 \times x_2 \times \cdots \times x_n} = (x_1 \cdot x_2 \cdots x_n)^{1/n}$$

| Symbol | Meaning |
|--------|---------|
| **x₁, x₂, ..., xₙ** | All n values in the dataset |
| **n** | Number of values |
| **(...)^(1/n)** | Take the n-th root = raise to the power 1/n |

**Example:**  
A company grew by 10%, 20%, 30% over 3 years. Average growth rate?

```
Values: 1.10, 1.20, 1.30
GM = (1.10 × 1.20 × 1.30)^(1/3) = (1.716)^(0.333) = 1.197
Average growth = 19.7% per year

(Arithmetic mean would give 20% — slightly overestimates)
```

> 📝 **Note:** **AM ≥ GM ≥ HM** for positive values. Use GM for compound interest, population growth, index numbers.

---

### 2.3 Harmonic Mean (HM)

> **Definition:** The reciprocal of the arithmetic mean of the reciprocals. Best for averaging RATES (speed, efficiency).

$$HM = \frac{n}{\sum \frac{1}{x_i}} = \frac{n}{\frac{1}{x_1} + \frac{1}{x_2} + \cdots + \frac{1}{x_n}}$$

| Symbol | Meaning |
|--------|---------|
| **1/x_i** | Reciprocal (inverse) of each value |
| **Σ(1/x_i)** | Sum of all reciprocals |
| **n** | Number of values |

**Example:**  
A car travels 60 km/h for the first half of a journey and 40 km/h for the second half. Average speed?

```
HM = 2 / (1/60 + 1/40) = 2 / (0.0167 + 0.025) = 2 / 0.0417 = 48 km/h

Note: Arithmetic mean gives (60+40)/2 = 50 km/h — INCORRECT for this scenario!
```

---

### 2.4 Median

> **Definition:** The MIDDLE value after sorting data in ascending order. Exactly 50% of values lie below it and 50% above. **Not affected by outliers.**

#### Ungrouped — Odd number of values

$$\text{Median} = \text{value at position } \frac{n+1}{2} \text{ (after sorting)}$$

**Example:** 7 house prices (thousands): 257, 289, 312, 374, 421, 497, 526  
Position = (7+1)/2 = 4th value = **374**

#### Ungrouped — Even number of values

$$\text{Median} = \text{average of values at positions } \frac{n}{2} \text{ and } \frac{n}{2}+1$$

**Example:** Profits (sorted): 7, 8, 9, 10, 11, **12, 13**, 13, 14, 17, 17, 45 (n=12)  
Positions 6 and 7: values 12 and 13 → Median = (12+13)/2 = **12.5**

#### Grouped Data (interpolation formula)

$$\text{Median} = L + \left[\frac{\frac{n}{2} - F}{f}\right] \times C$$

| Symbol | Meaning |
|--------|---------|
| **L** | Real lower boundary of the **median class** (the class containing the median) |
| **n** | Total number of observations |
| **n/2** | Target position — we are looking for the middle observation |
| **F** | Cumulative frequency of ALL classes **BEFORE** the median class |
| **f** | Frequency of the median class itself |
| **C** | Class width (length of the interval) |

**Example:**  
Classes: 50–69 (f=3), 70–89 (f=7), 90–109 (f=4), 110–129 (f=4), 130–149 (f=9). n=27

```
n/2 = 13.5 → find class where cumulative freq first reaches 13.5
Cumulative freqs: 3, 10, 14, 18, 27 → Median class = 90–109 (cum.freq=14 ≥ 13.5)

L = 89.5,  F = 10,  f = 4,  C = 20
Median = 89.5 + [(13.5 - 10) / 4] × 20
       = 89.5 + [3.5/4] × 20
       = 89.5 + 17.5 = 107
```

---

### 2.5 Mode

> **Definition:** The value that appears **most frequently** in the dataset.

$$\text{Mode} = \text{value with the highest frequency}$$

**Example:** Speeds: 77, 82, **74**, 81, 79, 84, **74**, 78 → **Mode = 74 mph** (appears twice)

| Distribution Shape | Relationship |
|--------------------|-------------|
| Symmetric | Mean = Median = Mode |
| Right-skewed (+) | Mode < Median < Mean |
| Left-skewed (−) | Mean < Median < Mode |

---

## 3. Measures of Dispersion

### 3.1 Range

> **Definition:** The simplest measure of spread — the gap between the biggest and smallest values.

$$R = X_{max} - X_{min}$$

$$\text{Coefficient of Range} = \frac{X_{max} - X_{min}}{X_{max} + X_{min}}$$

| Symbol | Meaning |
|--------|---------|
| **X_max** | The largest (maximum) value in the dataset |
| **X_min** | The smallest (minimum) value in the dataset |
| **R** | Range — total spread from lowest to highest |
| **Coefficient of Range** | Unit-free relative version — used to compare datasets with different units |

**Example:** Marks: 45, 32, 37, 46, 39, 36, 41, 48, 36  
X_max = 48, X_min = 32  
R = 48 − 32 = **16 marks**  
Coeff. of Range = (48−32)/(48+32) = 16/80 = **0.20**

> 📝 **Note:** Range is easily affected by outliers and ignores all values in between.

---

### 3.2 Quartile Deviation (Semi-Inter-Quartile Range)

> **Definition:** Half the distance between Q3 and Q1. Covers the middle 50% of data — not affected by outliers.

$$QD = \frac{Q_3 - Q_1}{2}$$

$$\text{Coefficient of QD} = \frac{Q_3 - Q_1}{Q_3 + Q_1}$$

| Symbol | Meaning |
|--------|---------|
| **Q₁** | Lower quartile — 25% of data falls BELOW this value |
| **Q₃** | Upper quartile — 75% of data falls BELOW this value |
| **Q₃ − Q₁** | Inter-Quartile Range (IQR) — spread of the middle 50% of data |
| **QD** | Semi-IQR — average distance from median to either quartile |

**Example:** Sorted marks: 32, 36, 36, 37, 39, 41, 45, 46, 48 (n=9)  
Q₁ = 36, Q₃ = 45  
QD = (45 − 36) / 2 = **4.5 marks**  
Coeff. of QD = (45−36)/(45+36) = 9/81 = **0.11**

---

### 3.3 Mean Deviation (Average Deviation)

> **Definition:** The average of how far each value is from the mean (or median), always taking distance as positive.

$$MD_{\bar{x}} = \frac{\sum |x_i - \bar{x}|}{n} \qquad MD_{Med} = \frac{\sum |x_i - \text{Median}|}{n}$$

$$MD_{\text{grouped}} = \frac{\sum f_i \cdot |x_i - \bar{x}|}{\sum f_i}$$

$$\text{Coefficient of MD} = \frac{MD}{\bar{x}} \quad \text{(or } \frac{MD}{\text{Median}}\text{)}$$

| Symbol | Meaning |
|--------|---------|
| **\|x_i − x̄\|** | Absolute deviation — distance of each value from the mean, always positive |
| **Σ\|...\|** | Add up all the absolute deviations |
| **f_i** | Frequency of class i (for grouped data) |

**Example:** Marks: 45,32,37,46,39,36,41,48,36. Mean x̄ = 40

```
|45−40|=5, |32−40|=8, |37−40|=3, |46−40|=6,
|39−40|=1, |36−40|=4, |41−40|=1, |48−40|=8, |36−40|=4

Σ|deviations| = 5+8+3+6+1+4+1+8+4 = 40
MD = 40 / 9 = 4.44 marks
Coefficient of MD = 4.44 / 40 = 0.111
```

---

### 3.4 Variance & Standard Deviation

> **Definition:** Variance = average of **squared** deviations from the mean. Standard deviation (σ or s) = its square root — in the same units as the data.

#### Ungrouped Data — Direct Formula

$$\sigma^2 = \frac{\sum (x_i - \mu)^2}{N} \qquad s^2 = \frac{\sum (x_i - \bar{x})^2}{n-1}$$

| Symbol | Meaning |
|--------|---------|
| **σ²** (sigma squared) | Population variance |
| **s²** | Sample variance |
| **(x_i − μ)²** | Squared deviation of each value from the mean — always positive |
| **N** | Population size |
| **n−1** | Degrees of freedom — we use n−1 (not n) for samples to avoid underestimating variance |

#### Shortcut Formula (faster computation)

$$\sigma^2 = \frac{\sum x_i^2 - \dfrac{(\sum x_i)^2}{N}}{N} \qquad s^2 = \frac{\sum x_i^2 - \dfrac{(\sum x_i)^2}{n}}{n-1}$$

| Symbol | Meaning |
|--------|---------|
| **Σx_i²** | Sum of the **SQUARES** of each value: x₁² + x₂² + ... + xₙ² |
| **(Σx_i)²** | **Square of the SUM** of all values: (x₁+x₂+...+xₙ)² ← different from above! |
| **(Σx_i)²/n** | Correction factor |

**Example:** Market values (billions): 34, 67, 238, 141, 182

```
n=5
Σx = 34+67+238+141+182 = 662
Σx² = 34²+67²+238²+141²+182² = 1156+4489+56644+19881+33124 = 115294

s² = [115294 − (662²)/5] / (5−1)
   = [115294 − 87648.8] / 4
   = 27645.2 / 4 = 6911.3  (billions²)

s = √6911.3 = 83.1 billion dollars
```
→ The typical market value deviates from the mean by about **$83 billion**.

#### Grouped Data Shortcut

$$s^2 = \frac{\sum m_i^2 f_i - \dfrac{(\sum m_i f_i)^2}{n}}{n-1}$$

| Symbol | Meaning |
|--------|---------|
| **m_i** | Midpoint of class i |
| **m_i² × f_i** | Square of midpoint times its frequency |
| **(Σm_if_i)²/n** | Correction factor using grouped mean |

#### Standard Deviation

$$\sigma = \sqrt{\sigma^2} \qquad s = \sqrt{s^2}$$

> 📝 **Note:** σ (or s) has the **same units** as the original data. A smaller σ means data is tightly clustered around the mean; a larger σ means it is more spread out.

---

### 3.5 Coefficient of Variation (CV)

> **Definition:** Expresses the standard deviation as a percentage of the mean. Used to compare variability between two datasets with different units or scales.

$$CV = \frac{\sigma}{\mu} \times 100 \quad \text{or} \quad CV = \frac{s}{\bar{x}} \times 100 \quad (\%)$$

| Symbol | Meaning |
|--------|---------|
| **σ or s** | Standard deviation of the dataset |
| **μ or x̄** | Mean of the dataset |
| **CV** | Result is a percentage — higher CV = more relative variability |

**Example:**  
Dataset A: mean=50, SD=5 → CV = (5/50)×100 = **10%**  
Dataset B: mean=1000, SD=50 → CV = (50/1000)×100 = **5%**

→ Dataset A is MORE variable (10% > 5%) even though Dataset B has a larger SD.

> 📝 **Note:** CV is unitless — you can compare apples and oranges. Introduced by **Karl Pearson**. Lower CV = more consistent data.

---

## 4. Quartiles, Deciles & Percentiles

> **Quartiles** divide sorted data into 4 equal parts.  
> **Deciles** divide into 10 equal parts.  
> **Percentiles** divide into 100 equal parts.

### 4.1 Ungrouped Data — Positional Formula

**Step 1:** Arrange data in **ascending order**.  
**Step 2:** Calculate position using formula below.  
**Step 3:**  
- If position is a **fraction** → use the **next integer's** value.  
- If position is a **whole number** → use the **average** of that value and the next one.

$$q_k = \frac{k}{4} \times n \quad \text{(Quartile position, } k=1,2,3\text{)}$$

$$d_k = \frac{k}{10} \times n \quad \text{(Decile position, } k=1,...,9\text{)}$$

$$p_k = \frac{k}{100} \times n \quad \text{(Percentile position, } k=1,...,99\text{)}$$

| Symbol | Meaning |
|--------|---------|
| **k** | The number of the quartile/decile/percentile you want (e.g. k=1 for Q₁, k=3 for Q₃) |
| **n** | Total number of values |
| **q_k, d_k, p_k** | The **position (rank)** in the sorted list where the value lies |

**Example (odd n):** Data: 20, 22, 23, 25, 30, 32, 36 (n=7, sorted)

```
Q₁: position = (1/4)×7 = 1.75 → fraction → use position 2 → Q₁ = 22
Q₂: position = (2/4)×7 = 3.5  → fraction → use position 4 → Q₂ = 25
Q₃: position = (3/4)×7 = 5.25 → fraction → use position 6 → Q₃ = 32
```

**Example (even n):** Sorted: 18, 20, 22, 23, 25, 30, 32, 36 (n=8)

```
Q₁: position = (1/4)×8 = 2 → whole number → average of positions 2 and 3
Q₁ = (20+22)/2 = 21
```

---

### 4.2 Grouped Data — Interpolation Formula

$$Q_k = L + \left[\frac{\frac{kn}{4} - F}{f}\right] \times C$$

$$D_k = L + \left[\frac{\frac{kn}{10} - F}{f}\right] \times C$$

$$P_k = L + \left[\frac{\frac{kn}{100} - F}{f}\right] \times C$$

| Symbol | Meaning |
|--------|---------|
| **L** | Real lower class boundary of the required class |
| **k** | The quartile/decile/percentile number you want |
| **n** | Total observations = Σf |
| **kn/4** | Target cumulative frequency position for quartile k |
| **F** | Cumulative frequency of ALL classes **BEFORE** the required class |
| **f** | Frequency of the required class |
| **C** | Class width |

**Example:** Find Q₁ from: 50–69(f=3), 70–89(f=7), 90–109(f=4), 110–129(f=4), 130–149(f=9). n=27

```
Target = (1/4)×27 = 6.75
Cumulative freqs: 3, 10, 14, 18, 27 → Q₁ class = 70–89 (cum.freq=10 ≥ 6.75)

L=69.5,  F=3,  f=7,  C=20
Q₁ = 69.5 + [(6.75−3)/7] × 20 = 69.5 + 10.71 = 80.21
```

> 📝 **Note:** Q₂ = D₅ = P₅₀ = Median. All three use the same formula — only the multiplier changes.

---

### 4.3 Percentile Rank (Reverse Lookup)

> Given a value X, find what percentage of data falls below it.

$$\text{Percentile Rank of } X = \frac{\left[\frac{X-L}{C} \times f + F\right]}{n} \times 100 \quad (\%)$$

---

## 5. Moments, Skewness & Kurtosis

### 5.1 Central Moments (Moments About the Mean)

> **Definition:** The r-th moment describes the shape of a distribution. Computed as the average of the r-th power of deviations from the mean.

#### Ungrouped Data

$$m_r = \frac{\sum (x_i - \bar{x})^r}{n} \qquad [r = 1, 2, 3, 4]$$

| Symbol | Meaning |
|--------|---------|
| **m_r** | The r-th central moment |
| **r** | Order of the moment (1st, 2nd, 3rd, or 4th) |
| **(x_i − x̄)** | Deviation of each value from the mean |
| **(x_i − x̄)^r** | That deviation raised to the power r |
| **Σ(...)/n** | Average of all those powered deviations |

$$m_1 = 0 \quad \text{(always — 1st central moment is always zero)}$$
$$m_2 = \text{Variance} = \sigma^2$$
$$m_3 = \frac{\sum(x_i - \bar{x})^3}{n} \quad \text{(related to asymmetry)}$$
$$m_4 = \frac{\sum(x_i - \bar{x})^4}{n} \quad \text{(related to peakedness)}$$

#### Grouped Data

$$m_r = \frac{\sum f_i (x_i - \bar{x})^r}{\sum f_i}$$

**Example:** Marks: 32,36,36,37,39,41,45,46,48.  x̄ = 40

```
Deviations: −8, −4, −4, −3, −1, 1, 5, 6, 8

m₁ = (0)/9 = 0
m₂ = (64+16+16+9+1+1+25+36+64)/9 = 232/9 = 25.78  marks²
m₃ = (−512−64−64−27−1+1+125+216+512)/9 = 186/9 = 20.67  marks³
m₄ = (4096+256+256+81+1+1+625+1296+4096)/9 = 1189.78  marks⁴
```

---

### 5.2 Skewness (β₁)

> **Definition:** Measures the ASYMMETRY of a distribution. A symmetric distribution (bell curve) has skewness = 0.

$$\beta_1 = \frac{m_3^2}{m_2^3}$$

$$\gamma_1 = \frac{m_3}{m_2^{3/2}} = \sqrt{\beta_1} \quad \text{(signed version)}$$

| Symbol | Meaning |
|--------|---------|
| **m₃** | 3rd central moment |
| **m₂** | 2nd central moment = variance |
| **β₁ = 0** | Symmetric (mean = median = mode) |
| **β₁ > 0** | Right-skewed: right tail longer, mean > median > mode |
| **γ₁ < 0** | Left-skewed: left tail longer, mean < median < mode |

**Example:** m₂ = 25.78,  m₃ = 20.67  
β₁ = (20.67)² / (25.78)³ = 427.25 / 17133.7 = **0.025** → slightly right-skewed

---

### 5.3 Kurtosis (β₂)

> **Definition:** Measures how PEAKED or FLAT the distribution is compared to the normal curve. Normal distribution has β₂ = 3.

$$\beta_2 = \frac{m_4}{m_2^2}$$

| β₂ Value | Type | Description |
|----------|------|-------------|
| β₂ = 3 | Mesokurtic | Same shape as normal distribution |
| β₂ > 3 | Leptokurtic | Taller, more peaked; heavier tails |
| β₂ < 3 | Platykurtic | Flatter than normal; lighter tails |

**Example:** m₂ = 25.78,  m₄ = 1189.78  
β₂ = 1189.78 / (25.78)² = 1189.78 / 664.6 = **1.79** → Platykurtic (flatter than normal)

---

## 6. Central Limit Theorem (CLT)

> **Definition:** When drawing repeated random samples of size n from ANY population with mean μ and standard deviation σ, the sampling distribution of sample means (x̄) will be approximately **NORMAL** when n ≥ 30, regardless of the original population's shape.

### 6.1 Standard Error of the Mean

$$\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$$

| Symbol | Meaning |
|--------|---------|
| **σ_x̄** | Standard Error — standard deviation of the sampling distribution of means |
| **σ** | Standard deviation of the original POPULATION |
| **n** | Sample size |
| **√n** | As sample size increases, standard error DECREASES — larger samples give more precise estimates |

**Example:** Tyre lifetimes: μ = 25000 miles, σ = 1600 miles, n = 64  
σ_x̄ = 1600 / √64 = 1600 / 8 = **200 miles**

---

### 6.2 Z-Score for Sample Means

$$Z = \frac{\bar{x} - \mu}{\sigma_{\bar{x}}} = \frac{\bar{x} - \mu}{\sigma / \sqrt{n}}$$

| Symbol | Meaning |
|--------|---------|
| **x̄** | The sample mean value you are testing |
| **μ** | The population mean |
| **σ_x̄** | Standard error = σ / √n |
| **Z** | How many standard errors x̄ is from μ — use Z-table to find probability |

**Example:** Find P(x̄ < 24600) when μ=25000, σ_x̄=200

```
Z = (24600 − 25000) / 200 = −400/200 = −2.0
P(Z < −2.0) = 0.0228  (from Z-table)
→ 2.28% chance that mean lifetime of 64 tyres is less than 24600 miles.
```

---

## 7. Correlation Analysis

### 7.1 Karl Pearson's Coefficient of Correlation (r)

> **Definition:** Measures the strength and direction of the LINEAR relationship between two variables x and y. Given by Karl Pearson in 1890.

$$r = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum(x_i - \bar{x})^2 \cdot \sum(y_i - \bar{y})^2}}$$

#### Shortcut (Computational) Formula

$$r = \frac{n\sum x_i y_i - \sum x_i \cdot \sum y_i}{\sqrt{\left[n\sum x_i^2 - (\sum x_i)^2\right]\left[n\sum y_i^2 - (\sum y_i)^2\right]}}$$

| Symbol | Meaning |
|--------|---------|
| **n** | Number of data pairs |
| **Σx_i y_i** | Sum of products of each (x, y) pair |
| **Σx_i** | Sum of all x values |
| **Σy_i** | Sum of all y values |
| **Σx_i²** | Sum of squares of x values |
| **Σy_i²** | Sum of squares of y values |
| **r** | Correlation coefficient — always between −1 and +1 |

**Example:** Pulse rate study (n=10): Σx=635, Σy=63, Σx²=40537, Σy²=541, Σxy=3835

```
r = [10×3835 − 635×63] / √{[10×40537 − 635²][10×541 − 63²]}
  = [38350 − 40005] / √{[405370−403225][5410−3969]}
  = −1655 / √{2145 × 1441}
  = −1655 / 1758.0 = −0.94

r = −0.94 → Strong NEGATIVE relationship:
As water temperature increases, pulse rate reduction decreases.
```

#### Interpretation of r

| r value | Interpretation |
|---------|----------------|
| r = +1 | Perfect positive |
| 0.7 ≤ r < 1 | Strong positive |
| 0.4 ≤ r < 0.7 | Fairly positive |
| 0 < r < 0.4 | Weak positive |
| r = 0 | No linear correlation |
| −0.4 < r < 0 | Weak negative |
| −0.7 < r ≤ −0.4 | Fairly negative |
| −1 < r ≤ −0.7 | Strong negative |
| r = −1 | Perfect negative |

#### Coefficient of Determination

$$r^2 = \frac{\text{Explained Variation}}{\text{Total Variation}}$$

> r² = 0.81 means **81%** of variation in y is explained by x. Range: 0 ≤ r² ≤ 1.

---

### 7.2 Spearman's Rank Correlation Coefficient (R)

> **Definition:** Used when data is in RANKS or is QUALITATIVE (beauty, honesty, etc.). Introduced by Spearman (1904).

#### No tied ranks

$$R = 1 - \frac{6\sum d_i^2}{n(n^2 - 1)}$$

| Symbol | Meaning |
|--------|---------|
| **d_i** | d_i = R₁ᵢ − R₂ᵢ = difference between ranks of i-th pair on variable x and y |
| **d_i²** | Square of each rank difference |
| **Σd_i²** | Sum of all squared rank differences |
| **n** | Number of pairs |
| **n(n²−1)** | Denominator formula for n items |

**Example:** 6 students ranked by two methods (d²: 9,1,25,1,16,16)

```
Σd² = 68,  n = 6
R = 1 − [6×68] / [6×(36−1)] = 1 − 408/210 = 1 − 1.943 = −0.94
→ Strong negative rank correlation
```

#### With tied ranks

$$R = 1 - \frac{6\left[\sum d_i^2 + \frac{m_1^3 - m_1}{12} + \frac{m_2^3 - m_2}{12} + \cdots\right]}{n(n^2-1)}$$

| Symbol | Meaning |
|--------|---------|
| **m** | Number of times a particular rank is repeated (size of a tie group) |
| **(m³−m)/12** | Correction term added to Σd² for each tie group |

---

## 8. Simple Linear Regression

> **Definition:** Finds the best-fit straight line to predict one variable from another. Term coined by Sir Francis Galton (1877).

### 8.1 Regression Line of y on x (predict y from x)

$$\hat{y} = a + b_{yx} \cdot x$$

| Symbol | Meaning |
|--------|---------|
| **ŷ** (y-hat) | Predicted (estimated) value of the dependent variable |
| **x** | Known value of the independent variable |
| **a** | y-intercept — predicted value of y when x = 0 |
| **b_yx** | Slope — how much y changes for each 1-unit increase in x |

#### Slope formula

$$b_{yx} = \frac{n\sum x_i y_i - \sum x_i \cdot \sum y_i}{n\sum x_i^2 - \left(\sum x_i\right)^2}$$

#### Intercept formula

$$a = \bar{y} - b_{yx} \cdot \bar{x}$$

**Example:** Husband/wife ages (n=7): Σx=224, Σy=175, Σx²=7334, Σy²=4643, Σxy=5798

```
b_yx = [7×5798 − 224×175] / [7×7334 − 224²]
     = [40586 − 39200] / [51338 − 50176]
     = 1386 / 1162 = 1.193

x̄ = 224/7 = 32,  ȳ = 175/7 = 25
a = 25 − 1.193×32 = 25 − 38.18 = −13.18

Regression line: ŷ = −13.18 + 1.193x

Prediction: If husband's age = 45 years:
ŷ = −13.18 + 1.193×45 = 40.5 years (wife's predicted age)
```

---

### 8.2 Regression Line of x on y (predict x from y)

$$\hat{x} = a + b_{xy} \cdot y$$

$$b_{xy} = \frac{n\sum x_i y_i - \sum x_i \cdot \sum y_i}{n\sum y_i^2 - \left(\sum y_i\right)^2}$$

$$a = \bar{x} - b_{xy} \cdot \bar{y}$$

> 📝 **Note:** b_yx ≠ b_xy — they are **different lines**! Use y-on-x to predict y; use x-on-y to predict x.

---

### 8.3 Finding r from Regression Coefficients

$$r = \sqrt{b_{yx} \times b_{xy}}$$

| Symbol | Meaning |
|--------|---------|
| **b_yx** | Slope of regression line of y on x |
| **b_xy** | Slope of regression line of x on y |
| **r** | Pearson's correlation coefficient — geometric mean of the two slopes |

> 📝 The **sign** of r is the same as the sign of b_yx and b_xy.

**Example:** b_yx = −0.77, b_xy = −1.1  
r = −√(0.77 × 1.1) = −√0.847 = **−0.92**

---

## 9. Multiple Regression & Correlation

### 9.1 Multiple Regression Model

> **Definition:** Extends simple regression to 2+ predictor variables. Finds the best-fitting hyperplane.

$$y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \cdots + \beta_k x_k + \varepsilon \quad \text{(population)}$$

$$\hat{y} = b_0 + b_1 x_1 + b_2 x_2 + \cdots + b_k x_k \quad \text{(fitted)}$$

| Symbol | Meaning |
|--------|---------|
| **y** | Dependent variable (what you predict) |
| **x₁, x₂, ..., xₖ** | Independent (predictor) variables |
| **b₀** | Intercept — predicted y when ALL predictors = 0 |
| **b_j** | Partial slope for x_j — change in y per 1-unit increase in x_j, **holding all other predictors constant** |
| **ε** (epsilon) | Error term — part of y not explained by the model |
| **k** | Number of predictor variables |

**Example:** ŷ = 164.0 − 0.44x₁ − 1.15x₂ (reading ability from brightness x₁ and noise x₂)

```
b₁ = −0.44: For each 1-unit increase in brightness (holding noise constant),
             reading ability DECREASES by 0.44 units.

b₂ = −1.15: For each 1-unit increase in noise (holding brightness constant),
             reading ability DECREASES by 1.15 units.

Prediction at x₁=19, x₂=58:
ŷ = 164.0 − 0.44(19) − 1.15(58) = 164.0 − 8.36 − 66.7 = 88.94
```

---

### 9.2 Multiple Correlation Coefficient (R)

$$R^2_{1.23} = \frac{r_{12}^2 + r_{13}^2 - 2r_{12}r_{13}r_{23}}{1 - r_{23}^2}$$

$$R^2_{2.13} = \frac{r_{12}^2 + r_{23}^2 - 2r_{12}r_{13}r_{23}}{1 - r_{13}^2} \qquad R^2_{3.12} = \frac{r_{13}^2 + r_{23}^2 - 2r_{12}r_{13}r_{23}}{1 - r_{12}^2}$$

| Symbol | Meaning |
|--------|---------|
| **R₁.₂₃** | Multiple correlation of X₁ with X₂ and X₃ combined |
| **r₁₂** | Simple Pearson correlation between X₁ and X₂ |
| **r₁₃** | Simple correlation between X₁ and X₃ |
| **r₂₃** | Simple correlation between X₂ and X₃ |
| **1 − r₂₃²** | Adjusts for correlation between the two predictors |

**Example:** r₁₂=0.80, r₁₃=0.64, r₂₃=0.79

```
R²₁.₂₃ = (0.64 + 0.41 − 2×0.80×0.64×0.79) / (1 − 0.62)
        = (1.05 − 0.81) / 0.38 = 0.24/0.38 = 0.632
R₁.₂₃ = √0.632 = 0.79
→ 79% of variation in X₁ is jointly explained by X₂ and X₃.
```

---

### 9.3 R², Adjusted R², and Standard Error

$$R^2 = \frac{SSR}{SST} = 1 - \frac{SSE}{SST}$$

| Term | Formula | Meaning |
|------|---------|---------|
| **SST** | Σ(y_i − ȳ)² | Total variation in y |
| **SSR** | Σ(ŷ − ȳ)² | Variation **explained** by the model |
| **SSE** | Σ(y_i − ŷ)² | Variation **not** explained (residuals) |
| **R²** | SSR/SST | Proportion of variation explained (0 to 1) |

$$R^2_{adj} = 1 - \frac{(1-R^2)(n-1)}{n-k-1} = 1 - \frac{SSE/(n-k-1)}{SST/(n-1)}$$

$$s_e = \sqrt{\frac{SSE}{n-k-1}}$$

> 📝 Use **Adjusted R²** when comparing models with different numbers of predictors — it penalizes for adding unnecessary variables.

---

### 9.4 Overall F-Test

> Tests whether the regression model as a WHOLE is significant.

$$H_0: \beta_1 = \beta_2 = \cdots = \beta_k = 0 \qquad H_1: \text{at least one } \beta_j \neq 0$$

$$F = \frac{MSR}{MSE} = \frac{SSR/k}{SSE/(n-k-1)}$$

| Symbol | Meaning |
|--------|---------|
| **MSR** | Mean Squared Regression = SSR/k |
| **MSE** | Mean Squared Error = SSE/(n−k−1) |
| **k** | Number of predictors |
| **n−k−1** | Error degrees of freedom |

> Reject H₀ if F > F*_(k, n−k−1) from F-table, or if p-value < α.

---

### 9.5 t-Test for Individual Predictors

$$t = \frac{b_j}{SE(b_j)} \qquad df = n-k-1$$

$$95\% \text{ CI}: \quad b_j \pm t^*_{n-k-1} \times SE(b_j)$$

> If |t| > t* or p-value < α → that predictor is statistically significant.

---

## 10. Quick Reference Table

| Formula | Expression | Section |
|---------|-----------|---------|
| Relative Frequency | f / n | 1.1 |
| Approx. Class Width | (X_max − X_min) / No. of classes | 1.2 |
| Class Midpoint | (Lower + Upper) / 2 | 1.2 |
| Population Mean | μ = Σx_i / N | 2.1 |
| Sample Mean | x̄ = Σx_i / n | 2.1 |
| Grouped Mean | x̄ = Σ(m_i f_i) / n | 2.1 |
| Geometric Mean | GM = (x₁×x₂×...×xₙ)^(1/n) | 2.2 |
| Harmonic Mean | HM = n / Σ(1/x_i) | 2.3 |
| Median (grouped) | L + [(n/2 − F)/f] × C | 2.4 |
| Range | R = X_max − X_min | 3.1 |
| Quartile Deviation | QD = (Q₃ − Q₁) / 2 | 3.2 |
| Mean Deviation | MD = Σ\|x − x̄\| / n | 3.3 |
| Population Variance | σ² = Σ(x−μ)² / N | 3.4 |
| Sample Variance | s² = Σ(x−x̄)² / (n−1) | 3.4 |
| Variance Shortcut | [Σx²−(Σx)²/n] / (n−1) | 3.4 |
| Standard Deviation | σ = √σ² | 3.4 |
| Coeff. of Variation | CV = (σ/μ) × 100 | 3.5 |
| Quartile (grouped) | Q_k = L + [(kn/4−F)/f] × C | 4.2 |
| Percentile (grouped) | P_k = L + [(kn/100−F)/f] × C | 4.2 |
| r-th Moment | m_r = Σ(x−x̄)^r / n | 5.1 |
| Skewness | β₁ = m₃² / m₂³ | 5.2 |
| Kurtosis | β₂ = m₄ / m₂² | 5.3 |
| Standard Error | σ_x̄ = σ / √n | 6.1 |
| Z-score (CLT) | Z = (x̄ − μ) / σ_x̄ | 6.2 |
| Pearson r (shortcut) | [nΣxy − ΣxΣy] / √{[nΣx²−(Σx)²][nΣy²−(Σy)²]} | 7.1 |
| Spearman R | 1 − 6Σd² / [n(n²−1)] | 7.2 |
| Reg. slope b_yx | [nΣxy − ΣxΣy] / [nΣx²−(Σx)²] | 8.1 |
| Reg. intercept a | ȳ − b_yx × x̄ | 8.1 |
| r from regression | r = √(b_yx × b_xy) | 8.3 |
| Multiple R²₁.₂₃ | (r₁₂²+r₁₃²−2r₁₂r₁₃r₂₃) / (1−r₂₃²) | 9.2 |
| R-squared | SSR/SST = 1−SSE/SST | 9.3 |
| Adjusted R² | 1−(1−R²)(n−1)/(n−k−1) | 9.3 |
| F-statistic | MSR/MSE | 9.4 |
| t for b_j | b_j / SE(b_j), df=n−k−1 | 9.5 |

---

*DS 107 Formula Reference Notes — Generated from Lecture Materials*
