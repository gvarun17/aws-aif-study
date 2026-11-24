# Day 08 — AWS Infrastructure and Services for GenAI

- Domain: D2 Fundamentals of GenAI
- Task statements: 2.3 (also supports 1.3)
- Time needed: 3 hours (plus 1 hour for Lab 1)
- Hands-on task: Lab 1 (Bedrock playground with 2 models)
- Last verified: 2026-11-24 (against exam guide v1.2)

## 1. Definition

AWS offers several ways to build GenAI applications. They differ in **how much you manage**.

```
More control, more work                          Less work, less control
SageMaker AI  ◄──────  Bedrock  ◄──────  Quick (business apps)
 (build/train/host)    (FMs by API)      Kiro (coding agent IDE)
```

## 2. Why it matters (exam focus)

Task 2.3 asks you to **describe** the services, their benefits and cost trade-offs. Most questions are "which service fits this need".

## 3. Service map

| Service | What it is | Pick it when |
|---|---|---|
| **Amazon Bedrock** | Managed service to use FMs from Amazon and other providers through one API. Has Knowledge Bases, Guardrails, agents, evaluations, prompt management | You want FMs without managing servers |
| **Amazon SageMaker AI** | Build, train, tune and host ML models and FMs | You need full control or custom training |
| **SageMaker JumpStart** | A hub of pre-trained models and solution templates | You want a ready model to deploy and tune quickly |
| **Amazon Nova** | Amazon's own FM family on Bedrock | You want AWS models with good price-performance |
| **Strands Agents** | Open-source SDK to build agents (model-driven) | You build agents in code |
| **Amazon Bedrock AgentCore** | Platform to deploy and operate agents securely at scale. Runtime, Memory, Gateway, Identity, Browser, Code Interpreter | You run agents in production |
| **Kiro** | Agentic IDE and CLI for spec-driven development: prompt to requirements, design, tasks, code and tests. Built on Bedrock | Developers want an AI coding agent |
| **Amazon Quick (AWS Quick)** | Agentic AI workspace for business users: research, business intelligence, automation. Grew out of QuickSight and is the next step after Amazon Q Business | Business users need answers and actions across company data |

## 4. Amazon Nova family

| Group | Models |
|---|---|
| Understanding (text, image, video in; text out) | Nova Micro, Lite, Pro, Premier |
| Creative content | Nova Canvas (image), Nova Reel (video) |
| Speech-to-speech | Nova Sonic |
| Agents that use browsers | Nova Act |

Newer Nova versions may exist. Check the Nova user guide for the current list.

## 5. Benefits of AWS GenAI services

- Fast start: no model hosting for managed services
- Choice of models
- Built-in security, privacy and compliance features (IAM, encryption, VPC endpoints)
- Responsible AI tools (Guardrails, evaluation)
- Pay as you go

## 6. Cost trade-offs

| Option | How you pay | Use when |
|---|---|---|
| On-demand | Per input and output token | Variable or low traffic, testing |
| Batch inference | Run jobs asynchronously | Large offline jobs, no real-time need |
| Provisioned Throughput | Dedicated capacity, hourly, with commitment options | Steady high traffic. Also used for custom models |
| Custom model | Training cost, plus storage and hosting | The task needs specialized behavior |

Other cost levers: prompt caching, a smaller model, shorter prompts and answers (Day 09). Region choice affects model **availability**, latency, price and data rules.

## 7. DevOps link

On-demand is like pay-per-request serverless. Provisioned Throughput is like reserved capacity. SageMaker AI is like running your own cluster. Bedrock is like a managed API.

## 8. Exam traps

- "No infrastructure to manage, FMs by API" is **Bedrock**.
- "Custom training, full control" is **SageMaker AI**.
- "Pre-trained model hub" is **JumpStart**.
- Quick is for **business users**. Kiro is for **developers**.
- Do not choose Amazon Q Business from old notes: AWS now calls Quick its next evolution.

## 9. Practice questions

1. A team wants to use foundation models through an API and manage no infrastructure. Which service fits?
   - A. Amazon SageMaker AI notebooks on self-managed GPUs
   - B. Amazon Bedrock
   - C. Amazon EC2 with self-installed models
   - D. AWS Config
2. A workload has steady, high traffic and needs guaranteed capacity for a custom model. Which Bedrock option fits?
   - A. On-demand
   - B. Provisioned Throughput
   - C. Prompt Management
   - D. Guardrails
3. Which TWO statements about Amazon Nova are correct? (Choose TWO.)
   - A. It is a family of foundation models available on Amazon Bedrock
   - B. It includes understanding models named Micro, Lite, Pro and Premier
   - C. It is a vector database
   - D. It is used only for billing reports
   - E. It runs only outside AWS

## 10. Answer key

> Cover this section until you have answered.

1. **B.** Bedrock offers FMs by API with no servers to manage. A, C require you to manage infrastructure. D checks resource configuration.
2. **B.** Provisioned Throughput gives dedicated capacity and is the way to run many custom models. A is pay per token with shared capacity. C stores prompts. D filters content.
3. **A and B.** Nova is Amazon's FM family on Bedrock. Micro, Lite, Pro and Premier are its understanding models. C, D, E are false.

## Recap

1. Bedrock = FMs by API. SageMaker AI = build and train. JumpStart = model hub.
2. Strands builds agents. AgentCore runs them. Kiro helps developers. Quick helps business users.
3. On-demand per token. Provisioned for steady load. Batch for offline jobs.

## Sources

- Bedrock docs (custom models, batch, provisioned throughput): https://docs.aws.amazon.com/bedrock/
- Bedrock cost options: https://aws.amazon.com/bedrock/cost-optimization/
- Nova overview: https://docs.aws.amazon.com/nova/latest/userguide/what-is-nova.html
- Strands Agents: https://aws.amazon.com/blogs/opensource/introducing-strands-agents-an-open-source-ai-agents-sdk/
- AgentCore overview: https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/what-is-bedrock-agentcore.html
- Kiro: https://kiro.dev/ide/ and https://aws.amazon.com/documentation-overview/kiro/
- AWS Quick: https://aws.amazon.com/quick/faqs/ and https://aws.amazon.com/q/business/
- SageMaker JumpStart description is from general knowledge. Confirm in the SageMaker AI docs.

Next: Day 09 — design considerations for FM applications.
