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

<table><thead>
  <tr>
    <th>Venue</th>
    <th>Link</th>
    <th>Paper</th>
    <th>Reasoning Topology</th>
    <th>Primary Objective</th>
    <th>Primary Objective Subcategory</th>
    <th>T-Dec</th>
    <th>T-Ver</th>
    <th>T-Ens</th>
    <th>T-Tool</th>
    <th>T-Know</th>
    <th>T-Multi</th>
    <th>T-Agent</th>
    <th>T-Align</th>
  </tr></thead>
<tbody>
  <tr>
    <td>•••••••••••••••</td>
    <td>•••</td>
    <td>............................................................................................................</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
    <td>......</td>
  </tr>
  <tr>
    <td>NeurIPS 2023</td>
    <td><a href="https://arxiv.org/abs/2310.07820">https://arxiv.org/abs/2310.07820</a></td>
    <td>Large Language Models Are Zero-Shot Time Series Forecasters</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>0</td>
    <td>P</td>
  </tr>
  <tr>
    <td>ICML 2025</td>
    <td><a href="https://arxiv.org/abs/2410.18959">https://arxiv.org/abs/2410.18959</a></td>
    <td>Context is Key: A Benchmark for Forecasting with Essential Textual Information</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>0</td>
    <td>P</td>
  </tr>
  <tr>
    <td>arXiv 2025</td>
    <td><a href="https://arxiv.org/abs/2508.04239">https://arxiv.org/abs/2508.04239</a></td>
    <td>DP-GPT4MTS: Dual-Prompt Large Language Model for Textual-Numerical Time Series Forecasting</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>0</td>
    <td>S</td>
  </tr>
  <tr>
    <td>ICLR 2024</td>
    <td><a href="https://arxiv.org/abs/2310.04948">https://arxiv.org/abs/2310.04948</a></td>
    <td>TEMPO: Prompt-based Generative Pre-trained Transformer for Time Series Forecasting</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>TRUE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>0</td>
    <td>S</td>
  </tr>
  <tr>
    <td>arXiv 2024</td>
    <td><a href="https://arxiv.org/abs/2412.04806">https://arxiv.org/abs/2412.04806</a></td>
    <td>Rethinking Time Series Forecasting with LLMs via Nearest Neighbor Contrastive Learning</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>0</td>
    <td>S</td>
  </tr>
</tbody></table>






---

## How to Contribute

We welcome contributions to keep this table updated:

1. Add missing papers as new rows following the same format.  
2. Ensure each paper is annotated with exactly one **Reasoning Topology** and one **Primary Objective**, plus appropriate tags.  
3. Submit a pull request.

---

## Citation

If you find this resource useful, please cite our survey (bibtex entry forthcoming).
