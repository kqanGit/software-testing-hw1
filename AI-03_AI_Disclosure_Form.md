# AI-03 AI Use Disclosure Form

**CS423 / CSC15003 — Software Testing (AI-augmented, 2026)**  
Attach this form to the assignment when AI was used in a permitted capacity.

## 1. Course and Student Information

| Field | Value |
|---|---|
| Course | CS423 / CSC15003 — Software Testing |
| Assignment ID | HW01-AI |
| Assignment title | HW01 — QA/QC Jobs, 20 Defects, Test a Physical Product |
| AI Use Category (1–5) | Category 4 — AI-Augmented Collaboration (Human-in-the-Loop) |
| Date | 26/09/2026 |
| Student name | Bùi Minh Quân |
| Student ID | 23120337 |

## 2. Disclosure Questions

### 2.1 AI tools used

* **Antigravity (Gemini 3.8 Flash / Imagen):** Used for initial job market search query ideation, drafting defect descriptions, generating the initial QA/QC mindmap, drafting standard happy-path test cases, and report skeleton structuring.
* **Codex (GPT-6):** Used for cross-checking technical defect root-cause descriptions and regex formatting of tables.

### 2.2 Assignment stages where AI was used

Mark every applicable stage:  
[x] Brainstorming  [x] Outlining  [x] Drafting  [ ] Feedback  [x] Revision  [ ] Coding  [x] Data analysis  [x] Visual design  [ ] Other: [Research & initial defect aggregation]

Details: AI was utilized as an assistive co-pilot to brainstorm initial search terms for QA job listings, draft initial defect candidate descriptions, generate an initial mindmap image, and propose a preliminary set of desk lamp test cases. All outputs were subjected to rigorous human auditing and manual verification.

### 2.3 Main prompts or tasks given to AI

Paste 2–3 of the most impactful prompts verbatim. Attach the complete prompt log as Appendix A.

1. **Mindmap Generation (Prompt #19 - 12:07 25/09/2026):**  
   `can you generate the image instead of mermaid?`  
   *(Requesting an infographic visual covering QA/QC roles and the 7 ISTQB testing process activities for Requirement 1)*
2. **20 Software Defects Gathering (Prompt #26 - 15:39 25/09/2026):**  
   `/browser Use browser MCP, find 20 publicized software defects for me, include the AI/LLM requirements. Then for each defect, provide 5 mandatory attributes follow the document, I'll verify all the defect by my self before write them down to the main document`  
   *(Prompting initial candidate aggregation for Requirement 2)*
3. **Physical Product Test Case Generation (Prompt #36 - 22:46 25/09/2026):**  
   `Okay let's start requirement 3, list the work I have to do`  
   *(Requesting baseline test cases and testing breakdown for the Xiaomi Desk Lamp for Requirement 3)*

### 2.4 Specific parts of the work AI contributed to

* **Requirement 1:** AI suggested initial job keywords and generated the initial `QAQC_Role_Mindmap.png`. The student independently searched, selected, verified all 10 job postings within the 60-day window, logged into portals under account "Quân Bùi" to capture 10 anti-cheat screenshots, wrote individual AI Impact Analyses, and performed an ISTQB CTFL v4.0.1 audit identifying 3 architectural errors in the AI mindmap.
* **Requirement 2:** AI aggregated preliminary descriptions for software defects. The student independently verified all 20 defects against primary sources, updated 6 entries with user-verified live URLs (e.g. Envive, StealthCloud, IT Jungle, TestMax, HIPAA Guide, Owler), and authored the audit debunking the Air Canada legal hallucination.
* **Requirement 3:** AI proposed standard app-centric test cases. The student rejected the app-bias, selected a real owned physical product (Xiaomi Mi Smart LED Desk Lamp `MJTD01YL`), captured anti-cheat photo with Student ID card (`23120337`), engineered 5 physical/electrical/spill edge cases (TC-08, TC-12–TC-15), executed 5 physical tests, and recorded 5 voice-narrated YouTube Unlisted demo videos.
* **Section 4 & 5:** The student authored the 233-word AI Critique and structured the AI Audit Report summary table.

### 2.5 How I reviewed, revised, or verified the AI output

* **Job Postings:** Directly visited job boards (ITviec, TopCV, LinkedIn), verified publication dates within 60 days of September 2026, confirmed salary disclosure, and captured authenticated logged-in screenshots.
* **Software Defects:** Evaluated defect claims against primary legal records (*Moffatt v. Air Canada*, 2024 BCCRT 149), CVE advisories, and technical post-mortems (CrowdStrike PIR, OpenAI incident log).
* **Mindmap Audit:** Cross-referenced every node and relationship in `QAQC_Role_Mindmap.png` against the official ISTQB CTFL v4.0.1 syllabus (Sections 1.4, 3.1, and 5.3), discovering that Monitoring & Control was wrongly drawn as a sequential step and QC roles were completely omitted.
* **Physical Hardware:** Physically operated the Xiaomi desk lamp on a workbench, executing knob rotations, hinge flexures, power disconnects, and simulated liquid spills to ensure test validity.

### 2.6 Citation, if required by course style guide

The supplied form specifies IEEE style. Add citations for the AI tool(s) used, following the instructor's guidance.

[1] Google DeepMind, "Antigravity (Gemini 3.8 Flash)," Google AI, Mountain View, CA, USA, 2026. [Online]. Available: https://deepmind.google/technologies/gemini/  
[2] OpenAI, "Codex (GPT-6 Model Family)," OpenAI, San Francisco, CA, USA, 2026. [Online]. Available: https://openai.com/research/  

## 3. Statement of Honesty

By signing below, I confirm that this disclosure is accurate and complete. I understand that undisclosed or false disclosure of AI use is treated as academic misconduct and may result in a 0 grade for the assignment and disciplinary referral.

**Student name (printed):** Bùi Minh Quân  
**Student ID:** 23120337  
**Class / Cohort:** Computer Science / IT (23CLC)  
**Course:** CS423 / CSC15003 — Software Testing  
**Instructor:** Dr. Lam Quang Vu / Dr. Tran Duy Hoang / MSc. Tran Thi Bich Hanh / MSc. Truong Phuoc Loc / MSc. Ho Tuan Thanh  
**Date:** 26/09/2026  
**Signature:** *Bùi Minh Quân* (Digital Signature / Verification Hash: `bmquan.gd@gmail.com / 23120337`)

## References

- ISTQB Foundation Level Syllabus v4.0.1 (International Software Testing Qualifications Board, 2023/2024).
- Hardman, P. (2025). *A Post-AI Learning Taxonomy*.
- Fuster Rabella, M. (2025). OECD Education Working Paper No. 338.
- Perkins, M., Roe, J., & Furze, L. (2025). AI Assessment Scale.
- Anthropic (2025). Building reliable AI test agents — engineering blog.
- DeepEval and Promptfoo documentation — testing frameworks for LLM systems.
