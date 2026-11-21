# Rubric Name: Graded Assignment-1 Evaluation Standard

**Course:** Analytics for E-Commerce  
**Weightage:** 20% | **Total Marks:** 20  
**Evaluation Model:** 5 Core Criteria × 4 Points Each = 20 Points Total  

---

## 1. Master Evaluation Rubric Table

| Criteria | Level 4<br>**(3.1 – 4.0 points)** | Level 3<br>**(2.1 – 3.0 points)** | Level 2<br>**(1.1 – 2.0 points)** | Level 1<br>**(0.0 – 1.0 points)** | Criterion Score |
| :--- | :--- | :--- | :--- | :--- | :---: |
| **1. Problem Understanding & Framing** | Fully grasps user lifecycle frameworks, telemetry design, funnel stages, and association parameters. Correctly frames business goals and intent metrics. | Good understanding of core analytics frameworks with minor non-critical gaps in contextual business interpretation. | Partial understanding; confuses funnel drop-offs with lifecycle stages or mistakes telemetry scopes. | Minimal or incorrect understanding of underlying e-commerce data and analytics concepts. | **__/ 4** |
| **2. Technical Calculations & Accuracy** | Calculates Support, Confidence, Lift, CRO rates, alert limits, CAC, and CLV with 100% mathematical accuracy. | Minor arithmetic or rounding errors, but overall formula setup, logic, and output structure are correct. | Significant calculation errors, incorrect formula applications, or wrong probability calculations. | Completely incorrect or missing quantitative calculations across multiple questions. | **__/ 4** |
| **3. Analytical Depth & Diagnostics** | Deeply isolates root causes (e.g., above-the-fold friction, systemic payment drop-offs, and channel performance contrasts). | Identifies main data insights but lacks depth in isolating external confounders or underlying channel quality. | Surface-level data summary without actionable diagnostic value or statistical rigor. | Summarizes raw numbers without drawing analytical or diagnostic conclusions. | **__/ 4** |
| **4. Practical Strategy & Recommendations** | Provides actionable, highly targeted strategy (ICE prioritization framework, clear budget reallocation recommendations). | Recommendations are sound but lack explicit operational metrics, ICE scoring, or strategic prioritization. | Vague or generic business recommendations that are disconnected from the calculated data findings. | Incomplete, missing, or impractical strategic recommendations. | **__/ 4** |
| **5. Structure & Documentation Quality** | Exceptionally well-organized submission with step-by-step mathematical working, valid JSON schemas, and clear formatting. | Organized submission with minor formatting issues or slight lack of clarity in step-by-step working. | Disorganized presentation making mathematical steps or JSON data schemas difficult to trace. | Poorly structured, unformatted, or incomplete submission. | **__/ 4** |
| **Total Score** | | | | | **__/ 20** |

---

## 2. Detailed Performance Level Descriptors & Criteria Breakdown

### Criterion 1: Problem Understanding & Framing (Weight: 4 Marks)
* **Scope:** Evaluates comprehension of e-commerce data architecture, telemetry hierarchy, funnel dynamics, and business objectives.
* **Level 4 (3.1 – 4.0 pts):** Demonstrates complete mastery of e-commerce data hierarchies (`User` $\to$ `Session` $\to$ `Event`), warehouse schemas (`Fact` vs. `Dimension`), conversion funnels, and customer lifecycle concepts. Articulates clear business intent behind tracking and metrics.
* **Level 3 (2.1 – 3.0 pts):** Demonstrates solid grasp of foundational concepts, but contains minor conceptual oversights in contextualizing business outcomes.
* **Level 2 (1.1 – 2.0 pts):** Shows confusion between distinct analytics paradigms (e.g., mixing up session-level telemetry with user-level dimensions, or conflating micro-funnel drop-offs with macroscopic lifecycle churn).
* **Level 1 (0.0 – 1.0 pts):** Fundamentally misinterprets e-commerce metrics, data pipelines, or tracking structures.

---

### Criterion 2: Technical Calculations & Accuracy (Weight: 4 Marks)
* **Scope:** Assesses quantitative rigor, formula application, and mathematical precision across all assignment questions.
* **Required Formula Checks:**
  1. **Market Basket Support:** $\text{Support}(A \cup B) = \frac{\text{Transactions with } A \text{ and } B}{\text{Total Transactions}}$
  2. **Market Basket Confidence:** $\text{Confidence}(A \to B) = \frac{\text{Support}(A \cup B)}{\text{Support}(A)}$
  3. **Lift Ratio:** $\text{Lift}(A \to B) = \frac{\text{Confidence}(A \to B)}{\text{Support}(B)}$
  4. **CRO Conversion Rates:**
     - Add-to-Cart (ATC) Rate $= \frac{\text{ATC Clicks}}{\text{PDP Visits}}$
     - Search/PDP-to-Purchase Rate $= \frac{\text{Completed Purchases}}{\text{PDP Visits}}$
  5. **Upper Alert Limit (UAL):** $\text{UAL} = \mu + 2\sigma$
  6. **Customer Acquisition Cost (CAC):** $\text{CAC} = \frac{\text{Total Acquisition Spend}}{\text{New Customers Acquired}}$
  7. **Customer Lifetime Value (Historic CLV):** $\text{CLV} = \text{AOV} \times \text{Purchase Frequency} \times \text{Customer Lifespan}$
  8. **CLV-to-CAC Ratio:** $\frac{\text{CLV}}{\text{CAC}}$
* **Level 4 (3.1 – 4.0 pts):** 100% mathematical accuracy across all steps, proper units, and exact percentage/decimal expressions without rounding errors.
* **Level 3 (2.1 – 3.0 pts):** Sound methodology and correct formula structures, but contains minor arithmetic or rounding slips.
* **Level 2 (1.1 – 2.0 pts):** Incorrect formulas applied (e.g., wrong denominator in conditional probability, flawed standard deviation multiplier, or incorrect CLV formulation).
* **Level 1 (0.0 – 1.0 pts):** Pervasive calculation failures or completely missing quantitative answers.

---

### Criterion 3: Analytical Depth & Diagnostics (Weight: 4 Marks)
* **Scope:** Assesses the ability to drill down into the data to isolate root causes rather than merely repeating numbers.
* **Key Diagnostic Expectations:**
  - **Question 3:** Diagnose the mobile UX bottleneck caused by 75% scroll-depth abandonment before the fold (unseen reviews and ingredient disclosures).
  - **Question 4:** Isolate statistical anomaly at Step 3 (Delivery Schedule drop-off) using process control limits ($\mu + 2\sigma$), distinguishing systemic technical/logistical friction from natural user churn.
  - **Question 5:** Contrast customer channel quality between Paid Social Ads (lower CAC, low CLV, lower order frequency) and Referral Program (higher CAC, massive CLV, high repeat intent).
* **Level 4 (3.1 – 4.0 pts):** Rigorous, multi-dimensional root-cause analysis isolating UX, technical, and behavioral factors with statistical confidence.
* **Level 3 (2.1 – 3.0 pts):** Identifies obvious high-level patterns but fails to isolate deeper confounding variables or underlying friction mechanisms.
* **Level 2 (1.1 – 2.0 pts):** Surface-level reporting of results without investigative diagnostics or causal deductions.
* **Level 1 (0.0 – 1.0 pts):** Restates the problem prompt or numbers without analytical insight.

---

### Criterion 4: Practical Strategy & Recommendations (Weight: 4 Marks)
* **Scope:** Evaluates strategic viability, structured decision frameworks, and concrete business execution plans.
* **Key Strategic Elements Required:**
  - **Digital Shelf Merchandising (Q2):** Cross-selling bundle strategy, recommendation widgets, or dynamic threshold discounts.
  - **ICE Framework Scoring (Q3):** Explicit quantitative evaluation of **Impact (1–5)**, **Confidence (1–5)**, and **Ease (1–5)** comparing the PDP mobile redesign vs. checkout button color test.
  - **Growth Budget Reallocation (Q5):** Actionable, math-backed budget reallocation between channels based on the $\ge 3:1$ CLV:CAC benchmark and net unit economics.
* **Level 4 (3.1 – 4.0 pts):** Highly actionable, prioritized recommendations supported by the ICE matrix and precise financial reallocation figures.
* **Level 3 (2.1 – 3.0 pts):** Sensible business suggestions that lack structured scoring (e.g., missing formal ICE score tables or exact budget percentage shifts).
* **Level 2 (1.1 – 2.0 pts):** Generic textbook advice detached from the empirical findings of the questions.
* **Level 1 (0.0 – 1.0 pts):** Infeasible, impractical, or completely absent recommendations.

---

### Criterion 5: Structure & Documentation Quality (Weight: 4 Marks)
* **Scope:** Evaluates academic presentation, schema validity, and clarity of working.
* **Formatting Requirements:**
  - Explicit step-by-step formula notation and substitutions.
  - Syntactically valid **JSON Schema** definition (valid draft meta-schema, property definitions, types, and required fields) for Question 1.
  - Clear markdown tables, bulleted takeaways, and visual hierarchy.
* **Level 4 (3.1 – 4.0 pts):** Flawless formatting, structured headings, readable math, and valid machine-parseable JSON schema.
* **Level 3 (2.1 – 3.0 pts):** Organized submission with minor formatting inconsistencies or omitted intermediate steps.
* **Level 2 (1.1 – 2.0 pts):** Disorganized or poorly formatted document where formulas or schemas are invalid/hard to trace.
* **Level 1 (0.0 – 1.0 pts):** Incomplete, unstructured, or unformatted submission.

---

## 3. Assignment Question to Rubric Mapping Matrix

| Question | Topic | Total Marks | Primary Rubric Criteria Tested |
| :---: | :--- | :---: | :--- |
| **Q1** | Telemetry Architecture & Event Data Models | 4 | **Criterion 1** (Hierarchy, scopes, schemas) & **Criterion 5** (JSON schema syntax) |
| **Q2** | Exploratory Data Analysis & Market Basket Affinity | 4 | **Criterion 2** (Support, Confidence, Lift math) & **Criterion 4** (Merchandising intervention) |
| **Q3** | Product Analytics & CRO Prioritization | 4 | **Criterion 2** (CRO rates), **Criterion 3** (Above-the-fold diagnostics), & **Criterion 4** (ICE framework) |
| **Q4** | Funnel Leakage & Statistical Diagnostics | 4 | **Criterion 2** (UAL calculation), **Criterion 3** (Systemic leak vs. natural churn diagnostics) |
| **Q5** | Customer Lifecycle, Cohorts & CLV Economics | 4 | **Criterion 2** (CAC, CLV, Net profit math), **Criterion 3** (Channel performance contrast), & **Criterion 4** (Budget reallocation) |
