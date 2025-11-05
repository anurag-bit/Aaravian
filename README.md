 # Finance/Compliance LLM Benchmark PoC

 This repository benchmarks four strategies (Classic RAG, Agentic, Agentic RAG, Graph RAG) on a Golden Dataset for finance/compliance use cases.

## Quickstart (Conda recommended)
Using Conda ensures compatible wheels (Python 3.11):

```bash
conda env create -f environment.yml
conda activate aaravian-llm-benchmark
python -m ipykernel install --user --name aaravian-llm-benchmark --display-name "aaravian-llm-benchmark"
```

Then open `notebooks/benchmark_llm_pipelines.ipynb` and select the `aaravian-llm-benchmark` kernel.

Alternatively (pip, may require system build tools on Python 3.13):

```bash
pip install -r requirements.txt
```

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
 - If using Neo4j locally, export `NEO4J_PASSWORD` and ensure the DB is running. Qdrant should run at `127.0.0.1:6333` (or update config).

