# AI-02 AI Audit Report

**CS423 / CSC15003 — Software Testing (AI-augmented, 2026)**  
**Assignment:** HW01-AI — QA/QC Jobs, 20 Defects, Test a Physical Product  
**Mandatory appendix for AI-assisted homework**

## 1. Student Information

| Field | Value |
|---|---|
| Student name (printed) | Bùi Minh Quân |
| Student ID | 23120337 |
| Class / Cohort | Computer Science / IT (23CLC) |
| Assignment ID | HW01-AI |
| Assignment date | 26/09/2026 |
| AI tool(s) used | Antigravity (Gemini 3.8 Flash), Codex (GPT-6) |
| AI used for this assignment? | [x] Yes  [ ] No |

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

### Artifact 2 — AI Explanation of Software Defect (Air Canada Chatbot Case)

**(1) Prompt + tool**  
Tool: Antigravity (Gemini 3.8 Flash)  
Timestamp: 15:39 25/09/2026  
Full prompt:

> /browser Use browser MCP, find 20 publicized software defects for me, include the AI/LLM requirements. Then for each defect, provide 5 mandatory attributes follow the document, I'll verify all the defect by my self before write them down to the main document

**(2) AI output**  
When generating the analysis for Defect #1 (*Moffatt v. Air Canada*), the AI generated the following explanation regarding the legal outcome:

> *"In Moffatt v. Air Canada, the passenger filed a landmark class-action lawsuit in the Supreme Court of Canada after the airline's generative AI chatbot provided inaccurate bereavement discount rates. Air Canada argued that the chatbot was an autonomous entity, but the court ruled against the airline, forcing Air Canada to settle out of court for $50,000 in damages and establishing that AI chatbots cannot be governed by ordinary human consumer contract law."*

**(3) Verdict**  
INVALID (Contains severe factual hallucinations, legal mischaracterizations, and fabricated financial amounts).

**(4) Reasoning**  
Evaluation against primary tribunal records (*Moffatt v. Air Canada*, 2024 BCCRT 149) and verified reporting (CBC News, Wired) reveals three distinct hallucinations:
1. *Legal Venue & Nature of Case:* It was not a "landmark class-action lawsuit in the Supreme Court of Canada." It was an individual small-claims action adjudicated by the British Columbia Civil Resolution Tribunal (BC CRT)—an online administrative tribunal.
2. *Settlement & Financial Damages:* Air Canada did not "settle out of court for $50,000." Air Canada actively contested the claim. Member Christopher Rivers ruled in Moffatt's favor and ordered Air Canada to pay exactly **$812.02 CAD** (comprising $650.88 CAD in fare difference, $36.14 pre-judgment interest, and $125 CRT fees).
3. *Legal Holding on AI Liability:* The tribunal did not rule that "AI chatbots cannot be governed by ordinary consumer contract law." In fact, the tribunal ruled the exact opposite: Member Rivers firmly dismissed Air Canada's defense that the bot was a "separate legal entity responsible for its own actions," establishing that corporations bear full vicarious liability for misrepresentations made by their automated tools.

**(5) Student fix**  
The student rejected the AI-generated claims and rewrote Section 2.1, 2.2 (Defect #1), and Section 2.3 of `Main_Report.md` using verified primary legal facts:
- Stated the exact jurisdiction as the BC Civil Resolution Tribunal (2024 BCCRT 149).
- Documented the exact award amount of $812.02 CAD.
- Formulated the precise technical root cause (RAG pipeline lacking schema-bound verification against static tariffs) and correct legal takeaway (vicarious corporate liability for conversational AI agents).

### Artifact 3 — AI-Generated Test Cases for Xiaomi Mi Smart LED Desk Lamp

**(1) Prompt + tool**  
Tool: Antigravity (Gemini 3.8 Flash)  
Timestamp: 22:46 25/09/2026  
Full prompt:

> Okay let's start requirement 3, list the work I have to do (and generate test cases for the Xiaomi Mi Smart LED Desk Lamp)

**(2) AI output**  
The AI initially generated 15 standard, predominantly software- and app-centric test cases:
1. Turn on/off via app power button.
2. Adjust brightness slider in app from 0% to 100%.
3. Set scheduled on/off timer in app.
4. Voice assistant command integration ("Turn lamp to daylight").
5. Connect lamp to 2.4 GHz Wi-Fi router.
6. Connect lamp with invalid Wi-Fi password (verify error handling).
7. Reconnect after router power cycle.
8. Factory reset via app unpair button.
9. Single-click physical knob to turn on/off.
10. Rotate physical knob to adjust brightness.
11. Press and rotate physical knob to adjust color temperature.
12. Double-click physical knob to activate pomodoro timer.
13. App notification when firmware update is available.
14. Perform OTA firmware update via app.
15. Multi-device sync (verify two phones reflect same lamp state).

**(3) Verdict**  
INCOMPLETE (Lacks physical, electrical transient, thermodynamic, and optical biological safety edge cases).

**(4) Reasoning**  
Evaluation against **ISTQB CTFL v4.0.1 Section 4.2 (Black-Box Test Techniques — Equivalence Partitioning & Boundary Value Analysis)** and Bloom-AI Level **G9.3 (Analyze)** demonstrates that commercial LLMs suffer from an "App-Centric Software Bias":
- The AI treats the physical smart lamp as if it were a purely virtual software application or Web API.
- The AI completely omits real-world physical embodiment constraints: contact bounce on the DC barrel jack (<200ms power interruption), physical rotary encoder interrupt race conditions (simultaneous depress and high-speed spin past mechanical limits), thermodynamic heat dissipation causing hinge cantilever friction sagging over time, and optical PWM stroboscopic ripple under IEEE 1789-2015 standards.

**(5) Student fix**  
The student rejected 4 redundant app/cloud test cases and engineered **4 critical physical hardware edge cases** (documented as TC-12 through TC-15 in Section 3.3 of `Main_Report.md`):
- **TC-12 (Edge Case 1):** Rapid DC barrel plug contact chatter (<200ms power bounce) to test microcontroller Brownout Detection (BOD) and driver latch-up prevention.
- **TC-13 (Edge Case 2):** Rotary encoder boundary overflow and simultaneous depress race condition to validate quadrature decoding ISR clamping.
- **TC-14 (Edge Case 3):** Sustained 100% lumen thermal dissipation and hinge cantilever friction retention under continuous 60-minute heat load.
- **TC-15 (Edge Case 4):** Optical stroboscopic flicker and PWM ripple compliance using 240fps slow-motion capture per IEEE 1789-2015 ocular health guidelines.

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
