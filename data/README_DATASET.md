 Golden Dataset Schema (JSONL)

 golden_dataset.jsonl rows must include:
 - query_id: string
 - job_story: one of [JS1, JS2, JS3, JS4, JS5]
 - query: user query string
 - ground_truth_answer: concise canonical answer
 - acceptable_variants: list of strings/regex for acceptable matches
 - ground_truth_citations: list of {doc_id, section?, page?, chunk_ids?}
 - difficulty: one of [easy, medium, hard]
 - notes: optional text

 docs_metadata.jsonl rows include:
 - doc_id, title, source_type, uri, pages, ingested_at

 Notes:
 - Keep doc_id stable for provenance.
 - Prefer section and page for citation fidelity.

