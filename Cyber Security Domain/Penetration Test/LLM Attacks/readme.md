## 🤖 Generative AI Attacks

**🎮 Interactive Practice**  
Try your hand at real-world prompt injection with [Gandalf AI](https://gandalf.lakera.ai/) — a free browser-based game that simulates attacking a large language model using crafted prompts.

---

### 🧠 Introduction to Generative AI and LLMs
- What is Generative AI?
- Examples: GPT, Claude, Gemini, DALL·E, Midjourney
- Large Language Models (LLMs) and foundation models
- Difference between training, fine-tuning, and inference
- Typical use cases: chatbots, assistants, code generation, content creation

### 🚨 Threat Landscape
- Trust boundaries in human-AI interaction
- Attack surfaces:
  - Prompt input field
  - API endpoints
  - Model training pipeline
  - Plugins and tools (agents)
- Public vs private models (open weights vs SaaS)

### 📥 Prompt Injection Attacks
- Direct prompt injection
- Indirect prompt injection (via data sources, websites, files)
- Encoding and escaping techniques
- Bypassing safety filters / jailbreaks
- Examples of prompt injection in chatbots and copilots

### 🧬 Training Data Poisoning
- Poisoning public datasets (GitHub, Stack Overflow, Wikipedia)
- Model skewing by injecting biased or malicious examples
- Detection difficulty and long-term risk

### 🔓 Model Output Manipulation
- Data leakage from models (training data inference)
- Model hallucinations used maliciously
- Induced misinformation campaigns
- Evasion of guardrails and alignment controls

### 🧑‍💻 Code Generation Vulnerabilities
- Insecure code generation by LLMs (e.g., SQL injection, path traversal)
- Overtrust by developers (copy/paste risk)
- Lack of contextual security validation
- Dependency confusion and package suggestion poisoning

### 📡 Abuse of AI for Recon and Payload Generation
- Using LLMs for crafting payloads (phishing, malware evasion, obfuscated code)
- Natural language recon (e.g., domain-specific information gathering)
- Social engineering automation via personas

### ⚙️ Model Abuse in Real-World Systems
- LLM-integrated APIs abused via crafted inputs
- Business logic manipulation
- Abuse of autonomous agents and AI decision-making pipelines

### 🛡️ Defensive Measures
- Prompt validation and contextual isolation
- Rate limiting and prompt memory control
- Fine-tuned moderation layers
- Red teaming AI systems (e.g., Anthropic’s RHP, OpenAI’s alignment evals)
- LLM firewalls and pre-processing wrappers

### 📚 Frameworks and Guidelines
- [OWASP Top 10 for LLM Applications (2023)](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [NIST AI Risk Management Framework (RMF)](https://www.nist.gov/itl/ai-risk-management-framework)
- [Microsoft Responsible AI Standard](https://www.microsoft.com/en-us/ai/responsible-ai)
- [Anthropic’s Red Teaming Playbook (RHP)](https://www.anthropic.com/index/2023/10/red-teaming)
- [OpenAI System Card & Safety Research](https://openai.com/research)

### 🧪 Labs and Tools
- [LLM-RedTeaming](https://github.com/llm-redteaming/llm-redteaming)
- [Atheris](https://github.com/google/atheris) – Python fuzzing engine
- [Gaia LLM Security Framework](https://github.com/gaia-ai/gaia)
- [LangChainGuard](https://github.com/langchain-ai/langchainguard)
- [PromptBench](https://github.com/PromptBench/promptbench)
- GPT4 jailbreak tracker repositories
- Adversarial testing platforms for generative models