# A Survey of Reasoning and Agentic Systems in Time Series with Large Language Models

Time series reasoning treats time as a first-class axis and integrates intermediate evidence into the answer itself.  
This survey organizes the field along two levels:

* **Reasoning Topology** — execution structures:  
  * Direct reasoning (single step)  
  * Linear chain reasoning (sequential intermediate steps)  
  * Branch-structured reasoning (exploration, feedback, and aggregation)  

* **Primary Objective** — the main intent:  
  * Traditional time series analysis (forecasting, classification, anomaly detection, segmentation)  
  * Explanation and understanding (temporal QA, diagnostics, structure discovery)  
  * Causal inference and decision making (counterfactuals, policy evaluation, decision support)  
  * Time series generation (simulation, editing, synthesis)  

We complement this two-level taxonomy with **attribute tags** that capture control-flow operators (decomposition, verification, ensembling), execution actors (tool use, agents), information sources (knowledge access, multimodality), and alignment regimes (prompting, supervised finetuning, reinforcement/preference, hybrid).

This repository curates and classifies papers in the field.  
The following table presents the unified taxonomy and tags for all papers we review.

---

## Curated Papers

| Venue | Link | Paper | Reasoning Topology | Primary Objective | Primary Objective Subcategory | T-Dec | T-Ver | T-Ens | T-Tool | T-Know | T-Multi | T-Agent | T-Align |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| ...... | ...... | ............................................................................................ | ...... | ...... | ...... | ...... | ...... | ...... | ...... | ...... | ...... | ...... | ...... |
| NeurIPS   2023 | https://arxiv.org/abs/2310.07820 | Large Language Models Are Zero-Shot Time Series Forecasters | Direct Reasoning | Traditional Time Series Analysis | Forecasting | FALSE | FALSE | TRUE | FALSE | FALSE | FALSE | 0 | P |
| ICML 2025 | https://arxiv.org/abs/2410.18959 | Context is Key: A Benchmark for Forecasting with Essential   Textual Information | Direct Reasoning | Traditional Time Series Analysis | Forecasting | FALSE | FALSE | FALSE | FALSE | FALSE | TRUE | 0 | P |
| arXiv 2025 | https://arxiv.org/abs/2508.04239 | DP-GPT4MTS: Dual-Prompt Large Language Model for   Textual-Numerical Time Series Forecasting | Direct Reasoning | Traditional Time Series Analysis | Forecasting | FALSE | FALSE | FALSE | FALSE | FALSE | TRUE | 0 | S |
| ICLR 2024 | https://arxiv.org/abs/2310.04948 | TEMPO: Prompt-based Generative Pre-trained Transformer for   Time Series Forecasting | Direct Reasoning | Traditional Time Series Analysis | Forecasting | TRUE | FALSE | FALSE | FALSE | FALSE | TRUE | 0 | S |
| arXiv 2024 | https://arxiv.org/abs/2412.04806 | Rethinking Time Series Forecasting with LLMs via Nearest   Neighbor Contrastive Learning | Direct Reasoning | Traditional Time Series Analysis | Forecasting | FALSE | FALSE | FALSE | FALSE | FALSE | FALSE | 0 | S |





---

## How to Contribute

We welcome contributions to keep this table updated:

1. Add missing papers as new rows following the same format.  
2. Ensure each paper is annotated with exactly one **Reasoning Topology** and one **Primary Objective**, plus appropriate tags.  
3. Submit a pull request.

---

## Citation

If you find this resource useful, please cite our survey (bibtex entry forthcoming).
