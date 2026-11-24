# In-Scope Services (guide v1.2)

Source: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-in-scope-services.html
Last verified: 2026-11-24. AWS says the list is **not exhaustive** and **can change**. Check it again before the exam.

The "Study depth" column is my own judgment, not AWS's. It uses how often the domain pages name the service.

- **Core** = named in the domain pages. Know what it does, when to pick it, and when not to.
- **Know** = know the one-line purpose.
- **Aware** = recognize the name. Low priority.

## Machine Learning

| Service | Study depth |
|---|---|
| Amazon Bedrock (with Knowledge Bases, Guardrails, Prompt Management, Model Evaluation) | Core |
| Amazon Bedrock AgentCore (with Identity and Policy) | Core |
| Amazon SageMaker AI (with Model Cards) | Core |
| Amazon SageMaker JumpStart | Core |
| Amazon Nova | Know |
| Amazon Comprehend | Core |
| Amazon Lex | Core |
| Amazon Polly | Core |
| Amazon Transcribe | Core |
| Amazon Translate | Core |
| Amazon Rekognition | Know |
| Amazon Textract | Know |
| Amazon Personalize | Know |
| AWS Transform | Aware |

## Developer tools

| Service | Study depth |
|---|---|
| Kiro | Core (named in tasks 1.3 and 2.3) |
| Strands Agents | Core (named in task 2.3) |

## Analytics

| Service | Study depth |
|---|---|
| Amazon OpenSearch Service | Core (vector store) |
| Amazon Quick (AWS now brands it "AWS Quick"; it grew out of QuickSight and succeeds Amazon Q Business) | Core (named in tasks 1.3 and 2.3) |
| AWS Glue, Glue DataBrew, Lake Formation | Aware |
| AWS Data Exchange, Amazon EMR, Amazon Redshift | Aware |

## Database (vector stores and more)

| Service | Study depth |
|---|---|
| Amazon Aurora, Amazon RDS (PostgreSQL), Amazon Neptune | Core (named as vector stores in task 3.1) |
| Amazon DynamoDB, DocumentDB, ElastiCache | Aware |

## Security, identity, compliance and governance

| Service | Study depth |
|---|---|
| AWS IAM | Core |
| AWS KMS (encryption) | Core |
| Amazon Macie | Core |
| AWS Artifact | Core |
| Amazon Inspector | Core |
| AWS CloudTrail | Core |
| AWS Config | Core |
| AWS Trusted Advisor | Core |
| AWS Secrets Manager | Aware |
| AWS Well-Architected Tool | Aware |
| Amazon VPC (with AWS PrivateLink) | Core (PrivateLink is named in task 5.1) |
| Amazon CloudWatch | Know |

## Other listed services

Compute and containers (EC2, Lambda, ECS, EKS), storage (S3, S3 Glacier), CloudFront, AWS Budgets, AWS Cost Explorer: **Aware.** You already know most of them.

## Not on the published in-scope list

Older study material often covers these. The v1.2 in-scope list does not name them. The list is non-exhaustive, so a question *could* still mention one. Study each at "Aware" level only (one line each) until you check the live guide.

| Service or feature | Why it appears in old material |
|---|---|
| Amazon Q Business, Amazon Q Developer | AI assistants (older exam versions) |
| Amazon Kendra | Enterprise search, RAG source |
| Amazon Forecast, Amazon Fraud Detector | "Managed AI service" examples |
| SageMaker Clarify, Model Monitor, Ground Truth, Canvas, Data Wrangler, Feature Store | ML lifecycle and bias examples |
| Amazon Augmented AI (A2I) | Human review of predictions |

The guide itself names these only: SageMaker AI, **SageMaker Model Cards**, JumpStart. It names "Amazon Bedrock Model Evaluation" and "Amazon Bedrock Guardrails" as features.

## Out of scope (examples from AWS's list)

AWS says these will not be tested. Skip them. Examples: AWS WAF, AWS Shield, GuardDuty, Security Hub, Cognito, X-Ray, Route 53, Control Tower, Systems Manager Incident Manager, Amazon MSK, AWS HealthImaging, AWS IoT services.
Full list: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/aif-01-out-of-scope-services.html
