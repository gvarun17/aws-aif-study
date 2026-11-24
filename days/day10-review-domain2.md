# Day 10 — Review: Domain 2 (GenAI Fundamentals)

- Domain: D2 review (plus Day 09 topics)
- Task statements: 2.1, 2.2, 2.3, 3.1 (part 1)
- Time needed: 2 hours
- Last verified: 2026-11-24 (against exam guide v1.2)

## How to use this day

1. Re-read the recaps of Days 04, 06, 07, 08 and 09 (15 minutes).
2. Draw from memory: the agent loop, the AWS service map (SageMaker AI, Bedrock, Quick, Kiro, Strands, AgentCore), and the cost options table.
3. Answer the 10 questions without notes. Time yourself: 15 minutes.
4. Log results in `scoreboard.md` by task statement.
5. Re-read the lesson for every wrong answer.

## Quick recall list

- Token = text piece. Embedding = meaning as vector. Context window = max tokens per request.
- Hallucination = confident false answer. Nondeterminism = outputs vary.
- Agent = model + tools + memory + instructions. MCP = open connector standard.
- Strands = build agents. AgentCore = run agents. Kiro = developer IDE agent. Quick = business-user workspace.
- On-demand = per token. Provisioned = dedicated capacity. Batch = offline jobs.
- Lower temperature = more consistent. Prompt caching = reuse repeated prefix.

## Questions

1. What unit does an on-demand foundation model request use for billing?
   - A. Tokens
   - B. IAM roles
   - C. S3 objects
   - D. VPC subnets
2. Which statement about the context window is correct?
   - A. It is the maximum number of tokens the model can handle in one request
   - B. It is the number of users that can sign in
   - C. It is the size of the training data
   - D. It is a type of vector database
3. A company wants an agent to call its internal REST APIs as tools through a common protocol. Which pairing is best?
   - A. MCP, with AgentCore Gateway making APIs available as tools
   - B. SMTP, with Amazon Polly
   - C. BGP, with AWS Config
   - D. TLS, with Amazon Rekognition
4. Which is the best reason to use a workflow instead of an agent?
   - A. The steps are known and fixed, and you want lower cost and risk
   - B. You want the model to choose any step it likes
   - C. You want to avoid logging
   - D. You want unlimited autonomy
5. A model invents a source that does not exist. Which fix is most direct?
   - A. Ground answers with retrieval from trusted documents and require citations
   - B. Increase the temperature
   - C. Remove all instructions
   - D. Use a larger image size
6. Which TWO are strengths of GenAI for business? (Choose TWO.)
   - A. One model can adapt to many tasks with new prompts
   - B. It always gives identical, exact results
   - C. It can draft and summarize content quickly
   - D. It never needs human review
   - E. It cannot make mistakes
7. A developer team wants an AI coding agent in an IDE that turns prompts into specs, tasks and code. Which service fits?
   - A. Kiro
   - B. Amazon Lex
   - C. Amazon Textract
   - D. Amazon Translate
8. Business users want an agentic workspace for research, business intelligence and automation across company data. Which service fits?
   - A. Amazon Rekognition
   - B. AWS Quick
   - C. Amazon Polly
   - D. AWS CloudTrail
9. Which setting caps the length of a model's answer?
   - A. Maximum length (max tokens)
   - B. Temperature
   - C. Embedding size
   - D. Region
10. Which TWO describe prompt caching? (Choose TWO.)
    - A. It reuses a repeated prompt prefix
    - B. It can reduce latency and input token cost
    - C. It trains the model on your data
    - D. It works with the batch inference API
    - E. It replaces the need for a system prompt

## Answer key

> Cover this section until you have answered.

1. **A.** Billing is per input and output token. B, C, D are not billing units for model calls.
2. **A.** The context window is the token limit for one request. B, C, D are unrelated.
3. **A.** MCP is the open standard. AgentCore Gateway can turn APIs and Lambda functions into MCP-compatible tools. B, C, D pair unrelated protocols and services.
4. **A.** Use a workflow for known steps: it costs less and has less risk. B, C, D are risky or false.
5. **A.** Grounding with RAG and citations limits invented content. B increases variation. C removes guidance. D is irrelevant.
6. **A and C.** Adaptability and fast drafting are strengths. B, D, E are false for GenAI.
7. **A.** Kiro is an agentic IDE with spec-driven development. B is a chatbot service. C reads documents. D translates text.
8. **B.** Quick is the agentic workspace for business users. A, C, D do other jobs.
9. **A.** Max tokens caps answer length. B controls variation. C is a vector property. D is a location.
10. **A and B.** Caching reuses a stable prefix and cuts cost and latency. C is false. D is false (not supported with batch inference). E is false.

## Score and next step

- 9–10 correct: move on.
- 7–8: re-read the lessons for the missed questions.
- Below 7: redo the Day 04 to 09 questions tomorrow before Day 11.

Next: Day 11 — RAG, Knowledge Bases and customization cost.
