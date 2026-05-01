# Individual Addendum Template
## QM 2023 Capstone Project — Milestone 4

---

**Individual Contribution Statement**

| Field | Response |
|-------|----------|
| **Name** | _________________________________ |
| **Team** | _________________________________ |
| **Date** | _________________________________ |

---

## 1. Personal Contribution to Capstone Milestones

*Provide specific, quantifiable contributions to each milestone. Include tasks, hours, and deliverables.*

### Milestone 1: Data Pipeline (Week 5)

**Tasks completed:**
- [ ] [Specific task 1, e.g., "Implemented FRED API integration for economic indicators"]
- [ ] [Specific task 2, e.g., "Handled missing value imputation for REIT returns"]
- [ ] [Specific task 3, e.g., "Verified merge logic and ensured no duplicate rows"]

**Hours spent:** _____ hours

**Key deliverable:** [e.g., "FRED data fetching function (Section 4 of `capstone_data_pipeline.py`)"]

---

### Milestone 2: EDA Dashboard (Week 10)

**Tasks completed:**
- [ ] [Specific task 1, e.g., "Created correlation heatmap and dual-axis plots"]
- [ ] [Specific task 2, e.g., "Conducted lagged effect analysis to determine optimal lag structure"]
- [ ] [Specific task 3, e.g., "Wrote economic interpretation captions for all visualizations"]

**Hours spent:** _____ hours

**Key deliverable:** [e.g., "Visualizations 1, 2, and 7 in `capstone_eda.ipynb` + captions"]

---

### Milestone 3: Econometric Models (Week 14)

**Tasks completed:**
- [ ] [Specific task 1, e.g., "Specified and estimated Fixed Effects model with clustered SEs"]
- [ ] [Specific task 2, e.g., "Ran heteroskedasticity and VIF diagnostics"]
- [ ] [Specific task 3, e.g., "Conducted robustness checks: alternative lags, COVID exclusion, sector subsamples"]

**Hours spent:** _____ hours

**Key deliverable:** [e.g., "M3 Fixed Effects regression code (Section 3) and diagnostics (Section 5)"]

---

### Milestone 4: Final Investment Memo (Week 14)

**Tasks completed:**
- [ ] [Specific task 1, e.g., "Drafted Executive Summary and Investment Recommendations sections"]
- [ ] [Specific task 2, e.g., "Compiled regression tables from M3 results"]
- [ ] [Specific task 3, e.g., "Edited full memo for clarity and professional tone"]

**Hours spent:** _____ hours

**Key deliverable:** [e.g., "Executive Summary, Conclusions & Recommendations sections (Sections 1 and 3 of final memo)"]

---

### Total Estimated Contribution

| Summary Item | Value |
|--------------|-------|
| Total hours across all milestones | _____ hours |
| Percentage of team workload | _____% *(must sum to 100% across all team members)* |
| Role(s) on team | [e.g., "Data Engineer (M1 lead), Visualization Specialist (M2 lead), Communication Lead (M4 lead)"] |

---

## 2. One Defended Methodological Decision

*Choose one methodological decision you made (or advocated for) during the capstone project. Explain your reasoning with evidence from the analysis or economic theory.*

**Decision:** [State the decision clearly]

> **Example:** "I recommended using a 2-month lag for the Federal Funds Rate in our Fixed Effects model."

**Reasoning:**

*Provide 2–4 sentences explaining WHY this decision was correct, grounding your argument in:*

- **Data evidence:** [e.g., "M2 exploratory analysis showed the strongest correlation at lag 2 (r = −0.38 vs. r = −0.20 at lag 1)."]
- **Economic reasoning:** [e.g., "REITs negotiate leases and refinance debt over 1–2 months, so immediate rate effects are muted."]
- **Robustness:** [e.g., "M3 robustness checks confirmed that lag 2 coefficient is most statistically significant (p = 0.012 vs. p = 0.08 for lag 1)."]

**Alternative considered (and why rejected):**

*[Optional but impressive: mention an alternative approach and why you chose your decision instead.]*

> **Example:** "We considered using the contemporaneous rate (lag 0) for simplicity, but this produced weaker statistical significance (p = 0.15) and was less consistent with REIT financing timelines."

---

## 3. One Key Limitation of Our Analysis

*Identify the most important limitation or caveat of your capstone analysis. Be honest and substantive — this is not the place for trivial concerns.*

**Limitation:** [State the limitation clearly]

> **Example:** "Our Fixed Effects model assumes that unobserved REIT characteristics (management quality, property mix) are time-invariant."

**Why this matters:**

*Explain the economic or statistical implication of this limitation in 2–4 sentences.*

> **Example:** However, during the COVID-19 pandemic, many REITs restructured their portfolios (e.g., exited retail properties, entered industrial warehouses). If these portfolio shifts correlate with both REIT returns and interest rate exposure, our Fixed Effects estimates may be biased. For instance, a REIT that shifted to industrial properties in 2020 would appear less rate-sensitive in our model, but this could be due to the portfolio change, not the rate environment.

**Potential mitigation:**

*Suggest how future work could address this limitation.*

> **Example:** A robustness check using two-way Fixed Effects with sector-time interactions could partially address this concern by allowing for time-varying sector effects. Alternatively, a dynamic panel model (e.g., Arellano-Bond GMM) could account for portfolio restructuring over time, but this requires a longer time series and is beyond the scope of this capstone.

---

## 4. AI Audit Notes *(If Applicable)*

*If you used AI tools for any specific tasks in your portion of the work, document them here. This section is optional if AI use was fully documented in the team AI Audit Appendix.*

**AI Tools Used** *(check all that apply):*
- [ ] ChatGPT
- [ ] GitHub Copilot
- [ ] Claude
- [ ] Other: _________________________________

### Specific AI Use Examples

**Example 1:**

| Field | Details |
|-------|---------|
| Task description | [What you were trying to accomplish] |
| Prompt | [What you asked the AI] |
| Output | [What the AI produced] |
| Verification | [How you tested it worked correctly] |
| Critique | [What the AI got wrong, how you corrected it] |

**Example 2:** *(Repeat for each significant AI interaction)*

| Field | Details |
|-------|---------|
| Task description | |
| Prompt | |
| Output | |
| Verification | |
| Critique | |

**Overall AI Use:**

> **Example:** I used AI for approximately 30% of my coding tasks (syntax help, debugging) but wrote all interpretations and economic reasoning independently. I verified all AI-generated code by running it on our dataset and cross-checking outputs against expected values.

[Your overall AI use statement here]

---

## 5. Self-Reflection

### What did I do particularly well on this capstone?

*1–2 sentences highlighting your strengths or proudest moments.*

> **Example:** I excelled at translating technical regression output into business language for the final memo. My Executive Summary clearly communicated complex findings to a non-technical audience without sacrificing accuracy.

[Your response here]

---

### What could I have improved?

*1–2 sentences acknowledging areas for growth.*

> **Example:** I could have started M3 econometric modeling earlier instead of waiting until the week before the deadline. This would have given me more time to explore alternative specifications and conduct deeper robustness checks.

[Your response here]

---

### What did I learn from this capstone project?

*2–3 sentences reflecting on skill development or conceptual insights.*

> **Example:** This capstone taught me that data cleaning is 80% of the work in real-world analysis. I also learned to defend methodological choices with evidence (not just intuition) and to communicate limitations honestly rather than hiding them. Most importantly, I developed confidence in my ability to execute an end-to-end data science workflow from raw data to professional deliverable.

[Your response here]

---

## 6. Attestation

By submitting this individual addendum, I affirm that:

- [ ] All contributions listed above are accurate and honest
- [ ] I have not exaggerated my role or minimized teammates' contributions
- [ ] I understand that this addendum may be used to adjust my individual grade relative to the team grade
- [ ] I take full responsibility for my work and any errors in the sections I authored

**Signature:** _________________________________ &nbsp;&nbsp;&nbsp;&nbsp; **Date:** _____________

---

## Submission Instructions

1. **Save as PDF:** `Individual_Addendum_[YourLastName].pdf`
   - Example: `Individual_Addendum_Johnson.pdf`

2. **Submit via GitHub Classroom** (in the M4 submission folder):
   ```bash
   git add Individual_Addendum_[YourLastName].pdf
   git commit -m "Add individual addendum - [Your Name]"
   git push origin main
   ```

3. **Verify submission:** Check GitHub repo; your PDF should appear alongside the team memo.

**Deadline:** Friday, Week 14 (May 1) by 11:59 PM *(same as M4 team memo)*

---

## Grading Criteria (10 points)

| Component | Points | Criteria |
|-----------|--------|----------|
| Specific Contribution | 3 | Tasks, hours, and deliverables are specific (not vague) |
| Defended Decision | 3 | Decision is clearly stated, reasoning is grounded in evidence |
| Key Limitation | 3 | Limitation is substantive and honestly discussed |
| Overall Quality | 1 | Professional writing, honest reflection |
| **Total** | **10** | *(part of M4 50-point grade)* |

---

## FAQs

**Q: What if I contributed equally to all milestones?**

A: That's fine. List specific tasks for each milestone and estimate equal hours. The key is specificity (not just "I helped with M2").

**Q: What if I contributed less than my teammates due to other commitments?**

A: Be honest. Instructors understand that life happens. Clearly document what you *did* contribute, and note in your reflection what you would do differently. Grades are adjusted based on actual contribution, not ideal contribution.
