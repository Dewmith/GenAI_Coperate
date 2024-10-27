# Corporate Knowledge Base Assistant

## Project Overview

The **Corporate Knowledge Base Assistant** is designed to assist employees by answering questions based on the organization's internal documentation. This includes HR policies, internal workflows, and IT support guidelines, providing quick, accurate answers without the need to sift through extensive documents.

### Use Case
Provide employees with accurate and prompt answers related to:
- HR policies
- Internal workflows
- IT support guidelines

### Key Challenges
- Document organization
- Maintaining confidentiality
- Adapting to updates in internal policies

---

## 1. Sample Questions and Expected Answers

### General HR Policies Questions
#### **General HR Policies Questions**
- **Q1: What is the process for requesting time off?**
  
    1. Time your request well in advance.
    2. Clearly communicate your reasons for the time off request.
    3. Adhere to company policies and guidelines.
    4. Demonstrate how your work will be managed in your absence.
    5. Maintain a professional and respectful tone in your request.

- **Q2: What is the policy on remote work at BNP Paribas?**
  - BNP Paribas allows its employees to work remotely for one or two days per week. With new technologies, they can work just as efficiently at home as in the office.

#### **IT Support Guidelines**
- **Q3: What is the process for requesting IT support?**
  
    1. Identify the Issue.
    2. Submit a Support Request.
    3. Provide Necessary Details.
    4. Priority Assignment.
    5. Track the Request.

- **Q4: How do I securely access company resources from a remote location?**
  
    - Use a VPN (Virtual Private Network).
    - Enable Two-Factor Authentication (2FA).
    - Access via Secure Connection (HTTPS).
    - Use a Company-Provided Device.
    - Follow Security Policies.
    - Avoid Public Wi-Fi.
    - Keep Software Updated.
    - Secure Storage of Company Data.

#### **Miscellaneous**
- **Q5: How can I give feedback about company policies or procedures?**
  
    1. Clearly state which policy or procedure you're referring to.
    2. Frame your feedback in a way that suggests improvements.
    3. Highlight impacts on productivity, employee morale, or company goals.
    4. Ensure feedback aligns with the company’s core values or mission.
    5. Use past examples to support your suggestions.
    6. Invite a dialogue to understand the current procedures better.

- **Q6: What are the emergency procedures for the office?**
  
    1. Know the nearest exit. Familiarize yourself with alternate exits.
    2. Avoid panic. Remain calm and follow instructions.
    3. Stop rumors to prevent confusion.
    4. Use the telephone for emergencies only.

#### **Internal Workflows**
- **Q7: What is the onboarding process for new employees?**
  - Onboarding includes orientation, training, socialization, and ongoing support to integrate new employees effectively.

- **Q8: What steps should I follow to request a new software or tool?**
  - 
    1. Define the scope and objectives.
    2. Create a detailed project plan.
    3. Select the software you need.
    4. Execute the project plan.
    5. Configure and integrate your software.
    6. Train and adopt your software.
    7. Go live.
    8. Support, maintain, and evaluate.

- **Q9: What is the protocol for reporting workplace harassment?**
  - 
    1. Try to resolve the issue.
    2. Compile evidence.
    3. Escalate to management or HR.
    4. Prevent retaliation.


---

## 2. Benchmarks for Evaluation

### Selected Benchmarks
Based on the project requirements, we've chosen the following benchmarks:

1. **SQuAD**  
   - **Description:** A dataset for evaluating question answering systems.
   - **Link:** [SQuAD Dataset](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1194/reports/default/15791990.pdf)
   - **Relevance:** Essential for measuring the accuracy of answers related to company policy or IT support questions.

2. **MultiWOZ**  
   - **Description:** A dialogue dataset for multi-turn, task-oriented conversations.
   - **Link:** [MultiWOZ Dataset](https://github.com/Tomiinek/MultiWOZ_Evaluation)
   - **Relevance:** Ensures the assistant can handle complex queries requiring multiple steps.

3. **Banking77**  
   - **Description:** A dataset for intent recognition in the banking domain.
   - **Link:** [Banking77 Dataset](https://huggingface.co/lxyuan/banking-intent-distilbert-classifier)
   - **Relevance:** Useful for recognizing employee intents regarding policies or IT procedures.

4. **SuperGLUE**  
   - **Description:** A benchmark for evaluating natural language understanding systems on a variety of tasks.
   - **Link:** [SuperGLUE Benchmark](https://super.gluebenchmark.com/diagnostics)
   - **Relevance:** Provides a comprehensive evaluation of the assistant's language understanding capabilities.

5. **XNLI**  
   - **Description:** A benchmark for cross-lingual natural language inference.
   - **Link:** [XNLI Benchmark](https://arxiv.org/pdf/1809.05053)
   - **Relevance:** Ensures the assistant can understand and infer meaning across multiple languages.

---

## 3. Validation Policy

### Answer Quality Metrics
- **Accuracy**: Ensure the assistant provides precise answers according to company documentation.
  - **Why**: Accuracy is critical to avoid misinformation and ensure employee trust.
- **Relevance**: Assess how well the answer aligns with the specific context of the question.
  - **Why**: Relevant answers improve user satisfaction and reduce follow-up questions.

### User Experience Metrics
- **Response Time**: Measure how quickly the assistant provides an answer.
  - **Why**: Quick responses improve usability and efficiency.
- **User Satisfaction**: Collect user feedback through surveys or ratings.
  - **Why**: Direct user feedback is a key indicator of system effectiveness.

### Performance Metrics
- **Latency**: Measure the time taken to process a query.
  - **Why**: Low latency ensures a smoother user experience, especially for frequent queries.
- **Scalability**: Assess the ability to handle a high volume of queries.
  - **Why**: Important for maintaining service quality as user demand increases.

### Cost Metrics
- **Operational Costs**: Track the computational cost for maintaining and updating the assistant.
  - **Why**: Helps in budget planning and optimizing resource usage.
- **Training Costs**: Measure the cost associated with model training and updates.
  - **Why**: Ensures the project remains cost-efficient.

---

## 4. Model Benchmark Scores

| Benchmark       | Model                  | Score | Description                       |
|-----------------|------------------------|-------|-----------------------------------|
| SQuAD           | BERT                   | 88.5 (SQuAD 1.1), 81.4 (SQuAD 2.0) | Evaluates question-answering accuracy. |
| MultiWOZ        | RoBERTa                | BLEU: 18.0, Inform: 83.5, Success: 75.0 | Measures task-oriented dialogue accuracy. |
| Banking77       | DistilBERT             | 92.4% | Assesses intent recognition accuracy. |
| SuperGLUE       | Various                | Varies by task normally 71.5% (average) | Evaluates natural language understanding across multiple tasks. |
| XNLI            | Various                | Varies by language, normally 79.2% (average) | Evaluates cross-lingual natural language inference. |


### In MultiWOZ Score
- **BLEU (Bilingual Evaluation Understudy)**: Measures the quality of text generated by the model by comparing it to reference texts. Higher scores indicate better performance.
- **Inform**: Evaluates whether the dialogue system provides an appropriate entity in response to the user's request.
- **Success**: Assesses whether the system successfully provides all the requested attributes in its response.



