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
Tool: Antigravity (Gemini 3.8 Flash Image Generator)  
Timestamp: 12:07 25/09/2026  
Full prompt:

> can you generate the image instead of mermaid? (Requesting an infographic mindmap visual covering QA/QC roles and the 7 ISTQB testing process activities)

**(2) AI output**  
The AI generated the visual infographic image asset `QAQC_Role_Mindmap.png` (embedded in Main Report Section 1.3), rendering a dual-branch structure: "Quality Assurance" on the left and "Quality Control & Testing" with 7 numbered procedural boxes on the right.

**(3) Verdict**  
INVALID (Contains 3 major structural, conceptual, and role-mapping defects when evaluated against the official ISTQB CTFL v4.0.1 syllabus).

**(4) Reasoning**  
1. *Misrepresentation of "Test Monitoring & Control":* The diagram models "2. Monitoring & Control" as an isolated, discrete step placed linearly between Planning and Analysis. According to **ISTQB CTFL v4.0.1 Section 1.4 and Section 5.3**, testing activities do not follow a rigid linear waterfall sequence; Monitoring & Control is an ongoing, continuous activity that spans all test phases to track progress and execute corrective actions.
2. *Misplaced and Detached "Static Testing" Flow:* The diagram features "Static Testing" as disconnected nodes floating in the middle, with an incorrect directional arrow linking into "Test Planning". According to **ISTQB CTFL v4.0.1 Chapter 3**, static testing consists of reviewing work products (such as requirements, designs, and user stories) and performing static code analysis without execution. It serves as an early defect prevention technique rather than an arbitrary sub-process feeding into Test Planning.
3. *Complete Omission of Testing/QC Roles:* While the QA branch explicitly defines organizational roles ("QA Lead, Process QA"), the QC & Testing branch merely lists procedural steps (1 to 7) without a single human job title. This violates the core HW01 requirement for a "QA/QC Role Mindmap" and contradicts **ISTQB CTFL v4.0.1 Section 1.4**, which establishes two fundamental role profiles: the **Test Management role** (responsible for planning, monitoring, and control) and the **Testing role** (e.g., Test Analyst, Test Engineer, Automation Tester, SDET).

**(5) Student fix**  
The student conducted an in-depth syllabus comparison and established the correct architectural corrections:
- Re-architected *Test Monitoring & Control* from a discrete sequential box into an ongoing, continuous feedback and governance loop that spans across all testing activities (from planning to completion).
- Re-anchored *Static Testing* as an early defect prevention practice (Shift-Left) applied across work products (requirements, user stories, designs, code reviews) rather than an isolated input to planning.
- Explicitly integrated human testing roles per ISTQB Section 1.4, mapping Test Management / QA Lead, Test Analyst, Technical Test Analyst, Automation Tester, and SDET to their corresponding static analysis and dynamic test execution stages.

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
