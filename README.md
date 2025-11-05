 # Finance/Compliance LLM Benchmark PoC

 This repository benchmarks four strategies (Classic RAG, Agentic, Agentic RAG, Graph RAG) on a Golden Dataset for finance/compliance use cases.

 ## Quickstart
 1. Python 3.11+ recommended
 2. `pip install -r requirements.txt`
 3. Set API keys as env vars (e.g., `OPENAI_API_KEY`, `COHERE_API_KEY`, `NEO4J_PASSWORD`)
 4. Open `notebooks/benchmark_llm_pipelines.ipynb` and run all cells

 ## Config
 - `configs/config.yaml` controls models, retrieval, agent, graph, pricing snapshot, artifacts

 ## Data
 - Golden dataset schema in `data/README_DATASET.md`
 - Place your JSONL files at paths in `configs/config.yaml`

 ## Outputs
 - `results/results.parquet`, `results/report-ready.csv`
 - Plots under `plots/`
 - Traces under `traces/`

 ## Notes
 - Stubs for pipelines and judge are provided; replace with LlamaIndex pipelines and RAGAS/LLM-judge for real runs.

