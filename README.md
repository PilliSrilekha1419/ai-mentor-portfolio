# AI Mentor Bootcamp - Pilli Srilekha
## Day 1 — Setup complete

- ✅ Google AI Studio API key provisioned
- ✅ Groq API key provisioned
- ✅ Hello-Gemini call working — see [Day1_Setup.ipynb](Day1_Setup.ipynb)
- 4-tool comparison matrix from Lab 1A: see screenshot below

- ![Gemini first call](gemini_first_call.png)

- ## Acceptance check

Push to `Day2_SixPatterns.md` in the ai-mentor-portfolio repo:
- ✅ Six prompts, clearly labelled by pattern
- ✅ Best output per pattern
- ✅ Self-score for each (1-5)
- ✅ Peer-score for each (sum of 5 criteria, out of 10)
- ✅ One paragraph at the bottom: "For my placement-prep students, the patterns I will use most are X and Y, because ___."

  
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

## DAY 3 Acceptance check (final 5 min)

For each mentor:
- ✅ 1-page PDF in repo
- ✅ All 8 student-AI scenarios classified with reasoning
- ✅ Permitted Uses section: 5-8 specific sentences
- ✅ Prohibited Uses section: 3-5 rules, each with a detection method
- ✅ Enforcement section: 3 sentences, honest about detection limits

- - ✅ Matrix has all 5 rows × 5 columns filled (claim, AI source, Perplexity check, primary source URL, verdict)
- ✅ At least 1 verdict is PARTIAL, FALSE, or NO PRIMARY SOURCE FOUND
- ✅ Reflection paragraph identifies the weakest-sounding-yet-strongest-looking claim
- ✅ Pushed as `Day3_Verification.md` to ai-mentor-portfolio repo

## DAY 4 Acceptance check (final 5 min, 12:00 sharp)

For each mentor:
- ✅ Brief PDF in repo (≤ 2 pages, with grounded citations)
- ✅ Deck PDF in repo (8 slides, cover + CTA hand-edited)
- ✅ README has 3-line edit-notes (which numbers needed verification)
- ✅ Total time elapsed ≤ 45 min (note overruns; do NOT extend)
## Acceptance check (final 5 min)

For each mentor:
- ✅ n8n container running at localhost:5678
- ✅ Workflow with all 4 nodes wired and ACTIVE
- ✅ Test email received in inbox
- ✅ Workflow JSON exported and pushed to repo
- ✅ Screenshot of test email in repo README
  
## DAY 5
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

## DAY 6 Acceptance check (final 5 min — mandatory before break)

For each pair:
- ✅ Day6_PlacementProcessor.ipynb runs end-to-end
- ✅ data/jds.jsonl in repo with ≥3 valid JDs
- ✅ Engineer Answer in README with all 5 questions answered specifically
- ✅ Pair names credited in README
- ✅ Push verified at github.com (you walk the room and check the green checkmark)

- ## Acceptance check (final 5 min)

For each pair:
- ✅ Notebook runs end-to-end without uncaught errors
- ✅ ≥4 of 5 résumés processed successfully
- ✅ Empty + whitespace inputs handled gracefully
- ✅ README documents the 3 errors handled with technical reasoning
- ✅ Notebook pushed (each pair pushes to ONE pair-member's repo for the lab; afternoon Sprint 1 starts the capstone arc)

- ## DAY 7 Acceptance check (final 5 min — mandatory before break)

For each pair:
- ✅ Day7_RAG_Chatbot.ipynb runs end-to-end
- ✅ ChromaDB collection has ≥50 documents
- ✅ 5 cited Q&A pairs in README (≥1 is "I do not know")
- ✅ Engineer Answer with all 5 questions answered specifically
- ✅ Notebook + chroma_db/ folder pushed to repo

## DAY 8 Acceptance check (final 5 min)

For each mentor:
- ✅ 20-question testset loaded
- ✅ RAGAS metrics computed (3 numbers, real values)
- ✅ Baseline table + interpretation in README
- ✅ Ship-or-not decision stated
- ✅ baseline.jsonl saved + pushed


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

4. ## Acceptance check (final 5 min — mandatory before break)

For each pair:
- ✅ MCP server starts and responds to MCP inspector tests
- ✅ Server registered in Claude Desktop config + visible in Claude Desktop UI
- ✅ Test call from Claude Desktop returns valid JD JSON
- ✅ Capstone main loop uses Gemini → Groq → Ollama fallback
- ✅ Loom recording of Wi-Fi disconnect with full capstone working
- ✅ Pushed to repo (mcp_server.py + src/llm_fallback.py + Loom URL)
