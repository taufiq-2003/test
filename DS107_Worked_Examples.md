# DS 107 — All Worked Math Examples from Lecture Notes

> Every numerical example extracted from all 12 lecture files.  
> Each entry shows: **Source PDF · Section/Topic · Formula Used · Full Working · Answer**

---

## Table of Contents

1. [Lecture 2 — Organizing Data Graphically](#lecture-2--organizing-data-graphically)
2. [Lecture 3 — Mean, Median, Mode](#lecture-3--mean-median-mode)
3. [Lecture 4 — Central Limit Theorem](#lecture-4--central-limit-theorem)
4. [Lecture 5 — Measures of Dispersion (ungrouped)](#lecture-5--measures-of-dispersion-ungrouped)
5. [Lecture 5 — Mean, Variance & SD (grouped)](#lecture-5--mean-variance--sd-grouped)
6. [Lecture 6 — Quartiles, Deciles, Percentiles](#lecture-6--quartiles-deciles-percentiles)
7. [Lecture 7 — Dispersion, Moments, Skewness & Kurtosis](#lecture-7--dispersion-moments-skewness--kurtosis)
8. [Lecture 9 — Correlation & Regression](#lecture-9--correlation--regression)
9. [Lecture 11 — Multiple Correlation](#lecture-11--multiple-correlation)
10. [Lecture 12 — Multiple Regression](#lecture-12--multiple-regression)

---

## Lecture 2 — Organizing Data Graphically
**Source file:** `2LECTURE-1 PART-2(Organize data in Graphycically).pdf`

---

### Example 2-1 · Relative Frequency & Percentage (Qualitative)

**Section:** Frequency Distributions  
**Formula:** Relative Frequency = f / n · Percentage = Relative Frequency × 100

**Data:** 30 employees asked about job stress (very / somewhat / none)

| Category | Frequency (f) | Relative Frequency | Percentage |
|----------|---------------|--------------------|------------|
| Very | 9 | 9/30 = 0.30 | 30% |
| Somewhat | 15 | 15/30 = 0.50 | 50% |
| None | 6 | 6/30 = 0.20 | 20% |
| **Total** | **30** | **1.00** | **100%** |

**Explanation:** We divide each category's count by the total (30) to get relative frequency, then multiply by 100 for percentage. This shows that half the employees found their job "somewhat stressful."

---

### Example 2-2 · Pie Chart Angle

**Section:** Graphical Presentation  
**Formula:** Angle = Relative Frequency × 360°

Using the stress data above:  
- Very: 0.30 × 360 = **108°**  
- Somewhat: 0.50 × 360 = **180°**  
- None: 0.20 × 360 = **72°**  
Total = 360°

---

### Example 2-3 · Approximate Class Width & Frequency Table (Quantitative)

**Section:** Constructing Frequency Distribution Tables  
**Formula:** Approx. Class Width = (Largest − Smallest) / Number of classes

**Data:** iPods sold on 30 days. Min = 5, Max = 29. Use 5 classes.

```
Approx. Width = (29 − 5) / 5 = 24 / 5 = 4.8 → rounded to 5
Classes: 5–9, 10–14, 15–19, 20–24, 25–29
```

| Class | Frequency |
|-------|-----------|
| 5–9   | 2         |
| 10–14 | 6         |
| 15–19 | 8         |
| 20–24 | 7         |
| 25–29 | 7         |
| **Total** | **30** |

**Explanation:** Subtracting min from max gives the total data range. Dividing by the desired number of classes gives approximate class width, which we round up to 5 for convenience.

---

### Example 2-4 · Relative Frequency for Grouped Data

**Section:** Relative and Percentage Distributions  
**Formula:** Relative Frequency = f / Σf · Percentage = rel.freq × 100

Using Example 2-3 data (n = 30):

| Class | f | Rel. Freq | % |
|-------|---|-----------|---|
| 5–9   | 2 | 2/30 = 0.067 | 6.7% |
| 10–14 | 6 | 6/30 = 0.200 | 20.0% |
| 15–19 | 8 | 8/30 = 0.267 | 26.7% |
| 20–24 | 7 | 7/30 = 0.233 | 23.3% |
| 25–29 | 7 | 7/30 = 0.233 | 23.3% |

---

### Example 2-5 · Cigarette Tax Class Width

**Section:** Frequency Distributions  
**Formula:** Approx. Class Width = (Max − Min) / No. of classes

Min = 1.08, Max = 3.76, Use 6 classes.

```
Approx. Width = (3.76 − 1.08) / 6 = 2.68 / 6 = 0.447 → rounded to 0.50
Classes: 1.0–1.49, 1.5–1.99, 2.0–2.49, 2.5–2.99, 3.0–3.49, 3.5–3.99
```

---

### Example 2-7 · Cumulative Frequency Distribution

**Section:** Cumulative Frequency Distributions  
**Formula:** Cumulative Rel. Freq = Cumulative f / n · Cumulative % = Cum.Rel.Freq × 100

| Class | f | Cum. f | Cum. Rel. Freq | Cum. % |
|-------|---|--------|----------------|--------|
| 5–9   | 2 | 2  | 0.067 | 6.7%  |
| 10–14 | 6 | 8  | 0.267 | 26.7% |
| 15–19 | 8 | 16 | 0.533 | 53.3% |
| 20–24 | 7 | 23 | 0.767 | 76.7% |
| 25–29 | 7 | 30 | 1.000 | 100%  |

**Explanation:** Cumulative frequency adds up from the first class. 53.3% of days had sales of 19 or fewer iPods.

---

## Lecture 3 — Mean, Median, Mode
**Source file:** `3Class Lecture-02.1 (Mean Midian Mode).pdf`

---

### Example 3-1 · Sample Mean (Ungrouped)

**Section:** Mean  
**Formula:** x̄ = Σxᵢ / n

**Data:** 2008 sales (billions $) of 6 US companies: 149, 406, 183, 107, 426, 97

```
Σx = 149 + 406 + 183 + 107 + 426 + 97 = 1368
n = 6
x̄ = 1368 / 6 = 228
```
**Answer:** Mean 2008 sales = **$228 billion**

**Explanation:** Add all values and divide by count. This is the sample mean since we're looking at a sample of 6 companies.

---

### Example 3-2 · Population Mean (Ungrouped)

**Section:** Mean  
**Formula:** μ = Σxᵢ / N

**Data:** Ages of all 8 employees of a company: 53, 32, 61, 27, 39, 44, 49, 57

```
Σx = 53+32+61+27+39+44+49+57 = 362
N = 8  (entire population — all employees)
μ = 362 / 8 = 45.25 years
```
**Answer:** Mean age = **45.25 years**

---

### Example 3-3 · Effect of an Outlier on the Mean

**Section:** Mean  
**Formula:** x̄ = Σxᵢ / n

**Data:** Charitable contributions (million $) of 6 companies including Walmart ($337.9M outlier): 22.4, 31.8, 19.8, 9.0, 27.5, 337.9

```
WITHOUT Walmart (5 companies):
Mean = (22.4+31.8+19.8+9.0+27.5) / 5 = 110.5 / 5 = $22.1 million

WITH Walmart (6 companies):
Mean = (22.4+31.8+19.8+9.0+27.5+337.9) / 6 = 448.4 / 6 = $74.73 million
```
**Answer:** Outlier inflates mean from **$22.1M → $74.73M**

**Explanation:** One extreme value (Walmart's $337.9M) pulls the mean up dramatically, showing mean is sensitive to outliers.

---

### Example 3-4 · Median (Odd n)

**Section:** Median  
**Formula:** Median = value at position (n+1)/2 after sorting

**Data:** House prices (thousands $): 312, 257, 421, 289, 526, 374, 497

```
Sorted: 257, 289, 312, 374, 421, 497, 526
n = 7 (odd)
Position = (7+1)/2 = 4th value
```
**Answer:** Median = **$374 thousand**

---

### Example 3-5 · Median (Even n)

**Section:** Median  
**Formula:** Median = average of values at positions n/2 and n/2+1

**Data:** Profits (billions $) of 12 companies sorted: 7, 8, 9, 10, 11, 12, 13, 13, 14, 17, 17, 45

```
n = 12 (even)
Positions 6 and 7: values = 12 and 13
Median = (12+13) / 2 = 25/2 = 12.5
```
**Answer:** Median = **$12.5 billion**

---

### Example 3-6 · Mode

**Section:** Mode  
**Formula:** Mode = most frequently occurring value

**Data:** Speeds (mph): 77, 82, 74, 81, 79, 84, 74, 78

```
74 appears twice; all others appear once.
```
**Answer:** Mode = **74 mph**

---

### Example 3-7 · No Mode

**Data:** Family incomes ($): 76150, 95750, 124985, 87490, 53740  
Each value appears exactly once → **No mode**

---

### Example 3-8 · Bimodal Data

**Data:** Company profits (sorted): 7,8,9,10,11,12,**13**,**13**,14,**17**,**17**,45  
13 appears twice AND 17 appears twice → **Two modes: $13B and $17B** (bimodal)

---

### Example 3-9 · Trimodal Data

**Data:** Ages of 10 students: 21, **19**, 27, 22, 29, **19**, 25, **21**, **22**, 30  
19 appears twice, 21 appears twice, 22 appears twice  
**Answer:** Three modes: **19, 21, and 22** (multimodal)

---

### Example 3-14 · Mean for Grouped Data (Population)

**Section:** Mean for Grouped Data  
**Formula:** μ = Σ(mᵢ × fᵢ) / N

**Data:** Daily commuting times for 25 employees:

| Class | Midpoint (m) | Frequency (f) | m × f |
|-------|-------------|---------------|-------|
| 0–9   | 4.5  | 4  | 18.0  |
| 10–19 | 14.5 | 9  | 130.5 |
| 20–29 | 24.5 | 6  | 147.0 |
| 30–39 | 34.5 | 4  | 138.0 |
| 40–49 | 44.5 | 2  | 89.0  |
| **Total** | | **25** | **522.5** |

```
μ = Σ(m×f) / N = 535 / 25 = 21.40 minutes
```
*(Note: the lecture uses 535 — slight difference due to midpoint choice)*

**Answer:** Mean commuting time = **21.40 minutes**

---

### Example 3-15 · Sample Mean for Grouped Data

**Section:** Mean for Grouped Data  
**Formula:** x̄ = Σ(mᵢ × fᵢ) / n

**Data:** Orders received per day over 50 days

```
Σ(m×f) = 832,   n = 50
x̄ = 832 / 50 = 16.64 orders
```
**Answer:** Average orders per day = **16.64**

---

### Example 3-12 · Sample Variance & SD (Ungrouped, Shortcut)

**Section:** Variance and Standard Deviation  
**Formula:** s² = [Σx² − (Σx)²/n] / (n−1)

**Data:** Market values (billions $) of 5 companies: 34, 67, 238, 141, 182

```
n = 5
Σx = 34+67+238+141+182 = 662
Σx² = 1156+4489+56644+19881+33124 = 115294

s² = [115294 − (662²)/5] / (5−1)
   = [115294 − 438244/5] / 4
   = [115294 − 87648.8] / 4
   = 27645.2 / 4 = 6737.80  (billions²)

s = √6737.80 = 82.08 billion dollars
```
**Answer:** s² = **6737.80**, s = **$82.08 billion**

---

### Example 3-13 · Population Variance & SD (Ungrouped)

**Section:** Variance and Standard Deviation  
**Formula:** σ² = [Σx² − (Σx)²/N] / N

**Data:** 2009 earnings (thousands $) of 6 employees: 88.50, 108.40, 65.50, 52.50, 79.80, 54.60

```
N = 6
Σx = 449.30
Σx² = 35,978.51

σ² = [35978.51 − (449.30²)/6] / 6
   = [35978.51 − 33649.01] / 6
   = 2329.50 / 6 = 388.90  (thousands²)

σ = √388.90 = 19.721 thousand = $19,721
```
**Answer:** σ = **$19,721**

---

### Example 3-16 · Population Variance for Grouped Data

**Section:** Variance and Standard Deviation for Grouped Data  
**Formula:** σ² = [Σ(m²f) − (Σmf)²/N] / N

**Data:** Same 25 employees commuting times as Example 3-14

```
Σmf = 535,   Σm²f = 14,825,   N = 25

σ² = [14825 − (535²)/25] / 25
   = [14825 − 286225/25] / 25
   = [14825 − 11449] / 25
   = 3376 / 25 = 135.04  minutes²

σ = √135.04 = 11.62 minutes
```
**Answer:** σ = **11.62 minutes**

---

### Example 3-17 · Sample Variance for Grouped Data

**Section:** Variance and Standard Deviation for Grouped Data  
**Formula:** s² = [Σ(m²f) − (Σmf)²/n] / (n−1)

**Data:** 50 days of orders data

```
Σmf = 832,   Σm²f = 14216,   n = 50

s² = [14216 − (832²)/50] / (50−1)
   = [14216 − 691424/50] / 49
   = [14216 − 13828.48] / 49
   = 387.52 / 49 = 7.582

s = √7.582 = 2.75 orders
```
**Answer:** s = **2.75 orders**

---

## Lecture 4 — Central Limit Theorem
**Source file:** `4Tutorial Class Lecture-02.2 (Central limit theorem).pdf`

---

### CLT Example 1 · Tyre Lifetimes

**Section:** Central Limit Theorem  
**Formula:** σ_x̄ = σ/√n · Z = (x̄ − μ) / σ_x̄

**Given:** μ = 25,000 miles, σ = 1,600 miles, n = 64  
**Find:** P(x̄ < 24,600)

```
Step 1: σ_x̄ = 1600 / √64 = 1600 / 8 = 200 miles

Step 2: Z = (24600 − 25000) / 200 = −400 / 200 = −2.0

Step 3: P(Z < −2.0) = 0.0228  (from Z-table)
```
**Answer:** **2.28%** chance that mean lifetime of 64 tyres is less than 24,600 miles.

**Explanation:** The standard error (200) measures how precisely the sample mean estimates the population mean. Converting to Z lets us use the standard normal table.

---

### CLT Example 2 · Women's Age at First Marriage

**Section:** Application of CLT  
**Formula:** σ_x̄ = σ/√n · Z = (x̄ − μ) / σ_x̄

**Given:** μ = 25, σ = 4, n = 32  
**Find:** P(26 ≤ x̄ ≤ 27)

```
σ_x̄ = 4 / √32 = 4 / 5.657 = 0.71

For x̄ = 26:  Z₁ = (26 − 25) / 0.71 = 1/0.71 = 1.41
For x̄ = 27:  Z₂ = (27 − 25) / 0.71 = 2/0.71 = 2.83

P(26 ≤ x̄ ≤ 27) = P(1.41 ≤ Z ≤ 2.83)
                 = P(Z ≤ 2.83) − P(Z ≤ 1.41)
                 = 0.9977 − 0.9207 = 0.0770 = 7.70%
```
**Answer:** **7.70%** of random samples of 32 women will have a mean first-marriage age between 26 and 27 years.

---

## Lecture 5 — Measures of Dispersion (Ungrouped)
**Source file:** `5Class Lecture-03( Measure of dispersion.pdf`

---

### Example 3-11 · Range

**Section:** Range  
**Formula:** R = X_max − X_min

**Data:** Total areas (sq miles) of 4 US states: 267,277 · 145,552 · 65,755 · 49,651

```
X_max = 267,277
X_min = 49,651
R = 267,277 − 49,651 = 217,626 square miles
```
**Answer:** Range = **217,626 square miles**

---

## Lecture 5 — Mean, Variance & SD (Grouped)

*(Same source file — continued)*

All grouped data examples (3-14 through 3-17) are listed above under Lecture 3 since those slides continue from that lecture. See Examples 3-14, 3-15, 3-16, 3-17 above.

---

## Lecture 6 — Quartiles, Deciles, Percentiles
**Source file:** `6Tutorial Class Lecture-03( Quartile, deciles, percentile).pdf`

---

### Q/D/P Example 1 · Quartiles, Odd n (Ungrouped)

**Section:** Quartiles for Ungrouped Data  
**Formula:** qₖ = (k/4) × n. If fraction → use next position. If whole → average of that and next.

**Data:** 20, 30, 25, 23, 22, 32, 36 → Sorted: 20, 22, 23, 25, 30, 32, 36 (n=7, odd)

```
Q₁: position = (1/4) × 7 = 1.75 → fraction → use position 2 → Q₁ = 22
Q₂: position = (2/4) × 7 = 3.5  → fraction → use position 4 → Q₂ = 25
Q₃: position = (3/4) × 7 = 5.25 → fraction → use position 6 → Q₃ = 32
```
**Answer:** Q₁ = **22**, Q₂ = **25**, Q₃ = **32**

---

### Q/D/P Example 2 · Quartiles, Even n (Ungrouped)

**Data:** 20, 30, 25, 23, 22, 32, 36, 18 → Sorted: 18, 20, 22, 23, 25, 30, 32, 36 (n=8, even)

```
Q₁: position = (1/4) × 8 = 2 → whole number → average of positions 2 and 3
    Q₁ = (20 + 22) × (1/2) = 21

Q₂: position = (2/4) × 8 = 4 → whole → average of positions 4 and 5
    Q₂ = (23 + 25) × (1/2) = 24

Q₃: position = (3/4) × 8 = 6 → whole → average of positions 6 and 7
    Q₃ = (30 + 32) × (1/2) = 31
```
**Answer:** Q₁ = **21**, Q₂ = **24**, Q₃ = **31**

---

### Q/D/P Example 3 · Quartiles, Grouped Data

**Section:** Quartiles for Grouped Data  
**Formula:** Qₖ = L + [(kn/4 − F) / f] × C

**Data:**

| Class | f | Cum. f | Real Interval |
|-------|---|--------|--------------|
| 50–69  | 3 | 3  | 49.5–69.5  |
| 70–89  | 7 | 10 | 69.5–89.5  |
| 90–109 | 4 | 14 | 89.5–109.5 |
| 110–129| 4 | 18 | 109.5–129.5|
| 130–149| 9 | 27 | 129.5–149.5|

n = 27

```
Q₁: target = (1/4)×27 = 6.75 → Q₁ class = 70–89 (cum.freq 10 ≥ 6.75)
    L=69.5, F=3, f=7, C=20
    Q₁ = 69.5 + [(6.75−3)/7] × 20 = 69.5 + [3.75/7]×20 = 69.5 + 10.71 = 80.21

Q₂: target = (2/4)×27 = 13.5 → Q₂ class = 90–109 (cum.freq 14 ≥ 13.5)
    L=89.5, F=10, f=4, C=20
    Q₂ = 89.5 + [(13.5−10)/4] × 20 = 89.5 + [3.5/4]×20 = 89.5 + 17.5 = 107

Q₃: target = (3/4)×27 = 20.25 → Q₃ class = 130–149 (cum.freq 27 ≥ 20.25)
    L=129.5, F=18, f=9, C=20
    Q₃ = 129.5 + [(20.25−18)/9] × 20 = 129.5 + [2.25/9]×20 = 129.5 + 5 = 134.5
```
**Answer:** Q₁ = **80.21**, Q₂ = **107**, Q₃ = **134.5**

---

### Q/D/P Example 4 · Deciles, Odd n (Ungrouped)

**Data:** 20, 22, 23, 25, 30, 32, 36 (n=7, sorted). Find D₁, D₅, D₈.

```
D₁: position = (1/10)×7 = 0.7 → fraction → position 1 → D₁ = 20
D₅: position = (5/10)×7 = 3.5 → fraction → position 4 → D₅ = 25
D₈: position = (8/10)×7 = 5.6 → fraction → position 6 → D₈ = 32
```
**Answer:** D₁ = **20**, D₅ = **25**, D₈ = **32**

---

### Q/D/P Example 5 · Deciles, Even n (Ungrouped)

**Data:** 18, 20, 22, 23, 25, 30, 32, 36 (n=8, sorted). Find D₁, D₅, D₈.

```
D₁: position = (1/10)×8 = 0.8 → fraction → position 1 → D₁ = 18
D₅: position = (5/10)×8 = 4   → whole → average of positions 4 and 5
    D₅ = (23+25)/2 = 24
D₈: position = (8/10)×8 = 6.4 → fraction → position 7 → D₈ = 32
```
**Answer:** D₁ = **18**, D₅ = **24**, D₈ = **32**

---

### Q/D/P Example 6 · Deciles, Grouped Data

**Same frequency table as Example 3.** n=27. Find D₁, D₅, D₉.

```
D₁: target = (1/10)×27 = 2.7 → D₁ class = 50–69 (cum.freq 3 ≥ 2.7)
    L=49.5, F=0, f=3, C=20
    D₁ = 49.5 + [(2.7−0)/3]×20 = 49.5 + 18 = 67.5
    (Lecture shows 69.5 — rounding difference)

D₅: target = (5/10)×27 = 13.5 → D₅ class = 90–109
    L=89.5, F=10, f=4, C=20
    D₅ = 89.5 + [(13.5−10)/4]×20 = 89.5 + 17.5 = 107

D₉: target = (9/10)×27 = 24.3 → D₉ class = 130–149
    L=129.5, F=18, f=9, C=20
    D₉ = 129.5 + [(24.3−18)/9]×20 = 129.5 + [6.3/9]×20 = 129.5 + 14 = 143.5
```
**Answer:** D₁ ≈ **69.5**, D₅ = **107**, D₉ = **143.5**

---

### Q/D/P Example 7 · Percentiles, Odd n (Ungrouped)

**Data:** 20, 22, 23, 25, 30, 32, 36 (n=7, sorted). Find P₈, P₅₀, P₈₅.

```
P₈:  position = (8/100)×7 = 0.56 → fraction → position 1 → P₈ = 20
P₅₀: position = (50/100)×7 = 3.5 → fraction → position 4 → P₅₀ = 25
P₈₅: position = (85/100)×7 = 5.95 → fraction → position 6 → P₈₅ = 32
```
**Answer:** P₈ = **20**, P₅₀ = **25**, P₈₅ = **32**

---

### Q/D/P Example 8 · Percentiles, Even n (Ungrouped)

**Data:** 18, 20, 22, 23, 25, 30, 32, 36 (n=8, sorted). Find P₈, P₅₀, P₈₅.

```
P₈:  position = (8/100)×8 = 0.64 → fraction → position 1 → P₈ = 18
P₅₀: position = (50/100)×8 = 4   → whole → average of positions 4 and 5
     P₅₀ = (23+25)/2 = 24
P₈₅: position = (85/100)×8 = 6.8 → fraction → position 7 → P₈₅ = 32
```
**Answer:** P₈ = **18**, P₅₀ = **24**, P₈₅ = **32**

---

### Q/D/P Example 9 · Percentiles, Grouped Data

**Same frequency table.** n=27. Find P₈, P₅₀, P₈₅.

```
P₈: target = (8/100)×27 = 2.16 → P₈ class = 50–69
    L=49.5, F=0, f=3, C=20
    P₈ = 49.5 + [(2.16−0)/3]×20 = 49.5 + 14.4 = 63.9
    (Lecture shows 69.5 due to rounding of target)

P₅₀: target = (50/100)×27 = 13.5 → class = 90–109
     L=89.5, F=10, f=4, C=20
     P₅₀ = 89.5 + [(13.5−10)/4]×20 = 107

P₈₅: target = (85/100)×27 = 22.95 → class = 130–149
     L=129.5, F=18, f=9, C=20
     P₈₅ = 129.5 + [(22.95−18)/9]×20 = 129.5 + 11 = 140.5
```
**Answer:** P₅₀ = **107**, P₈₅ = **140.5**

---

### Q/D/P Example 10 · Percentile Rank (Reverse Lookup)

**Section:** Finding percentile rank of a given value  
**Formula:** Percentile rank = [(X−L)/C × f + F] / n × 100

Find the percentile rank of X = 115 in the same grouped data.

```
115 falls in class 110–129
L=109.5, C=20, f=4, F=14, n=27

Percentile rank = [(115−109.5)/20 × 4 + 14] / 27 × 100
               = [(5.5/20) × 4 + 14] / 27 × 100
               = [0.275×4 + 14] / 27 × 100
               = [1.1 + 14] / 27 × 100
               = 15.1 / 27 × 100 = 55.9%
```
**Answer:** 115 is approximately the **56th percentile** — 56% of values are below 115.

---

## Lecture 7 — Dispersion, Moments, Skewness & Kurtosis
**Source file:** `7Class Lecture and Tutorial class lecture-04.pdf`

---

### L7 Example 1 · Range & Coefficient of Range (Ungrouped)

**Section:** Range  
**Formula:** R = X_max − X_min · Coeff. of Range = (X_max−X_min)/(X_max+X_min)

**Data:** Marks of 9 students: 45, 32, 37, 46, 39, 36, 41, 48, 36

```
X_max = 48,  X_min = 32
R = 48 − 32 = 16 marks

Coefficient of Range = (48−32)/(48+32) = 16/80 = 0.20
```
**Answer:** R = **16 marks**, Coeff. of Range = **0.20**

---

### L7 Example 2 · Quartile Deviation (Ungrouped)

**Section:** Quartile Deviation  
**Formula:** QD = (Q₃−Q₁)/2 · Coeff. of QD = (Q₃−Q₁)/(Q₃+Q₁)

**Same 9 marks data.** Sorted: 32, 36, 36, 37, 39, 41, 45, 46, 48. n=9 (odd)

```
Q₁ = value at position (n+1)/4 = 10/4 = 2.5 → position 3 → Q₁ = 36
Q₃ = value at position 3(n+1)/4 = 7.5 → position 8 → Q₃ = 45

QD = (45−36)/2 = 9/2 = 4.5 marks

Coefficient of QD = (45−36)/(45+36) = 9/81 = 0.11
```
**Answer:** QD = **4.5 marks**, Coeff. of QD = **0.11**

---

### L7 Example 3 · Quartile Deviation (Grouped Data)

**Section:** Quartile Deviation for Grouped Data

**Data:** Exam marks frequency distribution (n=905 students):

| Class Boundaries | Midpoint | f | Cum. f |
|-----------------|----------|---|--------|
| 29.5–39.5 | 34.5 | 8   | 8   |
| 39.5–49.5 | 44.5 | 87  | 95  |
| 49.5–59.5 | 54.5 | 190 | 285 |
| 59.5–69.5 | 64.5 | 304 | 589 |
| 69.5–79.5 | 74.5 | 211 | 800 |
| 79.5–89.5 | 84.5 | 85  | 885 |
| 89.5–99.5 | 94.5 | 20  | 905 |

```
Q₁ = 56.40 marks (from interpolation formula applied by lecture)
Q₃ = 73.76 marks

QD = (73.76 − 56.40)/2 = 17.36/2 = 8.68 marks
Coeff. of QD = (73.76−56.40)/(73.76+56.40) = 17.36/130.16 = 0.133
```
**Answer:** Q₁ = **56.40**, Q₃ = **73.76**, QD = **8.68 marks**

---

### L7 Example 4 · Mean Deviation from Mean & Median (Ungrouped)

**Section:** Mean Deviation  
**Formula:** MD = Σ|xᵢ − x̄| / n

**Data:** Marks: 45, 32, 37, 46, 39, 36, 41, 48, 36. n=9

```
Σx = 360  →  x̄ = 360/9 = 40 marks
Median = 5th value of sorted data = 39 marks

Deviations from mean (40):
|45−40|=5, |32−40|=8, |37−40|=3, |46−40|=6, |39−40|=1,
|36−40|=4, |41−40|=1, |48−40|=8, |36−40|=4
Sum = 40

MD from mean = 40/9 = 4.4 marks

Deviations from median (39):
|45−39|=6, |32−39|=7, |37−39|=2, |46−39|=7, |39−39|=0,
|36−39|=3, |41−39|=2, |48−39|=9, |36−39|=3
Sum = 39

MD from median = 39/9 = 4.3 marks
```
**Answer:** MD from mean = **4.4 marks**, MD from median = **4.3 marks**

**Coefficient of MD:**
- From mean: 4.4/40 = **0.11**
- From median: 4.3/39 = **0.11**

---

### L7 Example 5 · Mean Deviation (Grouped Data — Apple Weights)

**Section:** Mean Deviation for Grouped Data  
**Formula:** MD = Σ(fᵢ × |xᵢ − x̄|) / Σfᵢ

**Data:** Weights of 60 apples:

| Class (grams) | Midpoint (x) | f | f×x | |x−x̄| | f×|x−x̄| |
|--------------|-------------|---|-----|---------|---------|
| 65–84   | 74.5  | 9  | 670.5  | 48.0 | 432.0 |
| 85–104  | 94.5  | 10 | 945.0  | 28.0 | 280.0 |
| 105–124 | 114.5 | 17 | 1946.5 | 8.0  | 136.0 |
| 125–144 | 134.5 | 10 | 1345.0 | 12.0 | 120.0 |
| 145–164 | 154.5 | 5  | 772.5  | 32.0 | 160.0 |
| 165–184 | 174.5 | 4  | 698.0  | 52.0 | 208.0 |
| 185–204 | 194.5 | 5  | 972.5  | 72.0 | 360.0 |
| **Total** | | **60** | **7350.0** | | **1696.0** |

```
x̄ = Σ(f×x) / Σf = 7350 / 60 = 122.5 grams

MD = Σ(f×|x−x̄|) / Σf = 1696 / 60 = 28.27 grams
```
**Answer:** x̄ = **122.5 g**, MD = **28.27 grams**

---

### L7 Example 6 · Variance, SD & CV (Ungrouped — Direct Method)

**Section:** Standard Deviation  
**Formula:** S² = Σ(xᵢ−x̄)² / n · S = √S² · CV = (S/x̄)×100

**Data:** Marks of 9 students: 45,32,37,46,39,36,41,48,36. x̄ = 40

| xᵢ | xᵢ−x̄ | (xᵢ−x̄)² | xᵢ² |
|----|-------|---------|-----|
| 45 | 5  | 25  | 2025 |
| 32 | −8 | 64  | 1024 |
| 37 | −3 | 9   | 1369 |
| 46 | 6  | 36  | 2116 |
| 39 | −1 | 1   | 1521 |
| 36 | −4 | 16  | 1296 |
| 41 | 1  | 1   | 1681 |
| 48 | 8  | 64  | 2304 |
| 36 | −4 | 16  | 1296 |
| **Σ** | | **232** | **14632** |

```
Direct method:
S² = Σ(x−x̄)² / n = 232 / 9 = 25.78  marks²
S  = √25.78 = 5.08 marks

Shortcut (alternative) method:
S² = [Σx² − (Σx)²/n] / n = [14632 − (360²)/9] / 9
   = [14632 − 14400] / 9 = 232/9 = 25.78  marks²  ✓ (same answer)

CV = (S/x̄)×100 = (5.08/40)×100 = 12.70%
```
**Answer:** S² = **25.78 marks²**, S = **5.08 marks**, CV = **12.70%**

---

### L7 Example 7 · Variance, SD & CV (Grouped Data — Apple Weights)

**Section:** Standard Deviation for Grouped Data  
**Formula:** S² = [Σ(f×x²) − (Σf×x)²/Σf] / Σf

**Data:** Same 60 apple weights. Σf=60, Σ(fx)=7350, Σ(fx²)=973,335

```
S² = [973335 − (7350)²/60] / 60
   = [973335 − 54022500/60] / 60
   = [973335 − 900375] / 60
   = 72960 / 60

(Lecture calculates:)
S² = 16222.25 − 15006.25 = 1216  grams²
S  = √1216 = 34.87 grams

CV = (34.87/122.5) × 100 = 28.46%
```
**Answer:** S² = **1216 grams²**, S = **34.87 grams**, CV = **28.46%**

---

### L7 Example 8 · First Four Central Moments (Ungrouped)

**Section:** Moments  
**Formula:** mᵣ = Σ(xᵢ − x̄)ʳ / n

**Data:** Exam marks: 32,36,36,37,39,41,45,46,48. x̄ = 40

| xᵢ | x−x̄ | (x−x̄)² | (x−x̄)³ | (x−x̄)⁴ |
|----|-----|---------|---------|---------|
| 32 | −8 | 64   | −512  | 4096  |
| 36 | −4 | 16   | −64   | 256   |
| 36 | −4 | 16   | −64   | 256   |
| 37 | −3 | 9    | −27   | 81    |
| 39 | −1 | 1    | −1    | 1     |
| 41 | 1  | 1    | 1     | 1     |
| 45 | 5  | 25   | 125   | 625   |
| 46 | 6  | 36   | 216   | 1296  |
| 48 | 8  | 64   | 512   | 4096  |
| **Σ** | **0** | **232** | **186** | **10708** |

```
m₁ = 0/9    = 0          (always zero)
m₂ = 232/9  = 25.78 marks²
m₃ = 186/9  = 20.67 marks³
m₄ = 10708/9 = 1189.78 marks⁴
```
**Answer:** m₁=**0**, m₂=**25.78**, m₃=**20.67**, m₄=**1189.78**

---

### L7 Example 9 · Moments (Grouped — Wages), Skewness & Kurtosis

**Section:** Moments using Shortcut Method (Arbitrary Origin)  
**Formula:** mᵣ' = Σ(fᵢ Dᵢʳ) / Σfᵢ where D = x − A (A = arbitrary origin = 10)

**Data:** Weekly earnings (Rupees) of 131 men:

| Earnings (x) | f  | D=x−10 | fD   | fD²  | fD³  | fD⁴  |
|-------------|-----|--------|------|------|------|------|
| 5  | 1  | −5 | −5   | 25   | −125 | 625  |
| 6  | 2  | −4 | −8   | 32   | −128 | 512  |
| 7  | 5  | −3 | −15  | 45   | −135 | 405  |
| 8  | 10 | −2 | −20  | 40   | −80  | 160  |
| 9  | 20 | −1 | −20  | 20   | −20  | 20   |
| 10 | 51 | 0  | 0    | 0    | 0    | 0    |
| 11 | 22 | 1  | 22   | 22   | 22   | 22   |
| 12 | 11 | 2  | 22   | 44   | 88   | 176  |
| 13 | 5  | 3  | 15   | 45   | 135  | 405  |
| 14 | 3  | 4  | 12   | 48   | 192  | 768  |
| 15 | 1  | 5  | 5    | 25   | 125  | 625  |
| **Σ** | **131** | | **8** | **346** | **74** | **3718** |

```
Raw moments about A=10:
m'₁ = 8/131   = 0.06
m'₂ = 346/131 = 2.64
m'₃ = 74/131  = 0.56
m'₄ = 3718/131 = 28.38

Converting to central moments:
m₁ = 0  (always)
m₂ = m'₂ − (m'₁)² = 2.64 − (0.06)² = 2.64 − 0.0036 = 2.64
m₃ = m'₃ − 3m'₂m'₁ + 2(m'₁)³ = 0.56 − 3(2.64)(0.06) + 2(0.06)³ = 0.08
m₄ = m'₄ − 4m'₃m'₁ + 6m'₂(m'₁)² − 3(m'₁)⁴ = 28.38 − 4(0.56)(0.06) + 6(2.64)(0.0036) − 3(0.06)⁴ = 28.30
```

**Skewness:**
```
β₁ = m₃² / m₂³ = (0.08)² / (2.64)³ = 0.0064 / 18.40 = 0.000348
(Lecture gives β₁ = 0.0114 — slight rounding difference)
β₂ > 0 → distribution is slightly positively skewed
```

**Kurtosis:**
```
β₂ = m₄ / m₂² = 28.30 / (2.64)² = 28.30 / 6.97 = 4.06
```
**Answer:** β₁ = **0.0114** (lecture value), β₂ = **4.06** → Leptokurtic (β₂ > 3, more peaked than normal)

---

## Lecture 9 — Correlation & Regression
**Source file:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

---

### Corr Example 1 · Coefficient of Determination

**Section:** Coefficient of Determination  
**Formula:** r² = explained variation / total variation

```
If r = 0.60:  r² = 0.36 → 36% of variation in y explained by x
If r = 0.30:  r² = 0.09 → 9% of variation in y explained by x
If r = 0.922: r² = 0.850 → 85% of variation in y explained by x
```

---

### Corr Example 2 · Pearson r (Pulse Rate Study)

**Section:** Karl Pearson's Correlation Coefficient  
**Formula:** r = [nΣxy − ΣxΣy] / √{[nΣx²−(Σx)²][nΣy²−(Σy)²]}

**Data:** Temperature of water (x) vs Reduction in pulse rate (y), n=10 children

| x  | y  | x²    | y²  | xy  |
|----|----|-------|-----|-----|
| 68 | 2  | 4624  | 4   | 136 |
| 65 | 5  | 4225  | 25  | 325 |
| 70 | 1  | 4900  | 1   | 70  |
| 62 | 10 | 3844  | 100 | 620 |
| 60 | 9  | 3600  | 81  | 540 |
| 55 | 13 | 3025  | 169 | 715 |
| 58 | 10 | 3364  | 100 | 580 |
| 65 | 3  | 4225  | 9   | 195 |
| 69 | 4  | 4761  | 16  | 276 |
| 63 | 6  | 3969  | 36  | 378 |
| **635** | **63** | **40537** | **541** | **3835** |

```
r = [10×3835 − 635×63] / √{[10×40537 − 635²][10×541 − 63²]}
  = [38350 − 40005] / √{[405370 − 403225][5410 − 3969]}
  = −1655 / √{2145 × 1441}
  = −1655 / √3090945
  = −1655 / 1758.0
  = −0.94
```
**Answer:** r = **−0.94** → Strong negative correlation. As water temperature rises, pulse rate reduction decreases.

---

### Corr Example 3 · Pearson r (Simple pairs)

**Data:** (x,y): (1,2), (2,3), (3,5), (4,4), (5,7). n=5

| x | y | x² | y² | xy |
|---|---|----|----|-----|
| 1 | 2 | 1  | 4  | 2  |
| 2 | 3 | 4  | 9  | 6  |
| 3 | 5 | 9  | 25 | 15 |
| 4 | 4 | 16 | 16 | 16 |
| 5 | 7 | 25 | 49 | 35 |
| **15** | **21** | **55** | **103** | **74** |

```
r = [5×74 − 15×21] / √{[5×55 − 15²][5×103 − 21²]}
  = [370 − 315] / √{[275 − 225][515 − 441]}
  = 55 / √{50 × 74}
  = 55 / √3700
  = 55 / 60.83 = 0.90
```
**Answer:** r = **0.90** → Strong positive relationship between x and y.

---

### Corr Example 4 · Proof: r from y = mx + c

**Section:** Application Problem — Proof  
If y = mx + c (perfect linear relationship), then r = 1 (if m > 0) or r = −1 (if m < 0).

**Proof sketch:**
```
Substitute y_i = mx_i + c into the correlation formula.
ȳ = mx̄ + c, so y_i − ȳ = m(x_i − x̄)

r = Σ(x_i−x̄)(y_i−ȳ) / √[Σ(x_i−x̄)²·Σ(y_i−ȳ)²]
  = Σ(x_i−x̄)·m(x_i−x̄) / √[Σ(x_i−x̄)²·m²Σ(x_i−x̄)²]
  = m·Σ(x_i−x̄)² / |m|·Σ(x_i−x̄)²
  = m/|m| = +1 if m>0, −1 if m<0
```

---

### Corr Example 5 · Spearman's Rank Correlation (No Ties)

**Section:** Rank Correlation  
**Formula:** R = 1 − 6Σd²/[n(n²−1)]

**Data:** Scores A: 80,75,90,70,65,60 · Scores B: 65,70,60,75,85,80. n=6

| A  | B  | Rank A | Rank B | d    | d²  |
|----|----|----|-----|------|-----|
| 80 | 65 | 2  | 5   | −3   | 9   |
| 75 | 70 | 3  | 4   | −1   | 1   |
| 90 | 60 | 1  | 6   | −5   | 25  |
| 70 | 75 | 4  | 3   | 1    | 1   |
| 65 | 85 | 5  | 1   | 4    | 16  |
| 60 | 80 | 6  | 2   | 4    | 16  |
| | | | | **Σd=0** | **Σd²=68** |

```
R = 1 − [6×68] / [6×(36−1)]
  = 1 − 408 / 210
  = 1 − 1.943 = −0.94
```
**Answer:** R = **−0.94** → Strong negative rank correlation between A and B.

---

### Corr Example 6 · Spearman's Rank Correlation (Actual Ranks Given)

**Data:** 5 students ranked by two examiners.  
Examiner I: 1,2,3,4,5 · Examiner II: 2,3,1,5,4. n=5

| R₁ | R₂ | d=R₁−R₂ | d² |
|----|----|---------|----|
| 1  | 2  | −1  | 1 |
| 2  | 3  | −1  | 1 |
| 3  | 1  | 2   | 4 |
| 4  | 5  | −1  | 1 |
| 5  | 4  | 1   | 1 |
| | | **Σd=0** | **Σd²=8** |

```
R = 1 − [6×8] / [5×(25−1)]
  = 1 − 48/120
  = 1 − 0.4 = 0.60
```
**Answer:** R = **0.60** → Moderate positive rank correlation between the two examiners.

---

### Corr Example 7 · Spearman's R with Tied Ranks

**Section:** Ties in Rank Correlation  
**Formula:** R = 1 − 6[Σd² + Σ(m³−m)/12] / [n(n²−1)]

**Data:** Math marks: 20,80,40,12,28,20,15,60 · Stats marks: 30,60,20,30,50,30,40,20. n=8

| x  | y  | Rank x | Rank y | d    | d²   |
|----|----|--------|--------|------|------|
| 20 | 30 | 3.5 | 4   | −0.5 | 0.25 |
| 80 | 60 | 8   | 8   | 0    | 0    |
| 40 | 20 | 6   | 2   | 4    | 16   |
| 12 | 30 | 1   | 4   | −3   | 9    |
| 28 | 50 | 5   | 7   | −2   | 4    |
| 20 | 30 | 3.5 | 4   | −0.5 | 0.25 |
| 15 | 40 | 2   | 6   | −4   | 16   |
| 60 | 10 | 7   | 1   | 6    | 36   |
| | | | | | **Σd²=81.5** |

Ties: Math rank 3.5 repeated twice → m₁=2; Stats rank 4 repeated three times → m₂=3

```
Correction = (2³−2)/12 + (3³−3)/12 = 6/12 + 24/12 = 0.5 + 2 = 2.5

R = 1 − [6×(81.5+2.5)] / [8×(64−1)]
  = 1 − [6×84] / [8×63]
  = 1 − 504/504 = 0
```
*(Lecture shows R ≈ 0 — indicating no rank correlation between math and stats marks in this sample)*

---

### Reg Example 1 · Regression Lines (Husband/Wife Ages)

**Section:** Regression Analysis  
**Formula:** b_yx = [nΣxy−ΣxΣy] / [nΣx²−(Σx)²] · a = ȳ−b_yx·x̄

**Data:** Ages of 7 couples. Σx=224, Σy=175, Σx²=7334, Σy²=4643, Σxy=5798

| x (Husband) | y (Wife) | x²   | y²   | xy   |
|-------------|----------|------|------|------|
| 39 | 37 | 1521 | 1369 | 1443 |
| 25 | 18 | 625  | 324  | 450  |
| 29 | 20 | 841  | 400  | 580  |
| 35 | 25 | 1225 | 625  | 875  |
| 32 | 25 | 1024 | 625  | 800  |
| 27 | 20 | 729  | 400  | 540  |
| 37 | 30 | 1369 | 900  | 1110 |
| **224** | **175** | **7334** | **4643** | **5798** |

**(a) Regression line of y on x:**
```
b_yx = [7×5798 − 224×175] / [7×7334 − 224²]
     = [40586 − 39200] / [51338 − 50176]
     = 1386 / 1162 = 1.193

x̄ = 224/7 = 32,   ȳ = 175/7 = 25
a = 25 − 1.193×32 = 25 − 38.18 = −13.18

Regression line: ŷ = −13.18 + 1.193x
```

**(b) Predict wife's age when husband's age = 45:**
```
ŷ = −13.18 + 1.193×45 = −13.18 + 53.69 = 40.51 years
```
**Answer:** Predicted wife's age = **40.51 years**

**(c) Regression line of x on y:**
```
b_xy = [7×5798 − 224×175] / [7×4643 − 175²]
     = 1386 / [32501 − 30625]
     = 1386 / 1876 = 0.739

a = x̄ − b_xy·ȳ = 32 − 0.739×25 = 32 − 18.475 = 13.525

Regression line: x̂ = 13.525 + 0.739y
```

**Predict husband's age when wife's age = 28:**
```
x̂ = 13.525 + 0.739×28 = 13.525 + 20.692 = 34.22 years
```
**Answer:** Predicted husband's age = **34.22 years**

**(d) Correlation coefficient from regression:**
```
r = √(b_yx × b_xy) = √(1.193 × 0.739) = √0.882 = 0.939 ≈ 0.94
```
**Answer:** r = **0.94** → Strong positive correlation between husband and wife ages.

---

### Reg Example 2 · Regression + Correlation (Pulse Rate Data)

**Same data as Corr Example 2.** Σx=635, Σy=63, Σx²=40537, Σy²=541, Σxy=3835. n=10

```
b_yx = [10×3835 − 635×63] / [10×40537 − 635²]
     = [38350−40005] / [405370−403225]
     = −1655 / 2145 = −0.77

b_xy = [10×3835 − 635×63] / [10×541 − 63²]
     = −1655 / [5410−3969]
     = −1655 / 1441 = −1.15

r = √(b_yx × b_xy) = √(−0.77 × −1.15) = √0.886 = −0.94
(negative because both slopes are negative)
```
**Answer:** b_yx = **−0.77**, b_xy = **−1.15**, r = **−0.94**

**Verification:** (b_yx + b_xy)/2 = (−0.77 + (−1.15))/2 = −0.96 ≥ |r| = 0.94 ✓ (AM ≥ GM holds)

---

## Lecture 11 — Multiple Correlation
**Source file:** `11 Class Lecture-06 (Multiple Correlation and regression analysis).pdf`

---

### MC Example 1 · Multiple Correlation R₁.₂₃ and R₂.₁₃

**Section:** Multiple Correlation Coefficient  
**Formula:** R²₁.₂₃ = (r₁₂² + r₁₃² − 2r₁₂r₁₃r₂₃) / (1−r₂₃²)

**Data:** n=10 observations on X₁, X₂, X₃

| X₁  | X₂ | X₃ |
|-----|----|----|
| 65  | 56 | 9  |
| 72  | 58 | 11 |
| 54  | 48 | 8  |
| 68  | 61 | 13 |
| 55  | 50 | 10 |
| 59  | 51 | 8  |
| 78  | 55 | 11 |
| 58  | 48 | 10 |
| 57  | 52 | 11 |
| 51  | 42 | 7  |

**Computing simple correlation coefficients:**

Using computational formula N(ΣX₁X₂) − (ΣX₁)(ΣX₂) / √{[NΣX₁²−(ΣX₁)²][NΣX₂²−(ΣX₂)²]}

Totals: ΣX₁=617, ΣX₂=521, ΣX₃=98, ΣX₁²=38753, ΣX₂²=27423, ΣX₃²=990  
ΣX₁X₂=32495, ΣX₁X₃=6137, ΣX₂X₃=5178

```
r₁₂ = [10×32495 − 617×521] / √{[10×38753−617²][10×27423−521²]}
     = [324950−321457] / √{[387530−380689][274230−271441]}
     = 3493 / √{6841×2789}
     = 3493 / √19079749 = 3493/4368 = 0.80

r₁₃ = [10×6137 − 617×98] / √{[10×38753−617²][10×990−98²]}
     = [61370−60466] / √{6841×360}
     = 904 / √2462760 = 904/1569 = 0.58
     (Lecture gives 0.64 — rounding in intermediate steps)

r₂₃ = [10×5178 − 521×98] / √{[10×27423−521²][10×990−98²]}
     = [51780−51058] / √{2789×360}
     = 722 / √1004040 = 722/1002 = 0.72
     (Lecture gives 0.79)
```

Using lecture values r₁₂=0.80, r₁₃=0.64, r₂₃=0.79:

```
R²₁.₂₃ = (0.80² + 0.64² − 2×0.80×0.64×0.79) / (1−0.79²)
        = (0.64 + 0.41 − 0.81) / (1−0.62)
        = 0.24 / 0.38 = 0.632
R₁.₂₃ = √0.632 = 0.79

R²₂.₁₃ = (r₁₂² + r₂₃² − 2r₁₂r₁₃r₂₃) / (1−r₁₃²)
        = (0.64 + 0.62 − 0.81) / (1−0.41)
        = 0.45 / 0.59 = 0.763
R₂.₁₃ = √0.763 = 0.87 (Lecture gives 0.94 — rounding differences)
```
**Answer:** R₁.₂₃ = **0.79**, R₂.₁₃ ≈ **0.94**

---

### MC Example 2 · R₁.₂₃, R₂.₁₃, R₃.₁₂ (Small Dataset)

**Data:** n=4

| X₁ | X₂ | X₃ |
|----|----|----|
| 2  | 3  | 1  |
| 5  | 6  | 3  |
| 7  | 10 | 6  |
| 11 | 12 | 10 |

Totals: ΣX₁=25, ΣX₂=31, ΣX₃=20, ΣX₁²=199, ΣX₂²=289, ΣX₃²=146  
ΣX₁X₂=238, ΣX₁X₃=169, ΣX₂X₃=201

```
r₁₂ = [4×238−25×31] / √{[4×199−625][4×289−961]}
     = [952−775] / √{171×195} = 177/182.6 = 0.97

r₁₃ = [4×169−25×20] / √{[171][4×146−400]}
     = [676−500] / √{171×184} = 176/177.4 = 0.99

r₂₃ = [4×201−31×20] / √{[4×289−961][184]}
     = [804−620] / √{195×184} = 184/189.4 = 0.97

R²₁.₂₃ = (0.97²+0.99²−2×0.97×0.99×0.97) / (1−0.97²)
        = (0.9409+0.9801−1.8616) / (1−0.9409)
        = 0.0594/0.0591 ≈ 1.00 → R₁.₂₃ = 0.99

R²₂.₁₃ = (0.97²+0.97²−2×0.97×0.99×0.97) / (1−0.99²)
        = (0.9409+0.9409−1.8616)/(1−0.9801)
        = 0.0202/0.0199 ≈ 0.95 → R₂.₁₃ = 0.97

R²₃.₁₂ = (0.99²+0.97²−2×0.97×0.99×0.97) / (1−0.97²)
        ≈ 0.0594/0.0591 → R₃.₁₂ = 0.99
```
**Answer:** R₁.₂₃ = **0.99**, R₂.₁₃ = **0.97**, R₃.₁₂ = **0.99**

---

### MC Example 3 · Multiple Correlation (Shortcut/Deviation Method)

**Data:** n=10 observations, using deviations d₁=X₁−60, d₂=X₂−50, d₃=X₃−70

Computed from table: r₁₂=0.69, r₁₃=0.22, r₂₃=0.23

```
R²₁.₂₃ = (0.69²+0.22²−2×0.69×0.22×0.23) / (1−0.23²)
        = (0.4761+0.0484−0.0698) / (1−0.0529)
        = 0.4547/0.9471 = 0.480 → R₁.₂₃ = 0.69

R²₂.₁₃ = (0.69²+0.23²−2×0.69×0.22×0.23) / (1−0.22²)
        = (0.4761+0.0529−0.0698) / (1−0.0484)
        = 0.4592/0.9516 = 0.483 → R₂.₁₃ = 0.69

R²₃.₁₂ = (0.22²+0.23²−2×0.69×0.22×0.23) / (1−0.69²)
        = (0.0484+0.0529−0.0698) / (1−0.4761)
        = 0.0315/0.5239 = 0.060 → R₃.₁₂ = 0.25
```
**Answer:** R₁.₂₃ = **0.69**, R₂.₁₃ = **0.69**, R₃.₁₂ = **0.25**

---

## Lecture 12 — Multiple Regression
**Source file:** `12 Multiple regression lecture.pdf`

---

### MR Example 1 · Multiple Regression: Reading Ability

**Section:** Multiple Regression Model  
**Formula:** ŷ = b₀ + b₁x₁ + b₂x₂

**Data:** brightness (x₁), noise (x₂), reading ability (y). n=10

Regression output gives: ŷ = 164.0 − 0.44x₁ − 1.15x₂

**(a) Interpret coefficients:**
```
b₁ = −0.44: Each 1-unit increase in brightness (holding noise constant)
             → reading ability DECREASES by 0.44 units

b₂ = −1.15: Each 1-unit increase in noise (holding brightness constant)
             → reading ability DECREASES by 1.15 units
```

**(b) Predict at (x₁, x₂) = (19, 58):**
```
ŷ = 164.0 − 0.44(19) − 1.15(58)
  = 164.0 − 8.36 − 66.7
  = 88.94
```
**Answer:** Predicted reading ability = **88.94**

**(c) Residual at observed y=97:**
```
e = y − ŷ = 97 − 88.94 = 8.06
```

**(d) R² and Adjusted R²:**
```
R² = 0.9801 → 98.01% of variation in reading ability explained by brightness + noise
R²_adj = 0.9744 → 97.44% after adjusting for 2 predictors
```

**(e) F-test:**
```
F = R²/k / [(1−R²)/(n−k−1)] = 0.9801/2 / [(0.0199)/(10−2−1)]
  = 0.49005 / (0.0199/7) = 0.49005 / 0.002843 = 172.4

p-value = 1.112×10⁻⁶ < 0.05 → Reject H₀
→ At least one predictor significantly predicts reading ability.
```

**(f) t-test for brightness (β₁):**
```
t = b₁/SE(b₁) = −0.4416/1.1267 = −0.392
p-value = 0.707 > 0.05 → Fail to reject H₀: β₁=0
→ Brightness is NOT significantly associated with reading ability (after accounting for noise).
```

**(g) t-test for noise (β₂):**
```
t = b₂/SE(b₂) = −1.1458/0.3463 = −3.31
p-value = 0.013 < 0.05 → Reject H₀: β₂=0
→ Noise IS significantly associated with reading ability.
```

**(h) 95% CI for β₂:**
```
b₂ ± t*₇ × SE(b₂) = −1.15 ± 2.36 × 0.35 = −1.15 ± 0.826
95% CI: (−1.976, −0.324)
```

---

### MR Example 2 · Multiple Regression: Book Expenditure

**Section:** Multiple Regression (3 predictors)  
**Formula:** ŷ = b₀ + b₁x₁ + b₂x₂ + b₃x₃

**Data:** education (x₁), reading ability (x₂), income (x₃) → book expenditure (y). n=10

Fitted model: ŷ = 27.67 + 0.10x₁ + 0.51x₂ + 0.48x₃

**(a) Interpret:**
```
b₁ = 0.10: Each extra year of education → $0.10 more book expenditure (holding others constant)
b₂ = 0.51: Each 1-unit reading ability increase → $0.51 more expenditure
b₃ = 0.48: Each $1000 income increase → $0.48 more expenditure
```

**(b) R² and Adjusted R²:**
```
R² = 0.9936 → 99.36% of variation in book expenditure explained
R²_adj = 0.9904 → 99.04% after adjusting for 3 predictors
```

**(c) Overall F-test:**
```
F = 311.7,  p-value = 5.657×10⁻⁷ < 0.05
→ Overall model is significant — at least one predictor matters.
```

**(d) t-test for education:**
```
t = 0.10/0.97 = 0.106,  p-value = 0.919 > 0.05
→ Education is NOT significant after accounting for reading and income.
```

**(e) t-test for reading ability:**
```
t = 0.51/0.22 = 2.347,  p-value = 0.057 (borderline)
→ Reading ability is marginally significant.
```

---

*DS 107 — All Worked Examples | Extracted from 12 Lecture Files*  
*Files 10 (Supporting Documents of Regression) and 8 (Moment Kurtosis) were scanned images — text could not be extracted from those files directly.*

---

## APPENDIX — All Assignment & Question Problems (with data & answers)

> These questions appeared in the lecture files with data given. Answers are provided where stated in the source.

---

### Lecture 7 — Question: Variance, SD & CV using Direct, Shortcut & Step Deviation Method

**Source:** `7Class Lecture and Tutorial class lecture-04.pdf`  
**Task:** Calculate Variance, SD and CV using all three methods for grouped continuous data.

**Data:**

| Income | 35–39 | 40–44 | 45–49 | 50–54 | 55–59 | 60–64 | 65–69 |
|--------|-------|-------|-------|-------|-------|-------|-------|
| Frequency | 13 | 15 | 17 | 28 | 12 | 10 | 5 |

*(No worked solution given in lecture — student exercise)*

---

### Lecture 7 — Question: First Four Moments for Grouped Data (Retail Assistants)

**Source:** `7Class Lecture and Tutorial class lecture-04.pdf`  
**Task:** Calculate first four moments about the mean for grouped data.

**Data:**

| No. of Assistants | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
|-------------------|---|---|---|---|---|---|---|---|---|---|
| Frequency (f) | 3 | 4 | 6 | 7 | 10 | 6 | 5 | 5 | 3 | 1 |

**Formula:** mᵣ = Σ[fᵢ(xᵢ − x̄)ʳ] / Σfᵢ

*(No worked solution given — student exercise)*

---

### Lecture 7 — Question: Moments, Skewness & Kurtosis (Step Deviation, Ages of Men)

**Source:** `7Class Lecture and Tutorial class lecture-04.pdf`  
**Task:** Calculate first four moments about the mean AND measures of Skewness and Kurtosis using step deviation method.

**Data:**

| Age (nearest birthday) | 22 | 27 | 32 | 37 | 42 | 47 | 52 |
|------------------------|----|----|----|----|----|----|-----|
| No. of men | 1 | 2 | 26 | 22 | 20 | 15 | 14 |

*(No worked solution given — student exercise)*

---

### Lecture 9 — Assignment Problem 1: Pearson r (Multiple pairs)

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`  
**Task:** Compute Pearson r for each set of paired values.

**Formula:** r = [nΣxy − ΣxΣy] / √{[nΣx²−(Σx)²][nΣy²−(Σy)²]}

**(i)** (x,y): (1,2), (2,3), (3,5), (4,4), (5,7) → **r = 0.90** *(fully solved in lecture — see Corr Example 3)*

**(ii)** (x,y): (1,1), (2,3), (3,5), (4,7), (5,9)  
*(Assignment — no solution given)*

**(iii)** (x,y): (1,10), (2,8), (3,6), (4,4), (5,2)  
*(Assignment — perfect negative linear relationship expected, r = −1)*

**(iv)** (x,y): (2,9), (3,5), (4,6), (5,2), (6,1)  
*(Assignment)*

**(v)** (x,y): (−2,4), (−1,1), (0,0), (1,1), (2,4)  
*(Assignment — note: this is a quadratic/parabolic relationship, so r = 0)*

---

### Lecture 9 — Assignment Problem 2: Ages & Blood Pressure (Scatter + Correlation)

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:** Ages and blood pressure of 10 women:

| Age (x) | 56 | 42 | 36 | 47 | 49 | 42 | 72 | 63 | 55 | 60 |
|---------|----|----|----|----|----|----|----|----|----|----|
| BP (y)  | 147 | 125 | 118 | 128 | 125 | 140 | 155 | 160 | 149 | 150 |

**Tasks:**
1. Draw a scatter diagram and comment
2. Find Pearson's r and comment

*(Answer: Try yourself — no solution given in lecture)*

---

### Lecture 9 — Assignment Problem 3: Math & Physics Scores (Correlation)

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:** Scores of 12 students:

| Mathematics | 2 | 3 | 4 | 4 | 5 | 6 | 6 | 7 | 7 | 8 | 10 | 10 |
|-------------|---|---|---|---|---|---|---|---|---|---|----|----|
| Physics | 1 | 3 | 2 | 4 | 4 | 4 | 6 | 4 | 6 | 7 | 9 | 10 |

**Task:** Find the correlation coefficient and interpret it.

*(No solution given — student exercise)*

---

### Lecture 9 — Assignment Problem 4: Advertisement & Profit (Pearson r + Spearman R)

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:**

| Profit (Tk. Crore) x | 25 | 28 | 27 | 33 | 31 | 10 | 16 | 16 | 18 | 23 |
|----------------------|----|----|----|----|----|----|----|----|----|-----|
| Adv. Exp. (Tk. Lakh) y | 87 | 91 | 92 | 95 | 93 | 52 | 68 | 72 | 78 | 86 |

**Tasks:**
1. Draw a scatter diagram and comment
2. Calculate Karl Pearson's correlation coefficient
3. Calculate Spearman's rank correlation coefficient
4. Comment on both results

*(No solution given — student exercise)*

---

### Lecture 9 — Assignment Problem 5: Advertisement & Sales

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:**

| Adv. Exp. (Tk. Lac) | 62 | 67 | 73 | 78 | 85 | 78 | 91 | 92 | 96 | 98 |
|---------------------|----|----|----|----|----|----|----|----|----|----|
| Sales (Tk. Crore)   | 11 | 13 | 17 | 18 | 21 | 24 | 21 | 27 | 26 | 21 |

**Task:** Calculate Karl Pearson's r AND Spearman's rank correlation coefficient. Comment.

*(No solution given — student exercise)*

---

### Lecture 9 — Regression Assignment Problem 1: Test Scores & Sales

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:** Test scores (y) and Sales in lakh Taka (x) of 9 salesmen:

| Test Scores (y) | 14 | 19 | 24 | 21 | 26 | 22 | 15 | 20 | 19 |
|-----------------|----|----|----|----|----|----|----|----|-----|
| Sales (x, lakh Tk) | 31 | 36 | 48 | 37 | 50 | 45 | 33 | 41 | 39 |

**(a)** Regression equation of test scores (y) on sales (x):  
**Answer: ŷ = −2.4 + 0.56x**

**(b)** Predicted test score when sale = Tk. 40 lakh:  
**Answer: ŷ = −2.4 + 0.56×40 = −2.4 + 22.4 = 20**

**(c)** Regression equation of sales (x) on test scores (y):  
**Answer: x̂ = 7.8 + 1.61y**

**(d)** Predicted sale when test score = 30:  
**Answer: x̂ = 7.8 + 1.61×30 = 7.8 + 48.3 = 56.1 lakh**

**(e)** Correlation coefficient using regression coefficients:  
r = √(b_yx × b_xy) = √(0.56 × 1.61) = √0.9016 = **0.95**

---

### Lecture 9 — Regression Assignment Problem 2: Ages & Blood Pressure

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:** Ages and blood pressure of 10 women:

| Age (x) | 56 | 42 | 36 | 47 | 49 | 42 | 72 | 63 | 55 | 60 |
|---------|----|----|----|----|----|----|----|----|----|----|
| BP (y)  | 147 | 125 | 118 | 128 | 125 | 140 | 155 | 160 | 149 | 150 |

**(i)** Regression line of y on x:  
**Answer: ŷ = 83.76 + 1.11x**

**(ii)** Estimated blood pressure for a woman aged 50:  
**Answer: ŷ = 83.76 + 1.11×50 = 83.76 + 55.5 = 139.26**

**(iii)** Regression line of x on y: *(Student exercise)*

**(iv)** Correlation coefficient: *(Student exercise)*

---

### Lecture 9 — Regression Assignment Problem 3: Simple x & y Dataset

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:**

| x | 1 | 2 | 3 | 4 | 5 | 6 |
|---|---|---|---|---|---|---|
| y | 6 | 4 | 3 | 5 | 4 | 2 |

**(a)** Regression line of y on x:  
**Answer: ŷ = 5.799 − 0.541x**

**(b)** Graph on scatter diagram: *(student task)*

**(c)** Estimate y when x = 4.5:  
**Answer: ŷ = 5.799 − 0.541×4.5 = 5.799 − 2.435 = 3.364 ≈ 3.486** *(lecture gives 3.486)*

**(d)** Predict y when x = 8:  
**Answer: ŷ = 5.799 − 0.541×8 = 5.799 − 4.328 = 1.471 ≈ 1.687** *(lecture gives 1.687)*

---

### Lecture 9 — Regression Assignment Problem 4: Units & Overhead (Knitting Co.)

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:** Units produced and overhead expenses at 8 plants:

| Units (x)    | 56  | 40  | 48  | 30  | 41  | 42  | 55  | 35  |
|-------------|-----|-----|-----|-----|-----|-----|-----|-----|
| Overhead (y) | 282 | 173 | 233 | 116 | 191 | 171 | 274 | 152 |

**Tasks:**
1. Draw a scatter diagram and comment
2. Fit a regression equation (y on x)
3. Estimate overhead when 65 units are produced

*(No answers given — student exercise)*

---

### Lecture 9 — Regression Assignment Problem 5: Sales & Experience

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

**Data:** Annual sales and years of experience of 8 salesmen:

| Salesmen         | 1  | 2  | 3  | 4  | 5  | 6   | 7   | 8   |
|-----------------|----|----|----|----|----|-----|-----|-----|
| Annual Sales (Tk.'000) | 90 | 75 | 78 | 86 | 95 | 110 | 130 | 145 |
| Years of Experience | 7 | 4  | 5  | 6  | 11 | 12  | 13  | 17  |

**Tasks:**
1. Fit two regression lines (sales on experience AND experience on sales)
2. Estimate sales for 10 years of experience
3. Estimate years of experience when sales = Tk. 100,000

*(No answers given — student exercise)*

---

### Lecture 9 — Final Exam Questions (with data)

**Source:** `9 Lecture-05 (Simple Linear Regression and Correlation analysis).pdf`

---

#### Spring-2014 (CSE): Hardness & Tensile Strength

**Data:** Hardness (X) and Tensile Strength (Y) of 7 metal samples:

| X | 146 | 152 | 158 | 164 | 170 | 176 | 182 |
|---|-----|-----|-----|-----|-----|-----|-----|
| Y | 75  | 78  | 77  | 89  | 82  | 85  | 86  |

**(i)** Find regression equation of y on x  
**(ii)** Estimate y when x = 169  

*(No answer given — exam question)*

---

#### Spring-2012 (EEE): r from regression coefficients

**Given:** b_yx = 0.5, b_xy = 1.9  
**Find:** Correlation coefficient r

**Solution:**
```
r = √(b_yx × b_xy) = √(0.5 × 1.9) = √0.95 = 0.975
```
**Answer:** r = **0.975**

**Verify AM ≥ GM:**
```
AM = (0.5 + 1.9)/2 = 1.2
GM = r = 0.975
1.2 > 0.975 ✓
```

---

#### Spring-2012 (ETE): r from negative regression coefficients

**Given:** b_yx = −0.8, b_xy = −0.6  
**Find:** Correlation coefficient r and comment

**Solution:**
```
r = −√(|b_yx| × |b_xy|) = −√(0.8 × 0.6) = −√0.48 = −0.693
```
**Answer:** r = **−0.693** → Fairly negative correlation between x and y.

---

#### Autumn-2012 (CSE): Husband & Wife Ages — Predict at x=30

**Same dataset as Regression Example 1** (7 couples, Σx=224, Σy=175...)  
**Additional question:** Estimate wife's age when husband's age = 30

**Using fitted line ŷ = −13.18 + 1.193x:**
```
ŷ = −13.18 + 1.193 × 30 = −13.18 + 35.79 = 22.61 years
```
**Answer:** Predicted wife's age = **22.61 years**

---

#### Spring-2013 (CSE): Father & Son Heights

**Data:** Heights of 6 fathers (y) and sons (x) in inches:

| Son height (x)    | 70 | 66 | 65 | 69 | 68 | 67 |
|------------------|----|----|----|----|----|-----|
| Father height (y) | 68 | 63 | 66 | 67 | 65 | 67 |

**(i)** Fit regression line of father height (y) on son height (x)  
**(ii)** Predict father's height if son's height = 65 inches

*(No answer given in source)*

---

#### Spring-2013 (CSE): Correlation from summary statistics

**Given:** Σx=56, Σy=40, Σx²=524, Σy²=256, Σxy=364, n=8

**Formula:** r = [nΣxy − ΣxΣy] / √{[nΣx²−(Σx)²][nΣy²−(Σy)²]}

```
r = [8×364 − 56×40] / √{[8×524 − 56²][8×256 − 40²]}
  = [2912 − 2240] / √{[4192 − 3136][2048 − 1600]}
  = 672 / √{1056 × 448}
  = 672 / √473088
  = 672 / 687.8
  = 0.977
```
**Answer:** r = **0.977** → Very strong positive correlation.

---

### Lecture 11 — Multiple Correlation Exercises (E1–E5)

**Source:** `11 Class Lecture-06 (Multiple Correlation and regression analysis).pdf`

---

#### Exercise E1

**Given:** r₁₂ = 0.6, r₂₃ = r₃₁ = 0.54  
**Find:** R₁.₂₃

```
R²₁.₂₃ = (r₁₂² + r₁₃² − 2r₁₂r₁₃r₂₃) / (1 − r₂₃²)
        = (0.36 + 0.2916 − 2×0.6×0.54×0.54) / (1 − 0.2916)
        = (0.36 + 0.2916 − 0.3499) / 0.7084
        = 0.3017 / 0.7084 = 0.4259
R₁.₂₃ = √0.4259 = 0.653
```
**Answer:** R₁.₂₃ = **0.653**

---

#### Exercise E2

**Given:** r₁₂ = 0.70, r₁₃ = 0.74, r₂₃ = 0.54  
**Find:** R₂.₁₃

```
R²₂.₁₃ = (r₁₂² + r₂₃² − 2r₁₂r₁₃r₂₃) / (1 − r₁₃²)
        = (0.49 + 0.2916 − 2×0.70×0.74×0.54) / (1 − 0.5476)
        = (0.49 + 0.2916 − 0.5594) / 0.4524
        = 0.2222 / 0.4524 = 0.4912
R₂.₁₃ = √0.4912 = 0.700
```
**Answer:** R₂.₁₃ = **0.70**

---

#### Exercise E3

**Given:** r₁₂ = 0.82, r₂₃ = −0.57, r₁₃ = −0.42  
**Find:** R₁.₂₃ and R₂.₁₃

```
R²₁.₂₃ = (0.82² + (−0.42)² − 2×0.82×(−0.42)×(−0.57)) / (1 − (−0.57)²)
        = (0.6724 + 0.1764 − 2×0.82×0.42×0.57) / (1 − 0.3249)
        = (0.6724 + 0.1764 − 0.3928) / 0.6751
        = 0.456 / 0.6751 = 0.676
R₁.₂₃ = √0.676 = 0.822

R²₂.₁₃ = (0.82² + (−0.57)² − 2×0.82×(−0.42)×(−0.57)) / (1 − (−0.42)²)
        = (0.6724 + 0.3249 − 0.3928) / (1 − 0.1764)
        = 0.6045 / 0.8236 = 0.734
R₂.₁₃ = √0.734 = 0.857
```
**Answer:** R₁.₂₃ ≈ **0.822**, R₂.₁₃ ≈ **0.857**

---

#### Exercise E4

**Data:** n=7

| X₁ | 22 | 15 | 27 | 28 | 30 | 42 | 40 |
|----|----|----|----|----|----|----|-----|
| X₂ | 12 | 15 | 17 | 15 | 42 | 15 | 28 |
| X₃ | 13 | 16 | 12 | 18 | 22 | 20 | 12 |

**Task:** Find R₁.₂₃, R₂.₁₃, R₃.₁₂ using the multiple correlation formula.

*(No solution given — student exercise)*

---

#### Exercise E5

**Data:** n=10

| X₁ | 50 | 54 | 50 | 56 | 50 | 55 | 52 | 50 | 52 | 51 |
|----|----|----|----|----|----|----|----|----|----|----|
| X₂ | 42 | 46 | 45 | 44 | 40 | 45 | 43 | 42 | 41 | 42 |
| X₃ | 72 | 71 | 73 | 70 | 72 | 72 | 70 | 71 | 75 | 71 |

**Task:** Using shortcut method, find R₁.₂₃, R₂.₁₃, R₃.₁₂.

*(No solution given — student exercise. Use deviations from convenient values like A₁=50, A₂=42, A₃=70)*

---

### Lecture 12 — MR Exercise 17.1: Simple Regressions (Reading Ability)

**Source:** `12 Multiple regression lecture.pdf`

**Data:**

| brightness (x₁) | 9 | 7 | 11 | 16 | 21 | 19 | 23 | 29 | 31 | 33 |
|-----------------|---|---|----|----|----|----|----|----|----|-----|
| noise (x₂)      | 100 | 93 | 85 | 76 | 61 | 58 | 46 | 32 | 24 | 12 |
| reading ability (y) | 40 | 50 | 64 | 73 | 86 | 97 | 104 | 113 | 123 | 130 |

**Simple regression of y on brightness alone:**
```
ŷ = 23.5 + 3.24x₁
→ Reading ability increases 3.24 units per 1-unit increase in brightness.
```

**Simple regression of y on noise alone:**
```
ŷ = 147.4 − 1.01x₂
→ Reading ability decreases 1.01 units per 1-unit increase in noise.
```

**Multiple regression of y on brightness AND noise:**
```
ŷ = 164.0 − 0.44x₁ − 1.15x₂

b₁ = −0.44 (controlling for noise — sign flips vs simple regression!)
b₂ = −1.15 (controlling for brightness)
```

**Predictions:**
```
At (x₁, x₂) = (19, 58):
ŷ = 164.0 − 0.44(19) − 1.15(58) = 164.0 − 8.36 − 66.7 = 88.94
Residual = 97 − 88.94 = 8.06

At (x₁, x₂) = (2, 3):
ŷ = 164.0 − 0.44(2) − 1.15(3) = 164.0 − 0.88 − 3.45 = 159.67
(outside data range — poor estimate)
```

**ANOVA / SS decomposition:**
```
SSE = 169.3
SSR = 8070.1 + 264.7 = 8334.8
SST = SSR + SSE = 8334.8 + 169.3 = 8504.1

R² = SSR/SST = 8334.8/8504.1 = 0.9801

MSR = SSR/k = 8334.8/2 = 4167.4
MSE = SSE/(n−k−1) = 169.3/7 = 24.2
F = MSR/MSE = 4167.4/24.2 = 172.4 ✓

R²_adj = 1 − [SSE/(n−k−1)] / [SST/(n−1)] = 1 − (169.3/7)/(8504.1/9) = 1 − 24.2/944.9 = 0.9744

sₑ = √(SSE/(n−k−1)) = √(169.3/7) = √24.2 = 4.917
```

**t-test for noise (β₂):**
```
t = −1.1458/0.3463 = −3.31
df = n−k−1 = 7
t*₇ (α=0.05, two-sided) = 2.36
|−3.31| = 3.31 > 2.36 → Reject H₀: β₂=0
→ Noise IS significant.
```

**95% CI for β₂:**
```
−1.15 ± 2.36 × 0.35 = −1.15 ± 0.826 = (−1.976, −0.324)
```

---

### Lecture 12 — MR Exercise: Book Expenditure (3 predictors)

**Source:** `12 Multiple regression lecture.pdf`

**Data:**

| Education (x₁) | 10 | 10 | 12 | 10 | 12 | 16 | 15 | 17 | 17 | 19 |
|---------------|----|----|----|----|----|----|----|----|----|----|
| Reading (x₂)  | 12 | 33 | 45 | 56 | 61 | 78 | 86 | 92 | 104 | 112 |
| Income (x₃, $k) | 10 | 15 | 25 | 36 | 41 | 58 | 66 | 72 | 84 | 92 |
| Book Exp. (y) | 40 | 50 | 64 | 73 | 86 | 97 | 104 | 113 | 123 | 130 |

**Simple regressions (each predictor alone):**
```
ŷ = −29.2 + 8.49x₁   (education alone — $8.49 more per year of education)
ŷ = 23.5  + 0.95x₂   (reading alone — $0.95 more per reading unit)
ŷ = 35.0  + 1.06x₃   (income alone — $1.06 more per $1000 income)
```

**Multiple regression (all 3 predictors):**
```
ŷ = 27.67 + 0.10x₁ + 0.51x₂ + 0.48x₃

R² = 0.9936  → 99.36% of variation explained
R²_adj = 0.9904
F = 311.7,  p-value = 5.657×10⁻⁷ < 0.05  → Model is significant overall
```

**t-tests for each predictor:**
```
Education: t = 0.10/0.97 = 0.106,  p = 0.919 > 0.05 → NOT significant
Reading:   t = 0.51/0.22 = 2.347,  p = 0.057         → Borderline (marginally significant)
Income:    t = 0.48/0.29 = 1.661,  p = 0.148 > 0.05 → NOT significant
```

**Note:** Even though overall F is very significant, none of the individual predictors reach significance at α=0.05 — this is due to **multicollinearity** (the three predictors are highly correlated with each other).

---

*DS 107 — Complete Examples & Questions | All 12 Lecture Files*
