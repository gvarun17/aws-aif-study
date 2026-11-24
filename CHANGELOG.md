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

## Pass 2 — 2026-11-24: lessons for all days

Source of truth: exam guide v1.2 plus AWS docs read on 2026-11-24 (links are in each lesson).

| ID | Pri | File | Change | Why / source |
|---|---|---|---|---|
| C15 | P2 | days/day01…day04, day06–day09, day11–day14, day16–day19 | Wrote 16 lessons with the 9-step format: definition, exam focus, diagram, DevOps link, traps, 3 questions (2 single answer, 1 multiple response), answer key with reasons, recap, sources. | Plan in `plan/README.md`; exam-guide-map |
| C16 | P2 | days/day05, day10, day15, day20 | Wrote 4 review days with 10 mixed questions each and a score rule. | Review day every 5th day |
| C17 | P2 | days/day21, day24 | Wrote the weak-area guide and the final-prep checklist. | Plan |
| C18 | P2 | days/day22, day23 | Wrote mock-day procedures. **The question files are not written.** | Needs 130 new questions; left for a next pass |
| C19 | P2 | cheatsheets/service-picker.md (new) | Scenario → service → why not the others, from Days 01–20. | Day 20 task |
| C20 | P3 | days/README.md | Index, status and question counts (88 written). | – |
| C21 | P1 | cheatsheets/in-scope-services.md, days/day08 | Quick is now branded "AWS Quick". It grew out of QuickSight and succeeds Amazon Q Business. Lessons tell learners not to pick Q Business from old notes. | https://aws.amazon.com/q/business/ and https://aws.amazon.com/quick/faqs/ |
| C22 | P3 | plan/README.md, COACH_PROMPT.md | Changed "5 questions per day" to "3 per lesson day, 10 on review days" so the plan matches the lesson template. | Consistency |

### Facts checked against AWS pages in this pass

| Fact used in lessons | Source |
|---|---|
| AgentCore = platform to build, deploy and operate agents; Runtime, Memory, Gateway, Browser, Code Interpreter; session isolation in microVMs; Identity federates with OIDC providers; resource-based policies for Runtime, Gateway, Memory | AgentCore docs and FAQ |
| Strands Agents = open-source, model-driven SDK | AWS Open Source Blog |
| Kiro = agentic IDE and CLI, spec-driven development, built on Bedrock | kiro.dev, AWS Kiro docs |
| Nova: Micro, Lite, Pro, Premier (understanding); Canvas, Reel (creative); Sonic (speech); Act (browser agents) | Nova user guide and AWS blogs |
| Guardrails: six safeguards, works with non-Bedrock models | Guardrails docs and AWS blogs |
| Prompt caching: implicit and explicit; on-demand only; not supported with batch inference; some models need a minimum prefix (for example 1,024 tokens) | Bedrock prompt caching docs |
| Knowledge Bases: fetch, chunk, embed, store; RetrieveAndGenerate | AWS Prescriptive Guidance |
| Bedrock Evaluations: human, programmatic (BERTScore, F1), LLM-as-a-judge; RAG metrics (context relevance, coverage, correctness, completeness, faithfulness) | Bedrock Evaluations page and What's New posts |
| Model Cards: intended use, risk rating (unknown, low, medium, high) | SageMaker docs |
| Scoping Matrix: five scopes | AWS whitepaper and Security Blog |
| MCP: open standard, client-server, "USB-C for AI apps" | modelcontextprotocol.io, AWS Prescriptive Guidance |

### Open items after pass 2

1. **Mock exams** (`mocks/mock1.md`, `mocks/mock2.md`, 65 questions each) are not written. Days 22 and 23 wait for them.
2. **Lab step files** are not written. Check current console steps and pricing first.
3. **Domain cheat sheets** d1 to d5 are not written. `service-picker.md` exists as a draft.
4. **General-knowledge items** are marked in each lesson's Sources (for example SageMaker inference types, ROUGE and BLEU, metric formulas). Confirm them in AWS docs if you want a source link.
5. **Scope 2 and Scope 4 wording** in the Scoping Matrix table is summarized. Read the AWS Security Blog introduction for exact definitions.
6. **Distillation article** is from the preview period. Check the current Bedrock docs for supported models and billing.
7. **AgentCore "Policy"** is named in the guide. This pass verified resource-based policies and Identity only.
8. **Questions are original and unreviewed by a second person.** Have the coach or a fresh chat re-check the answer keys.
