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

## Table of Contents

- [Direct Reasoning](#research-papers-for-direct-reasoning)
- [Linear Chain Reasoning](#research-papers-for-linear-chain-reasoning)
- [Branch-Structured Reasoning](#research-papers-for-branch-structured-reasoning)
- [Non-Research Papers](#non-research-papers)

## Research Papers for Direct Reasoning

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Paper&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Primary Objective | Task | T-Dec | T-Ver | T-Ens | T-Tool | T-Know | T-Multi | T-Agent | T-Align |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Large Language Models Are Zero-Shot Time Series Forecasters](https://openreview.net/forum?id=md68e8iZK1) [NeurIPS 2023] | Trad. TS Anal. | Forc. |  |  | ✔ |  |  |  | 0 | P |
| [Context is Key: A Benchmark for Forecasting with Essential   Textual Information](https://arxiv.org/abs/2410.18959) [ICML 2025] | Trad. TS Anal. | Forc. |  |  |  |  |  | ✔ | 0 | P |
| [DP-GPT4MTS: Dual-Prompt Large Language Model for   Textual-Numerical Time Series Forecasting](https://arxiv.org/abs/2508.04239) [arXiv 2025] | Trad. TS Anal. | Forc. |  |  |  |  |  | ✔ | 0 | S |
| [TEMPO: Prompt-based Generative Pre-trained Transformer for   Time Series Forecasting](https://openreview.net/forum?id=YH5w12OUuU) [ICLR 2024] | Trad. TS Anal. | Forc. | ✔ |  |  |  |  | ✔ | 0 | S |
| [Rethinking Time Series Forecasting with LLMs via Nearest   Neighbor Contrastive Learning](https://arxiv.org/abs/2412.04806) [arXiv 2024] | Trad. TS Anal. | Forc. |  |  |  |  |  |  | 0 | S |
| [CMLLM: A Novel Cross-Modal Large Language Model for Wind Power   Forecasting](https://www.sciencedirect.com/science/article/pii/S0196890425001967) [Energy Conversion and   Management 2025] | Trad. TS Anal. | Forc. |  |  |  |  |  |  | 0 | P |
| [Multi-Modal Forecaster: Jointly Predicting Time Series and   Textual Data](https://arxiv.org/abs/2411.06735) [arXiv 2024] | Trad. TS Anal. | Forc. |  |  |  |  |  | ✔ | 0 | S |
| [Time Series Forecasting with LLMs: Understanding and Enhancing   Model Capabilities](https://dl.acm.org/doi/10.1145/3715073.3715083) [SIGKDD Explor. Newsl. 2025] | Trad. TS Anal. | Forc. |  |  |  |  |  |  | 0 | P |
| [Hierarchical Multimodal LLMs with Semantic Space Alignment for   Enhanced Time Series Classification](https://arxiv.org/abs/2410.18686) [arXiv 2024] | Trad. TS Anal. | Class. |  |  |  |  |  | ✔ | 0 | S |
| [Multimodal LLMs for Health Grounded in Individual-Specific   Data](https://doi.org/10.1007/978-3-031-47679-2_7) [Machine Learning for   Multimodal Healthcare Data 2023] | Trad. TS Anal. | Class. |  |  |  |  |  | ✔ | 0 | S |
| [Retrieval-augmented Large Language Models for Financial Time   Series Forecasting](https://arxiv.org/abs/2502.05878) [arXiv 2025] | Trad. TS Anal. | Class. |  |  |  | ✔ | ✔ |  | 0 | S |
| [Can LLMs Understand Time Series Anomalies?](https://openreview.net/forum?id=LGafQ1g2D2) [ICLR 2025] | Trad. TS Anal. | Anom. Det. | ✔ |  |  |  |  | ✔ | 0 | P |
| [MedTsLLM: Leveraging LLMs for Multimodal Medical Time Series   Analysis](https://arxiv.org/abs/2408.07773) [arXiv 2024] | Trad. TS Anal. | Segm. |  |  |  |  |  | ✔ | 0 | P |
| [ChatTime: A Unified Multimodal Time Series Foundation Model   Bridging Numerical and Textual Data](https://doi.org/10.1609/aaai.v39i12.33384) [AAAI 2025] | Trad. TS Anal. | Mult. Tasks |  |  |  |  |  | ✔ | 0 | S |
| [Chat-TS: Enhancing Multi-Modal Reasoning Over Time-Series and   Natural Language Data](https://arxiv.org/abs/2503.10883) [arXiv 2025] | Expl. & Und. | Temp. QA |  |  |  |  |  | ✔ | 0 | S |
| [ChatTS: Aligning Time Series with LLMs via Synthetic Data for   Enhanced Understanding and Reasoning](https://arxiv.org/abs/2412.03104) [VLDB 2025] | Expl. & Und. | Temp. QA |  |  |  |  |  | ✔ | 0 | S |
| [ITFormer: Bridging Time Series and Natural Language for   Multi-Modal QA with Large-Scale Multitask Dataset](https://openreview.net/forum?id=GByP03IitA) [ICML 2025] | Expl. & Und. | Temp. QA |  |  |  |  |  | ✔ | 0 | P |
| [Time-MQA: Time Series Multi-Task Question Answering with   Context Enhancement](https://aclanthology.org/2025.acl-long.1437/) [ACL 2025] | Expl. & Und. | Temp. QA |  |  |  |  |  | ✔ | 0 | S |
| [GEM: Empowering MLLM for Grounded ECG Understanding with Time   Series and Images](https://arxiv.org/abs/2503.06073) [arXiv 2025] | Expl. & Und. | Expl. Diagn. |  |  |  |  |  | ✔ | 0 | S |
| [Time-RA: Towards Time Series Reasoning for Anomaly with LLM   Feedback](https://arxiv.org/abs/2507.15066) [arXiv 2025] | Expl. & Und. | Expl. Diagn. | ✔ | ✔ | ✔ |  |  | ✔ | 0 | S |
| [Momentor: Advancing Video Large Language Model with   Fine-Grained Temporal Reasoning](https://arxiv.org/abs/2402.11435) [ICML 2024] | Expl. & Und. | Expl. Diagn. |  |  |  |  |  | ✔ | 0 | P |
| [RealTCD: Temporal Causal Discovery from Interventional Data   with Large Language Model](https://doi.org/10.1145/3627673.3680042) [CIKM 2024] | Expl. & Und. | Struct. Disc. |  |  |  |  |  |  | 0 | P |
| [GG-LLM: Geometrically Grounding Large Language Models for   Zero-shot Human Activity Forecasting in Human-Aware Task Planning](https://doi.org/10.1109/ICRA57147.2024.10611090) [ICRA 2024] | Causal Inf. | Auto. Policy |  |  |  |  |  |  | 0 | P |

## Research Papers for Linear Chain Reasoning

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Paper&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Primary Objective | Task | T-Dec | T-Ver | T-Ens | T-Tool | T-Know | T-Multi | T-Agent | T-Align |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Can Slow-thinking LLMs Reason Over Time? Empirical Studies in   Time Series Forecasting](https://arxiv.org/abs/2505.24511) [arXiv 2025] | Trad. TS Anal. | Forc. | ✔ | ✔ |  |  |  | ✔ | 0 | P |
| [Retrieval Augmented Time Series Forecasting](https://arxiv.org/abs/2411.08249) [arXiv 2024] | Trad. TS Anal. | Forc. |  |  |  | ✔ | ✔ |  | 0 | S |
| [TimeRAG: Boosting LLM Time Series Forecasting via   Retrieval-Augmented Generation](https://arxiv.org/abs/2412.16643) [arXiv 2024] | Trad. TS Anal. | Forc. |  |  |  | ✔ | ✔ |  | 0 | P |
| [Time Series Forecasting as Reasoning: A Slow-Thinking Approach   with Reinforced LLMs](https://arxiv.org/abs/2506.10630) [arXiv 2025] | Trad. TS Anal. | Forc. | ✔ |  |  |  |  |  | 0 | H |
| [Temporal Data Meets LLM - Explainable Financial Time Series   Forecasting](https://arxiv.org/abs/2306.11025) [arXiv 2023] | Trad. TS Anal. | Forc. | ✔ |  |  | ✔ | ✔ | ✔ | 0 | S |
| [TableTime: Reformulating Time Series Classification as   Training-Free Table Understanding with Large Language Models](https://arxiv.org/abs/2411.15737) [arXiv 2024] | Trad. TS Anal. | Class. | ✔ |  | ✔ | ✔ |  |  | 0 | P |
| [A Picture is Worth A Thousand Numbers: Enabling LLMs Reason   about Time Series via Visualization](https://aclanthology.org/2025.naacl-long.383/) [NAACL 2025] | Trad. TS Anal. | Class. | ✔ |  |  |  |  | ✔ | 0 | P |
| [ZARA: Zero-shot Motion Time-Series Analysis via Knowledge and   Retrieval Driven LLM Agents](https://arxiv.org/abs/2508.04038) [arXiv 2025] | Trad. TS Anal. | Class. | ✔ |  |  | ✔ | ✔ |  | M | P |
| [TimeMaster: Training Time-Series Multimodal LLMs to Reason via   Reinforcement Learning](https://arxiv.org/abs/2506.13705) [arXiv 2025] | Trad. TS Anal. | Class. | ✔ | ✔ |  | ✔ |  | ✔ | 0 | H |
| [Towards Time-Series Reasoning with LLMs](https://openreview.net/forum?id=W0UTR3LLwj) [NeurIPS Workshop on Time   Series in the Age of Large Models 2024] | Trad. TS Anal. | Class. | ✔ |  |  |  |  | ✔ | 0 | S |
| [REALM: RAG-Driven Enhancement of Multimodal Electronic Health   Records Analysis via Large Language Models](https://arxiv.org/abs/2402.07016) [arXiv 2024] | Trad. TS Anal. | Class. | ✔ | ✔ |  | ✔ | ✔ | ✔ | 0 | P |
| [Harnessing Vision-Language Models for Time Series Anomaly   Detection](https://arxiv.org/abs/2506.06836) [arXiv 2025] | Trad. TS Anal. | Anom. Det. | ✔ | ✔ |  |  |  | ✔ | 0 | P |
| [Large Language Models can Deliver Accurate and Interpretable   Time Series Anomaly Detection](https://doi.org/10.1145/3711896.3737239) [KDD 2025] | Trad. TS Anal. | Anom. Det. | ✔ | ✔ |  | ✔ | ✔ |  | 0 | P |
| [Can LLMs Serve As Time Series Anomaly Detectors?](https://arxiv.org/abs/2408.03475) [arXiv 2024] | Trad. TS Anal. | Anom. Det. | ✔ |  |  |  |  |  | 0 | S |
| [Large language models can be zero-shot anomaly detectors for   time series?](https://arxiv.org/abs/2405.14755) [DSAA 2024] | Trad. TS Anal. | Anom. Det. |  |  | ✔ |  |  |  | 0 | P |
| [Large-model-based smart agent for time series anomaly   detection in power systems](https://www.sciencedirect.com/science/article/pii/S0957417425025345) [Expert Systems with   Applications 2025] | Trad. TS Anal. | Anom. Det. |  | ✔ |  |  |  |  | 1 | P |
| [LEMAD: LLM-Empowered Multi-Agent System for Anomaly Detection   in Power Grid Services](https://www.mdpi.com/2079-9292/14/15/3008) [Electronics 2025] | Trad. TS Anal. | Anom. Det. | ✔ |  |  |  |  | ✔ | M | P |
| [A Time Series Multitask Framework Integrating a Large Language   Model, Pre-Trained Time Series Model, and Knowledge Graph](https://arxiv.org/abs/2503.07682) [arXiv 2025] | Trad. TS Anal. | Mult. Tasks |  |  |  | ✔ | ✔ | ✔ | 0 | P |
| [Agentic Retrieval-Augmented Generation for Time Series   Analysis](https://arxiv.org/abs/2408.14484) [arXiv 2024] | Trad. TS Anal. | Mult. Tasks |  |  |  | ✔ | ✔ |  | M | H |
| [Inferring Events from Time Series using Language Models](https://arxiv.org/abs/2503.14190) [arXiv 2025] | Expl. & Und. | Temp. QA | ✔ |  |  |  |  | ✔ | 0 | H |
| [Large Language Models Can Learn Temporal Reasoning](https://aclanthology.org/2024.acl-long.563/) [ACL 2024] | Expl. & Und. | Temp. QA | ✔ | ✔ |  |  |  |  | 0 | S |
| [TempoGPT: Enhancing Time Series Reasoning via Quantizing   Embedding](https://arxiv.org/abs/2501.07335) [arXiv 2025] | Expl. & Und. | Expl. Diagn. | ✔ |  |  |  |  | ✔ | 0 | S |
| [Time Series Language Model for Descriptive Caption Generation](https://arxiv.org/abs/2501.01832) [arXiv 2025] | Expl. & Und. | Expl. Diagn. |  |  | ✔ | ✔ |  | ✔ | 0 | S |
| [Visual Analysis of Time Series Data for Multi-Agent Systems   Driven by Large Language Models](https://doi.org/10.1145/3712335.3712410) [SPCNC 2024] | Expl. & Und. | Expl. Diagn. | ✔ |  |  | ✔ | ✔ | ✔ | M | P |
| [A Multimodal Foundation Agent for Financial Trading:   Tool-Augmented, Diversified, and Generalist](https://doi.org/10.1145/3637528.3671801) [KDD 2024] | Causal Inf. | Auto. Policy | ✔ | ✔ |  | ✔ | ✔ | ✔ | 1 | P |
| [FINMEM: A Performance-Enhanced LLM Trading Agent with Layered   Memory and Character Design](https://openreview.net/forum?id=sstfVOwbiG) [ICLR Workshop on Large   Language Model (LLM) Agents 2024] | Causal Inf. | Auto. Policy | ✔ | ✔ |  | ✔ | ✔ | ✔ | 1 | P |
| [Open-TI: Open Traffic Intelligence with Augmented Language   Model](https://arxiv.org/abs/2401.00211) [International Journal of   Machine Learning and Cybernetics 2024] | Causal Inf. | Auto. Policy | ✔ |  |  | ✔ |  |  | M | P |
| [SocioDojo: Building Lifelong Analytical Agents with Real-world   Text and Time Series](https://openreview.net/forum?id=s9z0HzWJJp) [ICLR 2024] | Causal Inf. | Adv. Dec. Supp. | ✔ | ✔ |  | ✔ | ✔ | ✔ | M | P |
| [GenG: An LLM-based Generic Time Series Data Generation   Approach for Edge Intelligence via Cross-domain Collaboration](https://doi.org/10.1109/INFOCOMWKSHPS61880.2024.10620716) [INFOCOM Wksps 2024] | TS Gen. | Cond. Synth. | ✔ |  |  |  |  | ✔ | 0 | S |
| [Using Gen AI Agents With GAE And VAE To Enhance Resilience Of   Us Markets](https://ssrn.com/abstract=5123068) [SSRN 2025] | TS Gen. | Cond. Synth. |  | ✔ |  | ✔ | ✔ |  | 0 | P |


---

## Research Papers for Branch-Structured Reasoning

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Paper&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Primary Objective | Task | T-Dec | T-Ver | T-Ens | T-Tool | T-Know | T-Multi | T-Agent | T-Align |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [Can Competition Enhance the Proficiency of Agents Powered by   Large Language Models in the Realm of News-driven Time Series Forecasting?](https://arxiv.org/abs/2504.10210) [arXiv 2025] | Trad. TS Anal. | Forc. | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | M | S |
| [From News to Forecast: Integrating Event Analysis in LLM-Based   Time Series Forecasting with Reflection](https://openreview.net/forum?id=tj8nsfxi5r) [NeurIPS 2024] | Trad. TS Anal. | Forc. | ✔ | ✔ |  |  | ✔ | ✔ | M | S |
| [Context-Aware Probabilistic Modeling with LLM for Multimodal   Time Series Forecasting](https://arxiv.org/abs/2505.10774) [arXiv 2025] | Trad. TS Anal. | Forc. |  |  | ✔ |  |  | ✔ | 0 | P |
| [Empowering Time Series Forecasting with LLM-Agents](https://arxiv.org/abs/2508.04231) [arXiv 2025] | Trad. TS Anal. | Forc. | ✔ | ✔ |  | ✔ | ✔ |  | 1 | P |
| [CoLLM: Industrial Large-Small Model Collaboration with Fuzzy   Decision-making Agent and Self-Reflection](https://doi.org/10.1109/TFUZZ.2025.3594229) [IEEE Transactions on Fuzzy   Systems 2025] | Trad. TS Anal. | Forc. |  | ✔ | ✔ |  |  |  | 0 | S |
| [Explainable Multi-modal Time Series Prediction with   LLM-in-the-Loop](https://arxiv.org/abs/2503.01013) [arXiv 2025] | Trad. TS Anal. | Forc. | ✔ | ✔ | ✔ |  |  | ✔ | M | P |
| [Enhancing LLM Reasoning for Time Series Classification by   Tailored Thinking and Fused Decision](https://arxiv.org/abs/2506.00807) [arXiv 2025] | Trad. TS Anal. | Class. | ✔ | ✔ |  | ✔ |  |  | 0 | P |
| [ColaCare: Enhancing Electronic Health Record Modeling through   Large Language Model-Driven Multi-Agent Collaboration](https://doi.org/10.1145/3696410.3714877) [WWW 2025] | Trad. TS Anal. | Class. | ✔ | ✔ |  | ✔ | ✔ | ✔ | M | P |
| [TimeCAP: Learning to Contextualize, Augment, and Predict Time   Series Events with Large Language Model Agents](https://doi.org/10.1609/aaai.v39i17.33989) [AAAI 2025] | Trad. TS Anal. | Class. | ✔ |  | ✔ | ✔ | ✔ | ✔ | M | P |
| [AD-AGENT: A Multi-agent Framework for End-to-end Anomaly   Detection](https://arxiv.org/abs/2505.12594) [arXiv 2025] | Trad. TS Anal. | Anom. Det. | ✔ | ✔ |  | ✔ | ✔ |  | M | P |
| [ARGOS: Agentic Time-Series Anomaly Detection with Autonomous   Rule Generation via Large Language Models](https://arxiv.org/abs/2501.14170) [arXiv 2025] | Trad. TS Anal. | Anom. Det. | ✔ | ✔ | ✔ |  |  |  | 0 | P |
| [See it, Think it, Sorted: Large Multimodal Models are Few-shot   Time Series Anomaly Analyzers](https://arxiv.org/abs/2411.02465) [arXiv 2024] | Trad. TS Anal. | Anom. Det. | ✔ | ✔ | ✔ |  |  | ✔ | 0 | P |
| [LLM-TSFD: An industrial time series human-in-the-loop fault   diagnosis method based on a large language model](https://doi.org/10.1016/j.eswa.2024.125861) [Expert Systems with   Applications 2025] | Trad. TS Anal. | Anom. Det. | ✔ | ✔ |  | ✔ | ✔ |  | 1 | P |
| [Domain-Oriented Time Series Inference Agents for Reasoning and   Automated Analysis](https://arxiv.org/abs/2410.04047) [arXiv 2025] | Trad. TS Anal. | Mult. Tasks | ✔ | ✔ |  | ✔ | ✔ |  | 1 | P |
| [MERIT: Multi-Agent Collaboration for Unsupervised Time Series   Representation Learning](https://aclanthology.org/2025.findings-acl.1231/) [ACL 2025] | Trad. TS Anal. | Mult. Tasks | ✔ | ✔ |  | ✔ | ✔ |  | M | P |
| [Decoding Time Series with LLMs: A Multi-Agent Framework for   Cross-Domain Annotation](https://arxiv.org/abs/2410.17462) [arXiv 2024] | Expl. & Und. | Expl. Diagn. | ✔ | ✔ |  |  |  | ✔ | M | P |
| [AgentFM: Role-Aware Failure Management for Distributed   Databases with LLM-Driven Multi-Agents](https://doi.org/10.1145/3696630.3728492) [FSE 2025] | Expl. & Und. | Expl. Diagn. | ✔ |  |  | ✔ | ✔ | ✔ | M | P |
| [ElliottAgents: A Natural Language-Driven Multi-Agent System   for Stock Market Analysis and Prediction](https://aclanthology.org/2024.paclic-1.91/) [PACLIC 2024] | Expl. & Und. | Expl. Diagn. | ✔ | ✔ |  | ✔ | ✔ |  | M | P |
| [Can Large Language Models Adequately Perform Symbolic   Reasoning Over Time Series?](https://arxiv.org/abs/2508.03963) [arXiv 2025] | Expl. & Und. | Struct. Disc. | ✔ | ✔ | ✔ | ✔ |  | ✔ | 0 | P |
| [FinArena: A Human-Agent Collaboration Framework for Financial   Market Analysis and Forecasting](https://arxiv.org/abs/2503.02692) [arXiv 2025] | Causal Inf. | Auto. Policy | ✔ | ✔ |  | ✔ | ✔ | ✔ | M | P |
| [FinCon: A Synthesized LLM Multi-Agent System with Conceptual   Verbal Reinforcement for Enhanced Financial Decision Making](https://openreview.net/forum?id=dG1HwKMYbC) [NeurIPS 2024] | Causal Inf. | Auto. Policy | ✔ | ✔ |  | ✔ | ✔ | ✔ | M | P |
| [TradingAgents: Multi-Agents LLM Financial Trading Framework](https://openreview.net/forum?id=4QPrXwMQt1) [AAA Workshop on Multi-Agent AI   in the Real World 2025] | Causal Inf. | Auto. Policy | ✔ | ✔ |  | ✔ | ✔ | ✔ | M | P |
| [BRIDGE: Bootstrapping Text to Control Time-Series Generation   via Multi-Agent Iterative Optimization and Diffusion Modeling](https://openreview.net/forum?id=uRD6wkqulN) [ICML 2025] | TS Gen. | Cond. Synth. | ✔ | ✔ |  | ✔ | ✔ | ✔ | M | P |


---

## Non-Research Papers

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Paper&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Type |
| --- | --- |
| [Evaluating Large Language Models on Time Series Feature   Understanding: A Comprehensive Taxonomy and Benchmark](https://aclanthology.org/2024.emnlp-main.1204/) [EMNLP 2024] | Reasoning-First Benchmarks |
| [Implicit Reasoning in Deep Time Series Forecasting](https://openreview.net/forum?id=PFZiJwX9j5) [NeurIPS Workshop on Time   Series in the Age of Large Models 2024] | Reasoning-First Benchmarks |
| [Investigating Compositional Reasoning in Time Series   Foundation Models](https://arxiv.org/abs/2502.06037) [arXiv 2025] | Reasoning-First Benchmarks |
| [Evaluating System 1 vs. 2 Reasoning Approaches for Zero-Shot   Time Series Forecasting: A Benchmark and Insights](https://arxiv.org/abs/2503.01895) [arXiv 2025] | Reasoning-First Benchmarks |
| [MTBench: A Multimodal Time Series Benchmark for Temporal   Reasoning and Question Answering](https://arxiv.org/abs/2503.16858) [arXiv 2025] | Reasoning-First Benchmarks |
| [Time-MQA: Time Series Multi-Task Question Answering with   Context Enhancement](https://aclanthology.org/2025.acl-long.1437/) [ACL 2025] | Reasoning-First Benchmarks |
| [PUB: Plot Understanding Benchmark and Dataset for Evaluating   Large Language Models on Synthetic Visual Data Interpretation](https://arxiv.org/abs/2409.02617) [arXiv 2024] | Reasoning-First Benchmarks |
| [Context is Key: A Benchmark for Forecasting with Essential   Textual Information](https://arxiv.org/abs/2410.18959) [ICML 2025] | Reasoning-First Benchmarks |
| [TimeSeriesGym: A Scalable Benchmark for (Time Series) Machine   Learning Engineering Agents](https://arxiv.org/abs/2505.13291) [arXiv 2025] | Reasoning-First Benchmarks |
| [SocioDojo: Building Lifelong Analytical Agents with Real-world   Text and Time Series](https://openreview.net/forum?id=s9z0HzWJJp) [ICLR 2024] | Reasoning-First Benchmarks |
| [Inferring Events from Time Series using Language Models](https://arxiv.org/abs/2503.14190) [arXiv 2025] | Reasoning-First Benchmarks |
| [Intervention-Aware Forecasting: Breaking Historical Limits   from a System Perspective](https://arxiv.org/abs/2405.13522) [arXiv 2024] | Reasoning-First Benchmarks |
| [ITFormer: Bridging Time Series and Natural Language for   Multi-Modal QA with Large-Scale Multitask Dataset](https://openreview.net/forum?id=GByP03IitA) [ICML 2025] | Reasoning-First Benchmarks |
| [GEM: Empowering MLLM for Grounded ECG Understanding with Time   Series and Images](https://arxiv.org/abs/2503.06073) [arXiv 2025] | Reasoning-Ready Benchmarks |
| [See it, Think it, Sorted: Large Multimodal Models are Few-shot   Time Series Anomaly Analyzers](https://arxiv.org/abs/2411.02465) [arXiv 2024] | Reasoning-Ready Benchmarks |
| [GPT4MTS: Prompt-Based Large Language Model for Multimodal   Time-Series Forecasting](https://ojs.aaai.org/index.php/AAAI/article/view/30383) [AAAI 2024] | Reasoning-Ready Benchmarks |
| [Multi-Modal Forecaster: Jointly Predicting Time Series and   Textual Data](https://arxiv.org/abs/2411.06735) [arXiv 2024] | Reasoning-Ready Benchmarks |
| [Retrieval-augmented Large Language Models for Financial Time   Series Forecasting](https://arxiv.org/abs/2502.05878) [arXiv 2025] | Reasoning-Ready Benchmarks |
| [TEMPO: Prompt-based Generative Pre-trained Transformer for   Time Series Forecasting](https://openreview.net/forum?id=YH5w12OUuU) [ICLR 2024] | Reasoning-Ready Benchmarks |
| [Time Travel is Cheating: Going Live with DeepFund for   Real-Time Fund Investment Benchmarking](https://arxiv.org/abs/2505.11065) [arXiv 2025] | Reasoning-Ready Benchmarks |
| [Momentor: Advancing Video Large Language Model with   Fine-Grained Temporal Reasoning](https://arxiv.org/abs/2402.11435) [ICML 2024] | Reasoning-Ready Benchmarks |
| [MoTime: A Dataset Suite for Multimodal Time Series Forecasting](https://arxiv.org/abs/2505.15072) [arXiv 2025] | Reasoning-Ready Benchmarks |
| [Time-IMM: A Dataset and Benchmark for Irregular Multimodal   Multivariate Time Series](https://arxiv.org/abs/2506.10412) [arXiv 2025] | Reasoning-Ready Benchmarks |
| [Time-MMD: Multi-Domain Multimodal Dataset for Time Series   Analysis](https://openreview.net/forum?id=fuD0h4R1IL) [NeurIPS 2024] | Reasoning-Ready Benchmarks |
| [TSFM-Bench: A Comprehensive and Unified Benchmark of   Foundation Models for Time Series Forecasting](https://doi.org/10.1145/3711896.3737442) [KDD 2025] | Reasoning-Ready Benchmarks |
| [Well Googled is Half Done: Multimodal Forecasting of New   Fashion Product Sales with Image-based Google Trends](https://arxiv.org/abs/2109.09824) [Journal of Forecasting 2024] | Reasoning-Ready Benchmarks |
| [Time-RA: Towards Time Series Reasoning for Anomaly with LLM   Feedback](https://arxiv.org/abs/2507.15066) [arXiv 2025] | Reasoning-Ready Benchmarks |
| [A Picture is Worth A Thousand Numbers: Enabling LLMs Reason   about Time Series via Visualization](https://aclanthology.org/2025.naacl-long.383/) [NAACL 2025] | General-Purpose Time Series Benchmarks |
| [Are Language Models Actually Useful for Time Series   Forecasting?](https://openreview.net/forum?id=DV15UbHCY1) [NeurIPS 2024] | General-Purpose Time Series Benchmarks |
| [Can Large Language Models Adequately Perform Symbolic   Reasoning Over Time Series?](https://arxiv.org/abs/2508.03963) [arXiv 2025] | General-Purpose Time Series Benchmarks |
| [Can LLMs Understand Time Series Anomalies?](https://openreview.net/forum?id=LGafQ1g2D2) [ICLR 2025] | General-Purpose Time Series Benchmarks |
| [Can Multimodal LLMs Perform Time Series Anomaly Detection?](https://arxiv.org/abs/2502.17812) [arXiv 2025] | General-Purpose Time Series Benchmarks |
| [TimeSeriesExam: A Time Series Understanding Exam](https://openreview.net/forum?id=oXRX7ABgLz) [NeurIPS Workshop on Time   Series in the Age of Large Models 2024] | General-Purpose Time Series Benchmarks |
| [Can LLMs Serve As Time Series Anomaly Detectors?](https://arxiv.org/abs/2408.03475) [arXiv 2024] | General-Purpose Time Series Benchmarks |
| [Language Models Still Struggle to Zero-shot Reason about Time   Series](https://aclanthology.org/2024.findings-emnlp.201/) [EMNLP 2024] | General-Purpose Time Series Benchmarks |
| [Chat-TS: Enhancing Multi-Modal Reasoning Over Time-Series and   Natural Language Data](https://arxiv.org/abs/2503.10883) [arXiv 2025] | General-Purpose Time Series Benchmarks |
| [ChatTS: Aligning Time Series with LLMs via Synthetic Data for   Enhanced Understanding and Reasoning](https://arxiv.org/abs/2412.03104) [VLDB 2025] | General-Purpose Time Series Benchmarks |
| [Domain-Oriented Time Series Inference Agents for Reasoning and   Automated Analysis](https://arxiv.org/abs/2410.04047) [arXiv 2025] | General-Purpose Time Series Benchmarks |
| [FinBen: An Holistic Financial Benchmark for Large Language   Models](https://openreview.net/forum?id=loDHZstVP6) [NeurIPS 2024] | General-Purpose Time Series Benchmarks |
| [FinTSB: A Comprehensive and Practical Benchmark for Financial   Time Series Forecasting](https://arxiv.org/abs/2502.18834) [arXiv 2025] | General-Purpose Time Series Benchmarks |
| [Foundation Models for Time Series Analysis: A Tutorial and   Survey](https://doi.org/10.1145/3637528.3671451) [KDD 2024] | Surveys and Tutorials |
| [Large Language Models for Forecasting and Anomaly Detection: A   Systematic Literature Review](https://arxiv.org/abs/2402.10350) [arXiv 2024] | Surveys and Tutorials |
| [Empowering Time Series Analysis with Synthetic Data: A Survey   and Outlook in the Era of Foundation Models](https://arxiv.org/abs/2503.11411) [arXiv 2025] | Surveys and Tutorials |
| [Integrating Artificial Intelligence Agents with the Internet   of Things for Enhanced Environmental Monitoring: Applications in Water   Quality and Climate Data](https://www.mdpi.com/2079-9292/14/4/696) [Electronics 2025] | Surveys and Tutorials |
| [LLMs Meet Cross-Modal Time Series Analytics: Overview and   Directions](https://arxiv.org/abs/2507.10620) [arXiv 2025] | Surveys and Tutorials |
| [Are Language Models Actually Useful for Time Series   Forecasting?](https://openreview.net/forum?id=DV15UbHCY1) [NeurIPS 2024] | Position and Vision Papers |
| [Context parroting: A simple but tough-to-beat baseline for   foundation models in scientific machine learning](https://arxiv.org/abs/2505.11349) [arXiv 2025] | Position and Vision Papers |
| [Position: Empowering Time Series Reasoning with Multimodal   LLMs](https://arxiv.org/abs/2502.01477) [arXiv 2025] | Position and Vision Papers |
| [Position: What Can Large Language Models Tell Us about Time   Series Analysis](https://arxiv.org/abs/2402.02713) [ICML 2024] | Position and Vision Papers |


---

## How to Contribute

We welcome contributions to keep this table updated:

1. Add missing papers as new rows following the same format.  
2. Ensure each paper is annotated with exactly one **Reasoning Topology** and one **Primary Objective**, plus appropriate tags.  
3. Submit a pull request.

---

## Citation

If you find this resource useful, please cite our survey (bibtex entry forthcoming).
