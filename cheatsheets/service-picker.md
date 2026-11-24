# Service Picker (draft)

Scenario → best AWS service → why not the others.
Built from Days 01 to 20. Last verified: 2026-11-24. Add the scenarios you get wrong in practice.

## AI services (managed, least effort)

| Scenario | Pick | Why not the others |
|---|---|---|
| Read text, tables and forms from scanned invoices | Amazon Textract | Comprehend needs text that already exists. Rekognition is for image content |
| Find sentiment, entities or PII in text | Amazon Comprehend | Textract reads scans. Translate only converts language |
| Detect objects, faces or unsafe content in images and video | Amazon Rekognition | Textract is for document text |
| Convert speech to text | Amazon Transcribe | Polly goes the other way (text to speech) |
| Convert text to speech | Amazon Polly | Transcribe is speech to text |
| Translate between languages | Amazon Translate | Comprehend analyzes, it does not translate |
| Build a text or voice chatbot | Amazon Lex | Personalize recommends items |
| Recommend products or content | Amazon Personalize | Lex is for conversation |
| Build and train a custom model with full control | Amazon SageMaker AI | Managed AI services have fixed tasks |

## GenAI building and running

| Scenario | Pick | Why not the others |
|---|---|---|
| Use FMs through an API with no servers | Amazon Bedrock | SageMaker AI and EC2 mean you manage more |
| Deploy a pre-trained model quickly from a hub | SageMaker JumpStart | Bedrock is API-based, not a model hub you host |
| Use Amazon's own FMs | Amazon Nova (on Bedrock) | Not a vector DB or a service for reports |
| Answer from private, changing documents without retraining | Bedrock Knowledge Bases (RAG) | Fine-tuning does not add live facts |
| Cut cost for a repeated long prompt prefix | Prompt caching | Higher temperature does nothing for cost |
| Steady high traffic or a custom model needs guaranteed capacity | Provisioned Throughput | On-demand has shared capacity |
| Large offline job, no real-time need | Batch inference | Real-time endpoints cost more for this |
| Smaller, cheaper model that copies a larger one | Distillation | Pre-training is far more costly |
| Build agents in code | Strands Agents | AgentCore hosts and runs them |
| Host and operate agents securely at scale | Bedrock AgentCore | Strands is the SDK, not the hosting platform |
| AI coding agent in an IDE (spec-driven) | Kiro | Quick is for business users |
| Agentic workspace for business users (research, BI, automation) | AWS Quick | Kiro is for developers. Q Business is now succeeded by Quick |
| Connect an agent to tools in a standard way | MCP | MCP is a protocol. Gateway makes APIs available as tools |

## Evaluation, responsible AI, security, governance

| Scenario | Pick | Why not the others |
|---|---|---|
| Compare models with human, programmatic or LLM-as-a-judge scores | Bedrock Evaluations | CloudTrail logs calls, it does not score quality |
| Summaries scored against a reference | ROUGE | BLEU is for translation |
| Translation quality | BLEU | ROUGE is for summaries |
| Check RAG answers are supported by sources | Faithfulness metric / contextual grounding check | CPU metrics do not measure truth |
| Block a topic | Guardrails denied topics | Word filters are too narrow |
| Mask PII in prompts and answers | Guardrails sensitive information filters | Macie scans S3 data at rest |
| Find PII in S3 before training | Amazon Macie | Guardrails work on prompts and outputs |
| Record intended use and risk rating of a model | SageMaker Model Cards | Artifact is for AWS reports |
| Private network path to Bedrock | AWS PrivateLink | NAT gateway uses a public path |
| Who called the API and when | AWS CloudTrail | Config tracks configuration |
| Is a resource configured to the rule | AWS Config | CloudTrail logs activity |
| Scan workloads for vulnerabilities | Amazon Inspector | Macie finds sensitive data |
| Download SOC and ISO reports | AWS Artifact | CloudTrail is an activity log |
| Best-practice checks on the account | AWS Trusted Advisor | Inspector scans vulnerabilities |
| Classify how much you own in a GenAI use case | Generative AI Security Scoping Matrix | Not a service. A framework with 5 scopes |

## Sources

Built from the lessons in `days/`. See each lesson for its sources.
