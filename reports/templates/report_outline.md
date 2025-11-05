 # Executive Report Outline

 ## 1. Executive Summary
 - Winner(s) and rationale in 3 bullets
 - Key trade-offs (quality, latency, cost)
 - Final recommendation (single or hybrid)

 ## 2. Problem & Users
 - Target teams and workflows
 - Why unstructured data is hard in finance/compliance

 ## 3. Methodology
 - Dataset composition and jobs-to-be-done
 - Metrics and controls (judge model, seeds)
 - Reproducibility and pricing snapshot

 ## 4. Systems Under Test
 - Classic RAG, Agentic, Agentic RAG, Graph RAG diagrams
 - Fixed knobs for fairness

 ## 5. Quantitative Results
 - Bar: Average Faithfulness by Strategy
 - Bar: Answer Relevancy by Strategy
 - Bar: Citation Correctness by Strategy
 - Heatmap: Context Precision vs Recall (Strategy x Job Story)
 - Box: End-to-End Latency by Strategy (p50/p90/p95)
 - Violin: First-token Latency by Strategy
 - Scatter: Cost vs Answer Relevancy (Pareto)
 - Waterfall: Cost breakdown per Strategy
 - Line: Throughput vs p95 Latency under load
 - Bar: Ingestion Time and Cost per 100 docs

 ## 6. Robustness & Safety
 - Variance across runs, refusal rates, canary outcomes

 ## 7. Qualitative Gallery (Smoking Guns)
 - 10–12 curated win/loss cases with evidence and judge notes

 ## 8. Trade-Off Matrix & Recommendation
 - Matrix: Strategies vs JS1–JS5 and constraints
 - Final recommendation with operating thresholds for switching

 ## 9. Implementation Roadmap
 - Next steps, risks, budget, platform choice, MVE→MLP

