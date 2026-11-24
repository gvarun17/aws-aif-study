# Day 20 — Review: Domains 4 and 5

- Domain: D4 and D5 review
- Task statements: 4.1, 4.2, 5.1, 5.2
- Time needed: 2 hours
- Last verified: 2026-11-24 (against exam guide v1.2)

## How to use this day

1. Re-read the recaps of Days 16 to 19 (15 minutes).
2. Draw from memory: the Guardrails input/output flow and the security layers diagram.
3. Answer the 10 questions without notes. Time yourself: 15 minutes.
4. Log results in `scoreboard.md` by task statement.
5. Finish `cheatsheets/service-picker.md` (scenario, best service, why not the others).

## Quick recall list

- Guardrails: content filters, denied topics, word filters, PII filters, contextual grounding, automated reasoning.
- Model Cards = intended use, risk rating, training and evaluation record.
- Macie = PII in S3. PrivateLink = private path. KMS = encryption. CloudTrail = audit. Artifact = reports. Config = rules. Inspector = vulnerabilities. Trusted Advisor = checks.
- Scoping Matrix: 1 consumer, 2 enterprise, 3 pre-trained, 4 fine-tuned, 5 self-trained.
- Ground answers with RAG and checks. Humans review high-impact decisions.

## Questions

1. Which Guardrails safeguard masks PII in prompts and responses?
   - A. Sensitive information filters
   - B. Denied topics
   - C. Contextual grounding checks
   - D. Provisioned Throughput
2. A team wants to block the topic "medical diagnosis" in a general chatbot. Which policy fits?
   - A. Denied topics
   - B. Word filters only for the word "medical"
   - C. Batch inference
   - D. Model distillation
3. Which dimension of responsible AI means the system gives truthful, accurate output?
   - A. Veracity
   - B. Latency
   - C. Throughput
   - D. Elasticity
4. Which feature records a model's risk rating (low, medium, high) and intended use?
   - A. SageMaker Model Cards
   - B. Amazon Polly
   - C. Amazon Translate
   - D. Amazon Lex
5. A team must keep a human in the loop for loan decisions made with AI. This is an example of what?
   - A. Human-centered design
   - B. Prompt caching
   - C. Model distillation
   - D. Serverless inference
6. A company wants private connectivity from its VPC to Bedrock with no internet path. Which fits?
   - A. AWS PrivateLink (VPC interface endpoint)
   - B. A public load balancer
   - C. Amazon Polly
   - D. AWS Budgets
7. Which service lets a team download SOC and ISO reports about AWS?
   - A. AWS Artifact
   - B. AWS Config
   - C. Amazon Inspector
   - D. Amazon Macie
8. A company builds a chatbot on a pre-trained model from Bedrock. Which Scoping Matrix scope is this?
   - A. Scope 3
   - B. Scope 1
   - C. Scope 5
   - D. Scope 0
9. Which TWO are valid controls against prompt injection in an agent that calls tools? (Choose TWO.)
   - A. Use Guardrails prompt-attack filtering
   - B. Give the agent narrow, least-privilege tool permissions
   - C. Give the agent admin access so it never fails
   - D. Hide all logs
   - E. Raise the temperature
10. Which TWO describe good data governance for AI? (Choose TWO.)
    - A. Define retention and deletion rules
    - B. Keep data in approved Regions (residency)
    - C. Keep all data forever with no review
    - D. Allow everyone to edit training data
    - E. Skip logging to save cost

## Answer key

> Cover this section until you have answered.

1. **A.** Sensitive information filters detect and mask PII. B blocks topics. C checks grounding. D is capacity.
2. **A.** Denied topics block a topic you define. B is too narrow for a topic. C, D do not filter content.
3. **A.** Veracity means truthful and accurate. B, C, D are performance terms.
4. **A.** Model Cards hold intended use and risk rating. B, C, D are AI services for other tasks.
5. **A.** Human oversight is part of human-centered design. B, C, D are cost or model topics.
6. **A.** PrivateLink gives private connectivity. B uses a public path. C, D do not provide it.
7. **A.** Artifact gives compliance reports. B checks configuration. C scans for vulnerabilities. D finds sensitive data.
8. **A.** Building an app on a pre-trained FM is Scope 3. B is consumer apps. C is self-trained models. D does not exist.
9. **A and B.** Filter attacks and narrow tool permissions. C is unsafe. D removes audit. E does not stop injection.
10. **A and B.** Retention rules and residency are core data governance. C, D, E are poor practice.

## Score and next step

- 9–10 correct: move on.
- 7–8: re-read the lessons for the missed questions.
- Below 7: redo the Day 16 to 19 questions tomorrow.

Next: Day 21 — fix weak areas.
