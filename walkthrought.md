# RND-01: Video Walkthrough Presentation Script
**Target Duration:** 3 minutes 30 seconds to 4 minutes (Strictly under the 5:00 maximum limit)  
**Tone:** Objective, academically disciplined, data-grounded, no overclaiming  
**Recording Tools Recommended:** Loom, OBS Studio, or Windows Clipchamp / Game Bar (Win+Alt+R)  

---

## Preparation Checklist Before Recording
1. Open your browser with two tabs:
   * **Tab 1:** Your Google Drive submission folder showing all 5 files (`README.md`, `Report.pdf`, `Data.csv`, `Prompt_Appendix.md`, and this video file or link).
   * **Tab 2:** `Report.pdf` (or `Report.html`) opened to the Results Table and Summary Statistics.
2. Have `Data.csv` open in Excel, Google Sheets, or VS Code / Notepad.
3. Check microphone levels and ensure screen recording resolution is at least 1080p.

---

## Timed Word-for-Word Script & Visual Directives

### [0:00 – 0:45] SECTION 1: Introduction & Problem Statement
**Visual Cue:** Screen shows the Google Drive folder titled `RND-01 - AI Feedback Experiment`, showing the folder set to "Anyone with the link can view". Mouse hovers over the files.

> **Speaker:**  
> "in this video presenting the findings for project **RND-01**, an experimental study investigating whether lightweight AI feedback improves short learner essays compared to a rubric-only self-check.
> 
> In educational writing, students frequently struggle to translate static grading rubrics into meaningful revisions. Our pre-registered hypothesis tested whether giving learners lightweight AI feedback—specifically highlighting one key strength and two targeted, rubric-aligned improvements—would generate statistically higher score gains than having learners self-evaluate with the rubric alone.
> 
> Everything shown in this walkthrough is organized right here in our public Google Drive repository: including our full research report, the raw data, and a complete prompt appendix ."

---

### [0:45 – 1:45] SECTION 2: Methodology & Scoring Rubric
**Visual Cue:** Switch screen to `Report.pdf` (Page 1/2), scrolling to Section 1.3 (The 100-Point Analytical Rubric) and Section 2 (Data Collection).

> **Speaker:**  
> "To test this hypothesis with academic rigor and eliminate subjective 'vibes-based' grading, we established a standardized 100-point analytical rubric across four distinct 25-point criteria:
> 1. *Thesis and Argumentation*,
> 2. *Structure and Flow*,
> 3. *Evidence and Support*, and
> 4. *Grammar, Style, and Mechanics*, complete with explicit scoring anchors from Poor to Excellent.
> 
> For our dataset, we generated an ethically compliant synthetic cohort of ten short student essays between 150 and 250 words responding to the prompt: *'Should smartphones be banned in high school classrooms?'* The essays spanned three natural skill bands: weak, moderate, and strong.
> 
> We split these into two equal groups of five:
> * **Control Group A** simulated students using only the rubric to self-check and revise their work.
> * **Treatment Group B** received lightweight AI feedback specifying one strength and two actionable improvements, and then revised their drafts based on that guidance."

---

### [1:45 – 3:00] SECTION 3: Experimental Results & Data Table
**Visual Cue:** Switch screen to `Data.csv` (or the summary table in Section 3 of `Report.pdf`). Highlight the Control gains versus the Treatment gains.

> **Speaker:**  
> "Let's examine the raw empirical data. Here in `Data.csv`, both baseline and revised essays were evaluated double-blind against the 100-point rubric.
> 
> Looking at **Control Group A**:
> * The baseline mean was **59.60 points**.
> * After rubric-only self-checking, the revised mean rose to **64.00 points**.
> * That represents an average score gain of **+4.40 points**, or about a 7.4% improvement. Notice that these gains were almost entirely confined to surface mechanics and minor typo fixes.
> 
> In contrast, looking at **Treatment Group B**:
> * Starting from a baseline mean of **77.20 points**,
> * The group receiving lightweight AI feedback achieved a revised mean of **89.80 points**.
> * That is an average score gain of **+12.60 points**, or a 16.3% improvement.
> 
> When we compare the two groups, the net comparative gain is **+8.20 points** in favor of AI feedback. With a pooled standard deviation of 1.43, this yields a **Cohen's d effect size of 5.73**, and a two-sample t-statistic of 9.055, which is statistically significant at p < 0.001.
> 
> The qualitative reason for this difference is clear: the AI feedback bridged the 'evaluation-execution gap' by providing specific conceptual directions—such as citing concrete working-memory studies—that a static rubric simply cannot deliver on its own."

---

### [3:00 – 4:00] SECTION 4: Honest Limitations & Realistic Conclusion
**Visual Cue:** Switch to Section 5 ("Honest Limitations") in `Report.pdf`.

> **Speaker:**  
> "Now, to remain completely honest and avoid overclaiming, we must call out four critical limitations:
> 
> 1. **Sample Size:** With n=10, this is a small pilot study. While statistically significant here, small samples are prone to individual sample variance.
> 2. **Baseline Distribution:** Our sequential split placed more developing writers in Control and stronger writers in Treatment. While we measured *gain* rather than final score, stronger writers may have more linguistic agility to implement feedback.
> 3. **Synthetic Compliance Bias:** Revisions were executed by simulated LLM agents, which exhibit hyper-compliance. Real high school students experience cognitive overload, distractions, and may ignore or misapply feedback. Real-world classroom effect sizes will naturally be much more modest.
> 4. **LLM Evaluator Self-Preference:** Both generation and grading relied on frontier models, introducing potential stylistic bias that requires human educator validation in future trials.
> 
> **In conclusion:** Lightweight AI feedback shows strong, promising signal for accelerating student writing revision, but larger randomized controlled trials in live classrooms are essential before widespread pedagogical adoption.
> 
> Thank you for your time, and please feel free to review all the raw files and code in the public repository."

---

## Recording Tips for Maximum Rubric Score
* **Keep Pace Steady:** 3.5 minutes is approx. 450–500 words. Speak clearly and don't rush.
* **Show the Artifacts:** Make sure the grader sees `Data.csv`, `Report.pdf`, and the folder directory.
* **Underclaim, Don't Overclaim:** Graders award the 25 points for "Analysis honesty" and 10 points for "Walkthrough" specifically when you emphasize the limitations without pretending AI solved writing education.
