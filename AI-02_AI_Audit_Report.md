# AI-02 AI Audit Report

**CS423 / CSC15003 — Software Testing (AI-augmented, 2026)**  
**Assignment:** HW01-AI — QA/QC Jobs, 20 Defects, Test a Physical Product  
**Mandatory appendix for AI-assisted homework**

## 1. Student Information

| Field | Value |
|---|---|
| Student name (printed) | [Complete] |
| Student ID | [Complete] |
| Class / Cohort | [Complete] |
| Assignment ID | HW01-AI |
| Assignment date | [Complete] |
| AI tool(s) used | [List every tool used] |
| AI used for this assignment? | [ ] Yes  [ ] No |

## 2. Instructions

- Add one entry for each AI-generated artifact (for example, test cases, scripts, checklists, or report content).
- Record the full prompt verbatim, tool name, and actual timestamp.
- Include the full AI output verbatim, or a labeled screenshot in the report. Do not summarize or paraphrase the output in place of it.
- Mark the verdict **VALID**, **INVALID**, or **INCOMPLETE**.
- Support the reasoning with a course slide, ISTQB section, or relevant technical reference.
- Show the corrected student version and highlight what changed.
- Remove any sample material and complete all entries before submission.

## 3. Audit Entries — one per AI-generated artifact

### Artifact 1 — QA/QC Role & ISTQB Process Mindmap

**(1) Prompt + tool**  
Tool: Antigravity (Gemini 3.8 Flash)  
Timestamp: 12:07 25/09/2026  
Full prompt:

> Generate a comprehensive mindmap connecting modern QA/QC roles (QA Lead, Manual Tester, Automation Engineer/SDET, Performance Tester) to the fundamental ISTQB software testing process activities.

**(2) AI output**  
```text
Software Quality Ecosystem
├── QA (Quality Assurance - Finding bugs in software)
│   ├── Manual Tester: Executes test cases after code is deployed
│   └── QA Automation Engineer: Writes Selenium scripts to replace manual testers
└── Testing Lifecycle (Process)
    ├── 1. Test Planning (Write test plan at project kickoff)
    ├── 2. Test Design & Analysis (Combined: write test cases and prep data)
    ├── 3. Test Execution (Run test cases, log defects in Jira)
    └── 4. Test Closure (Sign off release)
```

**(3) Verdict**  
INVALID (Contains fundamental conceptual conflations and process omissions per ISTQB Foundation Level standards).

**(4) Reasoning**  
1. *Conflation of QA and QC:* Citing **ISTQB FL v4.0 Section 1.2.2 ("Quality Assurance and Testing")**, QA is strictly process-oriented (preventing defects via process governance and standards), while Testing is part of QC, which is product-oriented (detecting defects). The AI incorrectly defined QA as "finding bugs".
2. *Omission of Continuous Monitoring & Merging Analysis/Design:* Per **ISTQB FL v4.0 Section 1.4.2 ("Test Activities and Tasks")**, the ISTQB test process comprises 7 distinct activities. The AI omitted *Test Monitoring and Control* (which runs continuously throughout the lifecycle) and merged *Test Analysis* ("what to test") with *Test Design* ("how to test").
3. *Flawed Role Lifecycle Positioning:* Per **ISTQB FL v4.0 Section 3.1 ("Static Testing Basics")**, testers do not merely execute tests post-deployment; they actively participate in early static reviews of requirements (Shift-Left principle) during the analysis activity.

**(5) Student fix**  
The student redesigned the conceptual architecture into the verified diagram `QAQC_Role_Mindmap.png`:
- Formally separated **Quality Assurance (Process Governance, Audits, DoD, QA Manager/Lead)** from **Quality Control & Testing**.
- Introduced **Static Testing** early in the process lifecycle.
- Fully mapped the **7 ISTQB Test Activities**: (1) Test Planning, (2) Test Monitoring & Control, (3) Test Analysis, (4) Test Design, (5) Test Implementation, (6) Test Execution, (7) Test Completion, mapping appropriate roles (Test Analyst, Technical Test Analyst, SDET, QA Lead) to each activity.

### Artifact 2 — [Artifact name]

**(1) Prompt + tool**  
Tool: [Name]  
Timestamp: [HH:MM dd/mm/yyyy]  
Full prompt: [Paste the exact prompt]

**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 3 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 4 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 5 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 6 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 7 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 8 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 9 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

### Artifact 10 — [Artifact name]

**(1) Prompt + tool:** [Tool, actual timestamp, and full prompt]  
**(2) AI output:** [Full verbatim output or labeled screenshot]  
**(3) Verdict:** [VALID / INVALID / INCOMPLETE]  
**(4) Reasoning:** [2–5 sentences with course/ISTQB/technical citation]  
**(5) Student fix:** [Corrected version; highlight changes]

> Add further entries if you used AI to generate more than 10 artifacts.

## 4. Summary of AI Accuracy

| Metric | Count | Percentage |
|---|---:|---:|
| Total AI-generated artifacts audited | [ ] | 100% |
| VALID — correct and accepted as-is | [ ] | [ ]% |
| INVALID — wrong and rejected | [ ] | [ ]% |
| INCOMPLETE — acceptable after edits | [ ] | [ ]% |

**Calculation basis / denominator:** [Explain which artifacts are counted. Percentages should total 100%, allowing rounding.]

## 5. Conclusion — When should AI be used or not?

[Write 80–150 words describing observed patterns, where AI helped, where it failed, and your recommendation for using AI in this kind of work.]

## 6. Mandatory Disclosure

> “[Test cases / script / dataset / report] was initially generated by [AI tool name]; I reviewed and modified [section X], added [edge cases Y, Z]; [section W] was written entirely by me. The detailed AI Audit Report is attached as Appendix A. I confirm I did not use AI to generate any artifact listed in the prohibited category.”

[Replace the bracketed text truthfully and ensure it matches your actual AI use and the assignment's required disclosure placement.]

**Student name:** [Complete]  
**Student ID:** [Complete]  
**Class / Cohort:** [Complete]  
**Course:** CS423 / CSC15003 — Software Testing  
**Instructor:** [Complete]  
**Date:** [Complete]  
**Signature:** [Sign]

## References

- ISTQB Foundation Level Syllabus (latest version).
- Hardman, P. (2025). *A Post-AI Learning Taxonomy*.
- Fuster Rabella, M. (2025). OECD Education Working Paper No. 338.
- Perkins, M., Roe, J., & Furze, L. (2025). AI Assessment Scale.
- Anthropic (2025). Building reliable AI test agents — engineering blog.
- DeepEval and Promptfoo documentation — testing frameworks for LLM systems.
