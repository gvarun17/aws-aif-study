# Labs

Last verified: 2026-11-24 (structure only). Check each service's current pricing page before a lab. Prices change.

Each lab has a cost warning, exact steps and a cleanup step.
Run cleanup every time. Check Billing after each lab. Set a low AWS Budgets alert first (AWS Budgets is in the exam's service list, so this also helps your study).

| # | Lab | Main services | Plan day | Task | Cost risk |
|---|---|---|---|---|---|
| 1 | Bedrock playground with 2 models | Amazon Bedrock | 8 | 2.3 | Per-token charges. Request model access first if the console asks. |
| 2 | Knowledge Base with a small S3 document set | Bedrock Knowledge Bases, S3, vector store | 11 | 3.1 | Vector store can bill hourly. Delete it. |
| 3 | Guardrail test | Bedrock Guardrails | 16 | 4.1 | Per-request charges |
| 4 | SageMaker JumpStart model | SageMaker JumpStart | 3 | 1.3 | Endpoint bills hourly. Delete it. |
| 5 | Rekognition / Comprehend / Textract with boto3 | Rekognition, Comprehend, Textract | 2 | 1.2 | Free tier, then per call |
| 6 (optional, new) | Small agent with Strands Agents and a Bedrock model; call one tool | Strands Agents, Bedrock | 6 | 2.1 | Per-token charges. Write the steps from current docs. Not yet written. |
| 7 (optional, new) | Read-only tour of Bedrock AgentCore and its identity features | Bedrock AgentCore | 18 | 5.1 | Check pricing before you create anything. Not yet written. |

Labs 6 and 7 are new because guide v1.2 names Strands Agents, Bedrock AgentCore and agentic AI. They are optional. The exam tests knowledge, not hands-on skill.

Lab files: `labNN-<name>.md`

Lab template rules:
1. Cost warning (first line)
2. Prerequisites
3. Steps with exact console paths or CLI commands
4. Check that it worked
5. **Cleanup** (list every resource to delete, in order)
6. Billing check
