# Audit — aws-aif-study (commit 232a481)

Date: 2026-11-24. Standard: exam guide v1.2 (2026-10-29).
Scope: 10 files, about 2,000 words. The repo is a scaffold. It has **no lessons, cheat sheets, labs or mock questions yet.**
Scores: 1 (poor) to 5 (good). "n/a" = nothing to judge yet.

| # | Criterion | Before | After | Main finding |
|---|---|---|---|---|
| 1 | Accuracy | 3 | 5 | Weights and exam facts were right. Two domain names were off. ESL step was vague. |
| 2 | Currency | 2 | 4 | Service list is from an older exam version. Missing all 2026 topics (agentic AI, MCP, AgentCore, Strands, Kiro, Nova, Quick). |
| 3 | Coverage | 2 | 4 | No map to the 14 task statements. No in-scope list. Labs ignore agents. |
| 4 | Depth and balance | n/a | n/a | No lessons yet. Draft plan follows the weights within a few points. |
| 5 | Clarity | 4 | 4 | Short and clear already. |
| 6 | Teaching quality | 3 | 4 | Good 8-step order. Added task statement link, sources and last-verified date. |
| 7 | Practice | 2 | 3 | Only a rule ("5 questions a day"). Added multiple-response format, answer key with "why wrong", mock split. No questions written yet. |
| 8 | Visuals | 4 | 4 | Two Mermaid flows. Added a plan flow. Not rendered here. |
| 9 | Style (STE) | 4 | 4 | Mostly simple English. Tables are dense in places. |
| 10 | Consistency | 3 | 4 | Domain names differ between files. Fixed. |

## Claims marked VERIFY and their result

| Claim in the old repo | Result |
|---|---|
| 65 questions, 50 scored, 15 unscored | Confirmed (exam guide) |
| 90 minutes | Confirmed (AWS exam page) |
| Pass score 700 / 1000 | Confirmed (exam guide) |
| Weights 20/24/28/14/14 | Confirmed (exam guide) |
| "Fundamentals of Generative AI" | Wrong name. Guide says "Fundamentals of GenAI". Fixed. |
| ESL +30: "request before booking, if available" | Confirmed, and made exact. Request before scheduling. |
| "No penalty for wrong answers" | Confirmed. Unanswered also counts as wrong. |
| "Managed / serverless option usually wins" | Not in any source. Kept as a labeled heuristic. |
| Service list in COACH_PROMPT | Outdated. Fixed (C1, C2). |
| Metrics AUC, RMSE | Not in the guide. Kept as extras. |
| "Sign in to AWS Training and Certification" | Wording changed to "AWS Certification account". |

## Top remaining gaps

1. (Done in pass 2) Lessons for all days. Review each against `plan/exam-guide-map.md` with a second reader.
2. Write the 2 mock exams (65 questions each), all tagged by task statement. Daily questions are done (88).
3. Write lab files. Check current docs for every console path. Price each lab.
4. Confirm what Quick, Kiro, AgentCore and Strands do from AWS docs before teaching them.
5. Check the guide revisions page every week until the exam.


## Update — pass 2 (lessons written)

| # | Criterion | After pass 1 | After pass 2 | Note |
|---|---|---|---|---|
| 2 | Currency | 4 | 4 | Lessons use sources read on 2026-11-24. Quick rebrand caught. |
| 3 | Coverage | 4 | 5 | All 14 task statements have a lesson. |
| 4 | Depth and balance | n/a | 4 | Lesson days follow the weights. Some topics are short (see open items). |
| 6 | Teaching quality | 4 | 4 | Same 9-step format in every lesson. |
| 7 | Practice | 3 | 4 | 88 questions with reasons. Mock exams still missing. |

Remaining gaps: mock exams (130 questions), lab step files, domain cheat sheets, a second-person check of all answer keys.
