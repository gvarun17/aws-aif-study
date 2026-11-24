# Exam Guide Map (AIF-C01, guide version 1.2)

Source: https://docs.aws.amazon.com/aws-certification/latest/ai-practitioner-01/ai-practitioner-01.html (domain pages 1–5)
Last verified: 2026-11-24. Topics below are my short paraphrase of the guide. Read the official page for exact wording.

Use this map as the checklist. A topic is done when you can explain it in your own words and pass its practice questions.

## Domain 1 — Fundamentals of AI and ML (20%)

| Task | Title | Main topics | Day | Done |
|---|---|---|---|---|
| 1.1 | Explain basic AI concepts and terminologies | AI, ML, deep learning, neural networks, computer vision, NLP, model, algorithm, training vs inference, bias, fairness, fit, LLM, GenAI, **agentic AI**; inference types (batch, real-time, asynchronous, serverless); data types (labeled/unlabeled, tabular, time-series, image, text, structured/unstructured); supervised, unsupervised, reinforcement learning | 1 | [ ] |
| 1.2 | Identify practical use cases for AI | Where AI/ML adds value; **when AI/ML is not right** (cost-benefit, need for an exact outcome); regression, classification, clustering; real-world uses (vision, NLP, speech, recommendation, fraud detection, forecasting, knowledge bases, agentic AI); managed AI services (SageMaker AI, Transcribe, Translate, Comprehend, Lex, Polly); traditional ML vs foundation models | 2 | [ ] |
| 1.3 | Describe the AI/ML development lifecycle | Pipeline stages; sources of FMs (open-source pre-trained vs custom); managed API vs self-hosted; AWS services per stage (Bedrock, Quick, Kiro, SageMaker AI); MLOps (experimentation, repeatability, technical debt, production readiness, monitoring, re-training); model metrics (accuracy, precision, recall, F1) and business metrics (cost per user, ROI, feedback) | 3 | [ ] |

## Domain 2 — Fundamentals of GenAI (24%)

| Task | Title | Main topics | Day | Done |
|---|---|---|---|---|
| 2.1 | Explain the basic concepts of generative AI | Tokens, chunking, embeddings, vectors, prompt engineering, transformer LLMs, FMs, multi-modal, diffusion; use cases; **FM lifecycle**; **token-based pricing**; **context engineering**; **agentic AI basics: multi-agent patterns, MCP, memory, tool use, workflow orchestration** | 4, 6 | [ ] |
| 2.2 | Understand capabilities and limits of GenAI for business problems | Advantages (adaptability, conversation, content); disadvantages (hallucination, interpretability, inaccuracy, nondeterminism); factors to select a model; business value metrics (ROI, efficiency, conversion, ARPU, accuracy, CLV) | 7 | [ ] |
| 2.3 | Describe AWS infrastructure and technologies for GenAI apps | Bedrock, SageMaker AI, JumpStart, **Quick, Kiro, Strands Agents, Bedrock AgentCore**; benefits of AWS GenAI services; infrastructure benefits (security, compliance, safety); cost tradeoffs (token pricing, provisioned throughput, custom models, regional coverage, availability) | 8 | [ ] |

## Domain 3 — Applications of Foundation Models (28%)

| Task | Title | Main topics | Day | Done |
|---|---|---|---|---|
| 3.1 | Design considerations for applications that use FMs | FM selection criteria (cost, modality, latency, language, size, customization, input/output length, **prompt caching**); inference parameters (temperature, length); **RAG** and Bedrock Knowledge Bases; vector stores (OpenSearch Service, Aurora, Neptune, RDS for PostgreSQL); cost of customization (pre-training, fine-tuning, in-context learning, RAG, **model distillation**); AI agents and their business uses | 9, 11 | [ ] |
| 3.2 | Choose effective prompt engineering techniques | Context, instruction, negative prompts; chain-of-thought, zero/single/few-shot, templates; best practices; risks (exposure, poisoning, hijacking, jailbreaking); **Bedrock Prompt Management** | 12 | [ ] |
| 3.3 | Training and fine-tuning process for FMs | Pre-training, fine-tuning, continuous pre-training, distillation; instruction tuning, domain adaptation, transfer learning; data preparation (curation, governance, size, labeling, representativeness, RLHF) | 13 | [ ] |
| 3.4 | Methods to evaluate FM performance | Human evaluation, benchmark datasets, Bedrock Model Evaluation; ROUGE, BLEU, BERTScore, **LLM-as-a-judge**; business fit (productivity, engagement); **evaluating RAG, agents and workflows**; business metrics (task completion, user satisfaction, cost per interaction) | 14 | [ ] |

## Domain 4 — Guidelines for Responsible AI (14%)

| Task | Title | Main topics | Day | Done |
|---|---|---|---|---|
| 4.1 | Develop responsible AI systems | Bias, fairness, inclusivity, robustness, safety, veracity; **Bedrock Guardrails**; responsible model selection (environment, sustainability); legal risks (IP claims, biased output, lost trust, hallucination); dataset characteristics; bias and variance effects; bias/truthfulness monitoring (label quality, human audit, subgroup analysis) | 16 | [ ] |
| 4.2 | Transparent and explainable models | Transparent vs opaque models; tools (SageMaker Model Cards, Bedrock Model Evaluations, open-source models, data and licensing); safety vs transparency tradeoff; human-centered design (feedback, decision transparency) | 17 | [ ] |

## Domain 5 — Security, Compliance, and Governance for AI Solutions (14%)

| Task | Title | Main topics | Day | Done |
|---|---|---|---|---|
| 5.1 | Methods to secure AI systems | IAM roles/policies, encryption, Macie, PrivateLink, shared responsibility, **AgentCore Identity and Policy**, Guardrails; data lineage, cataloging, Model Cards; secure data engineering; app security, threat detection, **prompt injection**, data leakage, output filtering, audit trails, toxicity; **hallucination detection and grounding** (RAG grounding, output validation, confidence scoring) | 18 | [ ] |
| 5.2 | Governance and compliance regulations for AI | Config, Inspector, Artifact, CloudTrail, Trusted Advisor; data governance (lifecycle, logging, residency, monitoring, retention); governance process (policies, review cadence, **Generative AI Security Scoping Matrix**, transparency standards, training) | 19 | [ ] |

Bold items are new or easy to miss in older study material.
