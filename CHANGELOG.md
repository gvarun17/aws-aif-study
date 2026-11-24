# Changelog

Review pass on 2026-11-24. Original repo: commit `232a481` ("Initial AIF-C01 study repo scaffold").
Source of truth: AWS Certified AI Practitioner exam guide, version 1.2 (2026-10-29).
All changes are in this `aif-study-v2` copy. The original repo is not changed.

Priority: P1 = wrong or outdated, P2 = missing coverage, P3 = clarity and teaching, P4 = polish.

| ID | Pri | File | Change | Why / source |
|---|---|---|---|---|
| C1 | P1 | COACH_PROMPT.md | Replaced the old service list (Q Business, Q Developer, Kendra, Forecast, Fraud Detector, Clarify, Model Monitor, Ground Truth, Canvas, Data Wrangler, Feature Store, A2I) with the guide's in-scope services. Old names moved to "Aware level only". | In-scope list does not name them. https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-in-scope-services.html |
| C2 | P1 | COACH_PROMPT.md | Added agentic AI, MCP, context engineering, prompt caching, model distillation, LLM-as-a-judge, Prompt Management, AgentCore Identity/Policy, Generative AI Security Scoping Matrix, Nova, Quick, Kiro, Strands Agents, AgentCore. | Domain pages 1-5 name these. |
| C3 | P1 | README.md, scoreboard.md, COACH_PROMPT.md | Domain names now match the guide: "Fundamentals of GenAI" and "Security, Compliance, and Governance for AI Solutions". | Exam guide landing page. |
| C4 | P1 | README.md | Replaced "to confirm" status with verified facts. Added guide version 1.2 and date. Weights confirmed unchanged: 20/24/28/14/14. | Exam guide landing page; revisions page. |
| C5 | P1 | exam-day.md | ESL +30: request before scheduling, with the exact console path. Old text said "before booking, if available" (vague). | https://aws.amazon.com/certification/policies/before-testing/ |
| C6 | P2 | exam-day.md | Added: 120 min with ESL (about 110 s per question), 83 s without. Check-in 30 min early for online. No penalty and unanswered = wrong. Compensatory scoring. Cost 100 USD. | Exam guide; AWS exam page; AWS "During testing" page. |
| C7 | P2 | plan/exam-guide-map.md (new) | Map of all 14 task statements to days, with a done checkbox. New or easy-to-miss items in bold. | Domain pages 1-5. |
| C8 | P2 | plan/README.md | Replaced the empty placeholder with a 24-day draft plan. Day split follows the weights (D1 19%, D2 25%, D3 31%, D4 12.5%, D5 12.5%). Review every 5th day. 2 mocks in the last week. | Weights from the guide. The day count is my assumption. Rescale on Day 0. |
| C9 | P2 | cheatsheets/in-scope-services.md (new) | Official in-scope list, with a study-depth column (Core / Know / Aware) and a list of services not on the list. | In-scope and out-of-scope pages. The study-depth column is my judgment. |
| C10 | P2 | labs/README.md | Added plan day and task statement per lab. Added optional labs 6 (Strands Agents) and 7 (AgentCore). Added Budgets alert tip. | Guide v1.2 names Strands Agents and AgentCore. Labs 6 and 7 are not written. |
| C11 | P2 | scoreboard.md | Added task-statement table and mock table. Noted that scoring is compensatory. | Exam guide. The 80% target stays as a study margin. |
| C12 | P3 | templates/lesson-template.md | Removed the HTML `<details>` tag (preference: no HTML). Added task statement, last-verified, sources, multiple-response question, answer key with "why wrong". | Repo style rules. |
| C13 | P3 | mocks/README.md | Added domain split for 65 questions (13/16/18/9/9), tagging by task statement, new-topic coverage. | Weights from the guide. |
| C14 | P4 | all | Added "Last verified" dates and source links. | Review rules. |

## Unverified or open items

1. **Question types.** The AWS guide page I read lists multiple choice and multiple response. Some third-party sites list ordering, matching and case study. I could not confirm this. The repo says to practice both.
2. **ESL accommodation scope.** An older AWS blog says it applies to all future exams once registered. The current policy page says to request it before scheduling each exam. The repo follows the newer page. Request it every time to be safe.
3. **Services not on the list.** The list is non-exhaustive. A question could still mention Q Business, Kendra and others. They are kept at "Aware" level.
4. **Task 2.3 and 1.3 text for "Quick" and "Kiro".** I did not look up what these services do. Lessons must check current AWS docs before they describe them.
5. **Domain weights for D4 and D5 and the five-domain list.** Read from the AWS landing page and confirmed. The domain 4 page text I fetched did not show its own weight line.
6. **Mermaid diagrams:** all 4 render without errors with mermaid-cli. Check the look on GitHub.
7. **No lessons or questions exist yet.** The repo has no day files, cheat sheets or mocks. This pass fixed the framework only. Content must be reviewed when it is written.
