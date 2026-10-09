# Hi, I'm Ravi

I'm a Lead Data Scientist at [Thoughtworks](https://www.thoughtworks.com) in Singapore. I build LLM agent systems and retrieval-augmented generation (RAG) applications for public sector clients, and the evaluation and monitoring that sits around them: checks for goal drift, hallucination, and drops in output quality once a system is running in production.

Before Thoughtworks I spent six years at Grab, first on high-throughput Go services for food and express deliveries and later on LLM systems for multilingual content. Before that I worked on trade rules violation detection engine & trade data pipelines at Morgan Stanley as a Backend and Data Engineer.

I hold an M.S. in Computer Science (Machine Learning) from Georgia Tech, where I also worked as a research assistant on graph neural networks and reinforcement learning for Boolean circuit analysis.

## What I'm working on

- **Long-horizon agents.** How to keep an agent on task during multi-hour unsupervised runs. Periodic goal re-reads, checkpointed progress, sub-agents that start with a fresh context, and judges that review the work without inheriting the agent's history.
- **RAG evaluation.** Growing an eval suite alongside the retrieval stack as it moves from BM25 to dense embeddings, then to hybrid search with rank fusion, and finally to cross-encoder reranking with context window tuning.
- **Multi-agent workflows** for triaging and resolving support tickets (DSPy), and guardrailed content generation with Guardrails AI.

## Research interests

- Fine-tuning LLMs, especially parameter-efficient methods such as LoRA
- Retrieval, ranking, and evaluation for RAG systems
- Representation geometry and mechanistic interpretability
- Graph neural networks and reinforcement learning

At Georgia Tech (2025) I studied whether properties of a Boolean function can be learned directly from its circuit encoding. Given a circuit, usually in CNF form, the model predicts the influence distribution over its inputs and its Hamming weight (bias). I used GNN-RE as the baseline and explored combining it with LLM and RL components to improve accuracy. The work used Python, PyTorch, and Hugging Face Transformers.

## Talks

- **Agents That Don't Lose the Plot.** Thoughtworks XConf APAC 2026, Ho Chi Minh City. Failure modes of long-running agents seen across three industry case studies, and ten practical fixes for keeping them on track.
- **Ship Reliable RAG: Evals That Grow with Your Retrieval Complexity.** PyCon Australia 2026, Brisbane. A level-by-level walk through building a RAG app and its eval suite together, using an AI-assisted IT support ticket system as the running example. Covers RAGAS metrics and compares rank fusion methods (RRF, weighted RRF, Z-score, and min-max).

Slides and recordings go up on [ravivats.github.io/talks](https://ravivats.github.io/talks/).

## Selected work

**Thoughtworks**, Lead Data Scientist (2025 to present)
- Designed and implemented a unified natural language search across every searchable entity type in an organisation. It uses hybrid retrieval that combines lexical keyword matching, fuzzy matching for typos and partial terms, and embedding-based semantic search.
- Multi-agent LLM systems that debug and resolve issue tickets raised by members of the public.
- Agentic content generation constrained by domain guardrails, with evaluation workflows that monitor agent output over time.

**Grab**, Senior Software Engineer (AI) and Software Engineer (2019 to 2025)
- Led the implementation of an agentic translation system built as a translator and critic loop on LangGraph. It writes emails, notifications, and promotional content in Grab's brand voice across English, Mandarin, and eight Southeast Asian languages, and served more than one million users a day.
- Fine-tuned Llama 3.1 8B with LoRA on promo text written by the firm's content team, then added few-shot retrieval over a FAISS index so the model could draw on content written after training.
- Built an LLM-assisted flow that suggests replacement items when part of an order is unavailable, using RAG over merchant's current available items.
- Designed a generic min/max TTL Redis cache in Go that keeps serving recent data while an upstream service recovers from errors. It was piloted on the GrabFood, Mart, and Express gateway.
- Built chaos engineering jobs that cut connections to Redis, DynamoDB, and config services in staging to test fallback paths.
- Applied ARIMA-based anomaly detection to AWS spend, then right-sized resources to cut infrastructure costs by 30% across seven services.
- Worked on the gRPC and REST services that manage food and express delivery orders from creation to completion, at a scale of millions of orders a day.
- Received the Generative AI Sprint Award during Grab's global GenAI sprint (2024).

**Morgan Stanley**, Technology Associate (2018 to 2019)
- Spark and Scala pipelines that applied data quality rules to roughly 500 million trade records a day for post-trade reporting. Received the division's Rookie Award.

## Toolbox

| Area | Tools |
| --- | --- |
| Languages | Python, Go, Java, Scala, C++ |
| ML and LLMs | PyTorch, Hugging Face Transformers, LangGraph, LangChain, LangSmith, DSPy, RAGAS, FAISS, Guardrails AI |
| Data and systems | gRPC, Protobuf, Kafka, Flink, Spark, Redis, Terraform |
| Cloud | AWS (Certified Solutions Architect, Associate), Azure (Data Scientist Associate, Fundamentals) |

## Writing

I write about problems I'm working through on [ravivats.github.io](https://ravivats.github.io). Older posts include the *HeadStart ML* series on ML fundamentals and statistics interview prep, and the *HeadStart System Design* series on design patterns and AWS architecture.

## Older projects

Some things from my student days that are still pinned here:

- [ds-algo-interview-cookbook](https://github.com/ravivats/ds-algo-interview-cookbook): data structure and algorithm implementations with interview solutions
- [Sentimental-Review-Analysis](https://github.com/ravivats/Sentimental-Review-Analysis): sentiment analysis of reviews using named entity identification
- [Air-Pollution-Analysis-BLR](https://github.com/ravivats/Air-Pollution-Analysis-BLR): air pollution analysis and prediction for Bangalore
- [pexeso-pygame](https://github.com/ravivats/pexeso-pygame): the Czech memory card game Pexeso, in Pygame

## Get in touch

[Website](https://ravivats.github.io) · [LinkedIn](https://www.linkedin.com/in/ravi-vats/) · [X](https://x.com/ravivats_) · [Email](mailto:mailravivats@gmail.com)
