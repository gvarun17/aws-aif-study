# Day 05 — Review: Domain 1 (AI and ML Fundamentals)

- Domain: D1 review
- Task statements: 1.1, 1.2, 1.3
- Time needed: 2 hours
- Last verified: 2026-11-24 (against exam guide v1.2)

## How to use this day

1. Re-read the recaps of Days 01 to 03 (10 minutes).
2. Redraw from memory: the AI nesting diagram, the ML lifecycle, and the service picker (inputs to services).
3. Answer the 10 questions below without notes. Time yourself: 15 minutes.
4. Log results in `scoreboard.md` by task statement.
5. For each wrong answer, re-read the matching lesson section.

## Quick recall list

- AI ⊃ ML ⊃ deep learning ⊃ GenAI ⊃ agentic AI
- Supervised = labels. Unsupervised = groups. Reinforcement = rewards.
- Inference: real-time, batch, asynchronous, serverless
- Regression = number. Classification = category. Clustering = groups.
- Textract = documents. Rekognition = images. Comprehend = text. Transcribe = speech to text. Polly = text to speech. Lex = bots. Personalize = recommendations. SageMaker AI = custom models.
- Recall = catch misses. Precision = avoid false alarms. Drift = monitor and retrain.

## Questions

1. A retailer has customer purchase data with no labels. It wants to find natural customer groups. Which approach fits?
   - A. Supervised classification
   - B. Unsupervised clustering
   - C. Regression
   - D. Reinforcement learning
2. Which statement describes reinforcement learning?
   - A. The model learns from labeled examples only
   - B. An agent learns actions by getting rewards or penalties
   - C. The model groups data without any feedback
   - D. The model translates text
3. A company must score 2 million records overnight. No user waits for the answer. Which inference type fits best?
   - A. Real-time
   - B. Batch
   - C. Streaming chat
   - D. Interactive
4. An internal ML tool is used a few times a day and sits idle most of the time. Which inference type avoids paying for idle capacity?
   - A. Always-on real-time endpoint on a large instance
   - B. Serverless inference
   - C. A dedicated GPU cluster
   - D. Daily full retraining
5. A call centre wants text transcripts of recorded calls. Which service fits?
   - A. Amazon Polly
   - B. Amazon Translate
   - C. Amazon Transcribe
   - D. Amazon Textract
6. A company wants a chatbot with text and voice interfaces. Which service fits?
   - A. Amazon Lex
   - B. Amazon Personalize
   - C. Amazon Rekognition
   - D. Amazon Comprehend
7. A spam filter must avoid sending real customer emails to the spam folder. Which metric matters most?
   - A. Recall
   - B. Precision
   - C. Training time
   - D. Epoch count
8. A team needs full control over a custom algorithm and training code. Which service fits?
   - A. Amazon Polly
   - B. Amazon Textract
   - C. Amazon SageMaker AI
   - D. Amazon Translate
9. Which stage of the ML lifecycle comes right after "deploy"?
   - A. Collect data
   - B. Monitor
   - C. Frame the problem
   - D. Feature engineering
10. Which TWO describe underfitting? (Choose TWO.)
    - A. High error on the training data
    - B. High error on new data too
    - C. Great on training data, poor on new data
    - D. The model memorizes noise in the training data
    - E. The model is always perfect

## Answer key

> Cover this section until you have answered.

1. **B.** No labels and the goal is groups: clustering (unsupervised). A needs labels. C predicts a number. D uses rewards.
2. **B.** Reinforcement learning uses rewards and penalties. A is supervised. C is unsupervised. D is an NLP task.
3. **B.** Batch inference scores large datasets when no one waits. A is for low-latency answers. C, D are not inference types in this list.
4. **B.** Serverless inference scales to zero when idle. A and C keep paid capacity running. D does not help with idle cost.
5. **C.** Transcribe converts speech to text. A is text to speech. B translates text. D reads documents.
6. **A.** Lex builds conversational bots. B recommends items. C analyzes images. D analyzes text.
7. **B.** Precision limits false positives (real mail marked as spam). A: recall limits misses. C, D are not quality metrics.
8. **C.** SageMaker AI is for custom building and training. A, B, D are managed AI services with fixed tasks.
9. **B.** After deploy comes monitoring. A, C, D come earlier.
10. **A and B.** Underfitting means the model is too simple and fails on both training and new data. C and D describe overfitting. E is false.

## Score and next step

- 9–10 correct: move on.
- 7–8: re-read the lessons for the questions you missed.
- Below 7: redo Day 01 to 03 questions tomorrow before Day 06.

Next: Day 06 — agentic AI, MCP and multi-agent systems.
