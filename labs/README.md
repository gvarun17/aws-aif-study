# Labs

Each lab has a cost warning, exact steps and a cleanup step.
Run cleanup every time. Check Billing after each lab.

| # | Lab | Main services | Cost risk |
|---|---|---|---|
| 1 | Bedrock playground with 2 models | Amazon Bedrock | Per-token charges |
| 2 | Knowledge Base with a small S3 document set | Bedrock Knowledge Bases, S3, vector store | Vector store can bill hourly — delete it |
| 3 | Guardrail test | Bedrock Guardrails | Per-request charges |
| 4 | SageMaker JumpStart model | SageMaker JumpStart | Endpoint bills hourly — delete it |
| 5 | Rekognition / Comprehend / Textract with boto3 | Rekognition, Comprehend, Textract | Free tier, then per-call |

Lab files: `labNN-<name>.md`
