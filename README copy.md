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

<div style="overflow-x: auto; width:100%;">
<table style="width:100%" border="2" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
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
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[Large Language Models Are Zero-Shot Time Series Forecasters](https://arxiv.org/abs/2205.13504)</td>
      <td>Direct Reasoning</td>
      <td>Traditional Time Series Analysis</td>
      <td>Forecasting</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">TRUE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">0</td>
      <td align="center">P</td>
    </tr>
    <tr>
      <td>[Context is Key: A Benchmark for Forecasting with Essential Textual Information](https://arxiv.org/abs/2302.02041)</td>
      <td>Direct Reasoning</td>
      <td>Traditional Time Series Analysis</td>
      <td>Forecasting</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">TRUE</td>
      <td align="center">0</td>
      <td align="center">P</td>
    </tr>
    <tr>
      <td>[DP-GPT4MTS: Dual-Prompt Large Language Model for Textual-Numerical Time Series Forecasting](https://arxiv.org/abs/2310.19771)</td>
      <td>Direct Reasoning</td>
      <td>Traditional Time Series Analysis</td>
      <td>Forecasting</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">TRUE</td>
      <td align="center">0</td>
      <td align="center">S</td>
    </tr>
    <tr>
      <td>[TEMPO: Prompt-Based Generative Pre-Trained Transformer for Time Series Forecasting](https://arxiv.org/abs/2306.03009)</td>
      <td>Direct Reasoning</td>
      <td>Traditional Time Series Analysis</td>
      <td>Forecasting</td>
      <td align="center">TRUE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">FALSE</td>
      <td align="center">TRUE</td>
      <td align="center">0</td>
      <td align="center">S</td>
    </tr>
  </tbody>
</table>
</div>







---

## How to Contribute

We welcome contributions to keep this table updated:

1. Add missing papers as new rows following the same format.  
2. Ensure each paper is annotated with exactly one **Reasoning Topology** and one **Primary Objective**, plus appropriate tags.  
3. Submit a pull request.

---

## Citation

If you find this resource useful, please cite our survey (bibtex entry forthcoming).
