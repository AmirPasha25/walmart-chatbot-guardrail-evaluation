# Walmart Chatbot Guardrail Evaluation

<img src="IMG_8227.PNG" width="50%">
<img src="IMG_8226.PNG" width="50%">

This project evaluates the behavior of Walmart’s grocery assistant chatbot to understand how effectively it enforces domain guardrails, intent routing, and topic boundaries. The study tests mixed-domain queries (e.g., groceries + unrelated questions) to observe whether the assistant stays focused on retail-specific topics or responds off-domain. Screenshots, observations, findings, and recommendations are included.

---

## 📌 Objective

	•	Evaluate the effectiveness of guardrails in a production-grade retail chatbot
	•	Assess intent-routing accuracy using mixed-domain user queries
	•	Analyze system behavior when handling off-topic or general knowledge requests
	•	Derive actionable insights to strengthen domain control and enhance user safety

---

## 🧪 Test Methodology

The chatbot was evaluated using:
	•	Standard grocery and product-related requests
	•	Hybrid queries combining grocery intents with general knowledge
	•	Fully off-domain queries, such as science or political questions

The goal was to measure:
1. **Intent Classification Accuracy**
2. **Domain-Specific Restrictions**
3. **Response Neutrality**
4. **Guardrail Enforcement for Non-Retail Topics**

---

## 🖼️ Screenshots

(Insert screenshots demonstrating chatbot conversations here)

Each screenshot illustrates how the chatbot:
	•	Correctly responded to grocery-related requests
	•	Appropriately handled unrelated or general knowledge queries
	•	Exposed boundary leakage by providing political information

---

## 🔎 Key Findings

- The chatbot handled grocery-related requests correctly and efficiently
- It answered general knowledge questions (e.g., science queries)
- It also responded to political questions, which are typically out of retail domain scope
- This indicates that domain guardrails can be strengthened to avoid off-topic drift

---

## ⚠️ Why This Matters

Retail chatbots are expected to:
	•	Operate strictly within the defined business domain
	•	Refrain from generating sensitive or political content
	•	Ensure neutrality, safety, and regulatory compliance

Weak intent routing can lead to:
- Incorrect domain behavior
- Regulatory risks
- Brand or CX inconsistencies

This evaluation highlights the importance of AI safety and domain restrictions in customer-facing environments.

---

## 🛠️ Recommendations

To improve guardrail performance:

- Add **topic classifiers** to detect whether user input is retail-related
- Reject or redirect **political, sensitive, or irrelevant topics**
- Use **intent filters** to constrain the chatbot to grocery-related tasks
- Add fallback messages such as:

> “I’m here to help with store and product inquiries only.”

- Implement **policy-based guardrails** for sensitive topics
- Strengthen **LLM prompting** with domain and role constraints

---

## 🧩 Future Work

- Quantitative scoring for intent classification accuracy
- Automated testing with multiple random user prompts
- Comparison of retail chatbots from multiple brands
- Development of a guardrail testing framework

---

## 🔐 Disclaimer

This project is a **user-initiated evaluation of a publicly accessible chatbot**.  
No hacking, reverse engineering, intrusive access, or malicious activity was performed.  

All testing was done through standard user interactions for **academic and research purposes only**.

This study does **not claim security vulnerabilities**, and it does not criticize any brand.  
The purpose is to understand AI guardrail behavior and improve safety best practices.

---

## 👤 Author

Developed and documented for research, AI safety evaluation, and portfolio demonstration.

---

