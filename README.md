# AI Mentor Bootcamp - Pilli Srilekha
## Day 1 — Setup complete

- ✅ Google AI Studio API key provisioned
- ✅ Groq API key provisioned
- ✅ Hello-Gemini call working — see [Day1_Setup.ipynb](Day1_Setup.ipynb)
- 4-tool comparison matrix from Lab 1A: see screenshot below

- ![Gemini first call](gemini_first_call.png)
  
## Day 2 Lab 2B — Errors handled

1. Markdown fence wrapping
   Retry prompt forces raw JSON output.

2. Missing phone number
   Optional[str] = None allows validation.

3. Empty input
   Empty strings are caught before Gemini API call.

## Reflection

Semantic search returns the nearest semantic match,
not necessarily the correct factual answer.

Embeddings group related topics together in vector space.
PCA visualization helped show semantic clustering.


Built React dashboards for 3 startups              -> frontend dev (0.88)
Implemented Spring Boot microservices in Java for  -> backend dev (0.63)
Trained CNN for image classification using PyTorch -> ML engineer (0.40)
Cleaned 100k row dataset using pandas + plotted in -> data analyst (0.54)
Wrote SQL queries against PostgreSQL               -> data analyst (0.48)

Sentiment scores:
[POSITIVE 1.00] I really enjoyed working on the team and shipped 3 features.
[NEGATIVE 1.00] I was the only one writing code; everyone else was slow.
[POSITIVE 1.00] I learned a lot from my mentor and grew technically.
[NEGATIVE 1.00] I had to redo most of my teammate's work because it was wron
[POSITIVE 1.00] My internship was great — would recommend it to anyone.


API:   min A0.8s | avg 1.2s
Local: min 0.68s | avg 0.71s


## Day 9 Lab 9A — Hello-LangGraph

- 1-tool ReAct agent with DuckDuckGo web_search
- 4-message trace printed successfully
- Failure-case testing completed successfully

### Reflection

1. The trace explains the reasoning process.
2. Tool docstrings guide tool selection.
3. Agents need explicit failure handling.

## Day 9 — Capstone Sprint 4: Career Agent

- Multi-tool LangGraph ReAct agent
- 3 tools integrated:
  - jd_fetcher
  - skills_gap
  - answer_scorer
- Failure recovery tested successfully

### Reflection
1. Agents choose tools dynamically.
2. Tool docstrings guide reasoning.
3. Explicit ERROR handling prevents hallucination.

## Day 10 Lab 10A — Hello-CrewAI

### Goal

Built a 2-agent CrewAI system that generates a 1-page TCS Digital placement preparation brief.

### Agents

1. Placement Researcher
2. Placement Brief Writer

### Workflow

Researcher → Writer → Final Markdown Brief

### Files Generated

* day10_lab10a_transcript.txt
* tcs_digital_brief.md

### Reflection

1. The handoff between agents is the design quality.
2. expected_output acts as the contract between agents.
3. Verbose mode helps debug multi-agent workflows.

## Day 11 Lab 11A — Ollama Offline + Hybrid Fallback

### Completed
- ✅ Ollama installed locally
- ✅ llama3.2 model downloaded
- ✅ Offline AI tested after Wi-Fi disconnect
- ✅ Gemini → Groq → Ollama fallback chain implemented
- ✅ Force-failure testing completed
- ✅ Local fallback verified

### Demo Proof
- Wi-Fi disconnect demo recorded
- Fallback chain outputs captured

### Reflection
1. First inference is slow because the model loads into RAM.
2. Ollama is useful for privacy, offline access, and zero per-call cost.
3. Production AI systems should not depend on a single provider.
