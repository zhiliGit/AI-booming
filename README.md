# AI-booming

## AI Skills Engineers Should Master in the AI Era (Sorted by Difficulty)

| Difficulty | Skill Area | What to Learn | Terminology Explanation | Typical Enterprise Use Cases |
|---|---|---|---|---|
| ⭐ | AI Coding Tools | Cursor, Copilot, Claude Code, AI Debugging | **Copilot**: AI coding assistant; **Cursor**: AI-integrated IDE; **AI Debugging**: Using AI to analyze and fix code issues | Daily development acceleration, code completion, automated testing |
| ⭐ | Prompt Engineering | Prompt design, structured output, multi-turn dialogue | **Prompt**: Input instruction given to a model; **Structured Output**: Returning outputs in fixed formats like JSON | Chatbots, customer service, content generation |
| ⭐⭐ | LLM API Development | OpenAI API, Function Calling, Streaming | **LLM**: Large Language Model; **Function Calling**: Allowing models to invoke external functions/APIs; **Streaming**: Incremental output generation | AI assistants, enterprise Q&A systems |
| ⭐⭐ | RAG | Embedding, vector databases, retrieval | **RAG (Retrieval-Augmented Generation)**: Combining retrieval with generation; **Embedding**: Converting text into vectors; **Vector Database**: Semantic search storage system | Enterprise knowledge bases, document search |
| ⭐⭐⭐ | Agent Development | ReAct, Tool Use, Memory | **Agent**: AI capable of autonomous decision-making and tool usage; **Memory**: Persistent contextual memory; **ReAct**: Reasoning + acting framework | Workflow automation, AI employees |
| ⭐⭐⭐ | MCP | MCP Server, Tool Schema | **MCP (Model Context Protocol)**: Protocol connecting AI with external tools; **Tool Schema**: Tool interface definition | AI integration with Jira, Slack, databases |
| ⭐⭐⭐ | AI Evaluation | Ragas, LangSmith, A/B Testing | **Evaluation**: Measuring AI output quality; **Hallucination**: Fabricated model outputs; **A/B Testing**: Comparing online performance variants | AI product quality assurance |
| ⭐⭐⭐⭐ | AI Infra / Inference Engineering | vLLM, quantization, GPU inference | **vLLM**: High-performance LLM inference framework; **Quantization**: Reducing model precision to lower resource usage; **KV Cache**: Context cache for faster inference | Private deployment, low-cost inference |
| ⭐⭐⭐⭐ | AI Security & Governance | Prompt Injection, data leakage prevention | **Prompt Injection**: Malicious prompts inducing unauthorized behavior; **PII**: Personally Identifiable Information; **Guardrails**: AI safety restriction mechanisms | Finance, healthcare, government AI |
| ⭐⭐⭐⭐⭐ | Multi-Agent Systems | Multi-Agent, Planner, Workflow | **Multi-Agent**: Multiple collaborating AI agents; **Planner**: Task planning module; **Workflow**: Task execution pipeline | Enterprise automation platforms |
| ⭐⭐⭐⭐⭐ | Model Training / Fine-Tuning | Fine-tuning, LoRA, RLHF | **Fine-tuning**: Adapting models for domain-specific tasks; **LoRA**: Low-cost fine-tuning method; **RLHF**: Reinforcement Learning from Human Feedback | Industry-specific models |
| ⭐⭐⭐⭐⭐ | GPU / CUDA Optimization | CUDA, TensorRT, parallel computing | **CUDA**: NVIDIA GPU programming platform; **TensorRT**: Inference optimization engine | Large-scale model deployment |

## Who Is Working on Large Model Stability Today

The industry is gradually shifting from "Training a larger model" toward "Building verifiable, controllable, and auditable AI systems". 

The main participants can be grouped into:
- Foundation model companies
- Academia
- Agent / AI infrastructure companies

---

### 1. Foundation Model Companies
#### [OpenAI](https://openai.com)
Main directions:
- Tool Use
- Reasoning Models
- Verifiers
- Structured Output
- Agent Orchestration
- External Memory

Typical system architecture: LLM + Tool + Verifier + Workflow + Memory

Core idea:
- No longer relying purely on next-token prediction
- Introducing tools, planning, and verification mechanisms
- Improving controllability and stability

Focus areas:
| Area | Description |
|---|---|
| Tool Use | Using external tools for deterministic tasks |
| Structured Output | JSON / function calling |
| Verifier | Result checking and correction |
| Workflow | Agent process orchestration |
| Memory | Long-context consistency |

---

#### [Anthropic](https://www.anthropic.com)
Main directions:
- Constitutional AI
- AI Safety
- Long-horizon Agents
- Self-Critique
- Policy Layers

Core idea: AI Generation → AI Self-Review → AI Correction

Focus areas:
| Technology | Purpose |
|---|---|
| Constitutional AI | Rule-constrained behavior |
| Self-Reflection | Model self-checking |
| Policy Layer | Behavioral boundaries |
| Tool Agent | Tool-enhanced stability |

Characteristics:
- Strong emphasis on behavioral stability
- Focus on controllable AI systems

---

#### [Google DeepMind](https://deepmind.google)
Main directions:
- Neuro-symbolic AI
- Formal Reasoning
- Planning
- World Models
- Theorem Proving

Representative projects:
| Project | Description |
|---|---|
| AlphaGeometry | Geometric reasoning |
| AlphaProof | Mathematical proving |
| Gemini Reasoning | Enhanced reasoning capabilities |

Core idea: Neural Networks + Symbolic Reasoning + Search

DeepMind is currently one of the strongest proponents of Neuro-Symbolic AI among major AI labs.
---

### 2. Academia
Academia is arguably the primary source of "Stable AI" theory

---
#### The Gary Marcus Camp
Representative researchers:
- Gary Marcus
- Vaishak Belle

Core viewpoint:
> Pure deep learning cannot achieve robust reasoning.

Main proposal: Neuro-Symbolic AI

Neural Network + Logic + Program

Focus areas:
| Area | Description |
|---|---|
| Symbolic Reasoning | Logic-based reasoning |
| Logic Constraints | Formal constraints |
| Program Synthesis | Generating executable programs |
| Verifiable AI | Provably reliable AI |
---

#### MIT / Stanford / CMU / Edinburgh and Others
Research directions:
| Area | Description |
|---|---|
| Formal Verification | Mathematical verification |
| Theorem Proving | Automated proving |
| Neuro-symbolic AI | Neural-symbolic integration |
| Agent Verification | Reliable agent systems |
| Trustworthy AI | Reliable and safe AI |

---

### 3. Agent / AI Infrastructure Companies
These companies focus on:
> Turning LLMs into stable systems rather than standalone chat models.
---
#### [LangChain / LangGraph](https://www.langchain.com)
Main directions:
- Workflow orchestration
- State graphs
- Retry mechanisms
- Deterministic orchestration

Core idea: Put the LLM inside a finite-state machine

LangGraph is essentially: Workflow + FSM (Finite State Machine)

Key functions:
| Technology | Purpose |
|---|---|
| State Graph | Stable execution states |
| Retry | Automatic recovery |
| Workflow DAG | Process control |
| Memory | Long-task consistency |

---
#### [Microsoft Semantic Kernel](https://learn.microsoft.com/semantic-kernel/)
Main directions:
- Planning
- Tool Routing
- Enterprise Reliability
- Memory

Microsoft’s approach:LLM + Enterprise System

Characteristics:
- Enterprise-grade reliability
- AI orchestration emphasis

---
#### [Model Context Protocol (MCP)](https://modelcontextprotocol.io)
Core objective: Standardized tool interfaces for agents

Functions:
| Function | Description |
|---|---|
| Tool Interface | Standardized tool protocols |
| Context Injection | Unified context handling |
| External Grounding | External knowledge integration |
| Agent Infrastructure | Agent system foundation |

---

### 4. Major Industry Trend

The industry increasingly recognizes that "LLM ≠ Complete AI System"

As a result, the field is moving from a single large model toward:

Model + Tools + Verifier + Memory + Planner + Workflow + Symbolic Layer

This is often referred to as Compound AI Systems

---

### 5. Current Technical Split

#### Path A: Continue Scaling
Representatives:
- OpenAI (partially)
- Meta
- xAI
- DeepSeek (partially)

Core belief:
> Larger models + more data + more compute
> will naturally yield stable reasoning capabilities.

---

#### Path B: Neuro-Symbolic / System AI
Representatives:
- DeepMind
- Anthropic (partially)
- Many academic researchers

Core belief:
> Pure statistical generation will never be sufficiently stable.

Therefore AI systems must incorporate:
- Logic
- Planning
- Verification
- Symbolic Constraints

---

### 6. Current Leaders by Area
| Area | Leading Organizations |
|---|---|
| Reasoning | OpenAI / DeepMind |
| Constitutional AI | Anthropic |
| Agent Engineering | LangChain / Microsoft |
| Neuro-symbolic AI | DeepMind / Academia |
| Formal Verification | Academia |
| Enterprise Reliable AI | Microsoft |

---
