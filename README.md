# AWS Certified AI Practitioner (AIF-C01) — Study Repo

This repo holds my study plan, lessons, labs, practice and tracking for the AWS AIF-C01 exam.
A coach (Claude) follows the rules in [`COACH_PROMPT.md`](COACH_PROMPT.md).

## Exam facts (to confirm against the live exam guide on Day 0)

| Item | Value |
|---|---|
| Questions | 65 (50 scored, 15 unscored) |
| Time | 90 minutes |
| Passing score | 700 / 1000 |
| Delivery | Pearson VUE (online or test centre) |

| Domain | Weight | Study-time share |
|---|---|---|
| D1 Fundamentals of AI and ML | 20% | 20% |
| D2 Fundamentals of Generative AI | 24% | 24% |
| D3 Applications of Foundation Models | 28% | 28% |
| D4 Guidelines for Responsible AI | 14% | 14% |
| D5 Security, Compliance and Governance for AI Solutions | 14% | 14% |

> Status: the values above come from the coach prompt. Day 0 checks them against
> the official guide (aws.amazon.com/certification). Any change gets recorded here.

## Study flow

```mermaid
flowchart LR
    A[Day 0: check live exam guide] --> B[5 diagnostic questions]
    B --> C[Build day-by-day plan]
    C --> D[Daily lesson + lab + 5 questions]
    D --> E{Every 5th day?}
    E -- yes --> F[Review day]
    E -- no --> D
    F --> G[Update scoreboard]
    G --> D
    D --> H[Last week: 2 timed mock exams]
    H --> I[Review every wrong answer]
    I --> J[Exam day]
```

## Repo layout

```
aws-aif-study/
├── COACH_PROMPT.md      # Rules for the coach (source of truth)
├── scoreboard.md        # % correct by domain, updated weekly
├── exam-day.md          # Booking steps and exam-day tactics
├── plan/                # Day-by-day study plan
├── days/                # One lesson file per day (dayNN-topic.md)
├── labs/                # Low-cost hands-on labs with cleanup steps
├── cheatsheets/         # One page per domain + service picker table
├── mocks/               # Mock exams and wrong-answer reviews
└── templates/           # Lesson template
```

## How each lesson is taught

1. Plain definition
2. Why it matters and where the exam tests it
3. Diagram
4. Real example (DevOps / cloud case)
5. Comparison table with look-alike options
6. "Pick this when / not this when" rule
7. Exam traps and keywords
8. 3 practice questions, then explanations

## Personal settings (fill in)

- Study time: `[X]` hours per day
- Duration: `[Y]` weeks
- Target exam date: `[date]`
- Time zone: IST
