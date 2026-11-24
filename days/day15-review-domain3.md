# Day 15 — Review: Domain 3 (Applications of Foundation Models)

- Domain: D3 review (the largest domain, 28%)
- Task statements: 3.1, 3.2, 3.3, 3.4
- Time needed: 2.5 hours
- Last verified: 2026-11-24 (against exam guide v1.2)

## How to use this day

1. Re-read the recaps of Days 09, 11, 12, 13 and 14 (15 minutes).
2. Draw from memory: the RAG flow and the customization cost ladder.
3. Answer the 10 questions without notes. Time yourself: 15 minutes.
4. Log results in `scoreboard.md` by task statement (3.1 to 3.4).
5. Re-read the lesson for every wrong answer.

## Quick recall list

- Selection: cost, modality, latency, language, size, customization, context length, Region.
- Lower temperature = more consistent. Max tokens caps length. Prompt caching = reuse repeated prefix.
- RAG = retrieve then generate. Vector stores: OpenSearch, Aurora, RDS PostgreSQL, Neptune.
- Cost ladder: prompts, examples, RAG, fine-tuning, continued pre-training, pre-training.
- Few-shot = examples. Chain-of-thought = steps. Risks = exposure, poisoning, hijacking, jailbreaking.
- Continued pre-training = unlabeled domain text. Fine-tuning = labeled pairs. Distillation = small student.
- ROUGE = summaries. BLEU = translation. BERTScore = meaning. Faithfulness = hallucination check.

## Questions

1. A company wants a smaller, cheaper model that copies the behavior of a larger model for one task. Which method fits?
   - A. Distillation
   - B. Pre-training from scratch
   - C. Batch inference
   - D. Prompt injection
2. Which customization option is usually the cheapest to try first?
   - A. Pre-training from scratch
   - B. Prompt engineering
   - C. Continued pre-training
   - D. Fine-tuning on a large dataset
3. A support bot must always cite the exact policy paragraph it used. Which design helps most?
   - A. RAG that returns source attribution with the answer
   - B. A higher temperature
   - C. A shorter max token limit
   - D. Removing the system prompt
4. What is a good reason to use chain-of-thought prompting?
   - A. The task needs multi-step reasoning
   - B. You want to skip testing
   - C. You want to hide the answer
   - D. You want to train a new model
5. An attacker plants misleading text in documents that a RAG app retrieves, so the model gives bad answers. Which risk is this closest to?
   - A. Poisoning
   - B. Right-sizing
   - C. Load balancing
   - D. Tokenization
6. Which dataset is used to fine-tune a model for a customer-support task?
   - A. Labeled prompt and response pairs
   - B. Unlabeled video only
   - C. Random numbers
   - D. Billing reports
7. Which metric is typically used to check summaries against a reference?
   - A. ROUGE
   - B. BLEU
   - C. Throughput
   - D. IOPS
8. A RAG app returns answers that are not supported by the retrieved text. Which metric checks this?
   - A. Faithfulness
   - B. CPU utilization
   - C. Subnet count
   - D. Cache hit rate
9. Which TWO are inference parameters or settings that you can change per request? (Choose TWO.)
   - A. Temperature
   - B. Maximum length (max tokens)
   - C. The company's VPC CIDR
   - D. The IAM user name
   - E. The S3 bucket policy
10. Which TWO are valid ways to lower the cost of a repeated-prompt workload on Bedrock? (Choose TWO.)
    - A. Use prompt caching for the stable prefix
    - B. Use a smaller model for easy tasks
    - C. Add more tokens to every prompt
    - D. Always use the largest model
    - E. Turn off all evaluation

## Answer key

> Cover this section until you have answered.

1. **A.** Distillation trains a small "student" from a large "teacher". B is very costly. C is a processing mode. D is an attack.
2. **B.** Prompt engineering needs no training. A, C, D need data and compute.
3. **A.** RAG with source attribution lets the app cite the passage. B changes variation. C limits length. D removes guidance.
4. **A.** Chain-of-thought helps with multi-step reasoning. B, C, D are not its purpose.
5. **A.** Bad data inserted to bend model output is poisoning. B, C, D are unrelated.
6. **A.** Fine-tuning uses labeled examples. B, C, D are not usable training data for this task.
7. **A.** ROUGE is for summaries. B is for translation. C, D are performance measures.
8. **A.** Faithfulness checks that the answer is supported by the context. B, C, D are infrastructure metrics.
9. **A and B.** Temperature and max tokens are per-request settings. C, D, E are account or network settings.
10. **A and B.** Caching and a right-sized model both lower cost. C, D raise cost. E removes quality control.

## Score and next step

- 9–10 correct: move on.
- 7–8: re-read the lessons for the missed questions.
- Below 7: redo the Day 09 to 14 questions tomorrow before Day 16. D3 is 28% of the exam, so do not skip this.

Next: Day 16 — responsible AI and Guardrails.
