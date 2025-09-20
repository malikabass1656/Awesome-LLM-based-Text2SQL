# Awesome-LLM-based-Text2SQL

<div align="center">
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-green.svg"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/stars/DEEP-PolyU/Awesome-LLM-based-Text2SQL"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/forks/DEEP-PolyU/Awesome-LLM-based-Text2SQL"/></a>
      <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/last-commit/DEEP-PolyU/Awesome-LLM-based-Text2SQL?color=blue"/></a>
</div>

This repository provides a comprehensive collection of research papers, benchmarks, and open-source projects on **large language model-based text-to-SQL (LLM-based Text-to-SQL)**. It includes all the contents from our survey paper *"[**Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL**](https://arxiv.org/pdf/2406.08426)"* and will be continuously updated to incorporate the up-to-date advances and notable contributions from the text-to-SQL community. Stay tuned!!

🤗 **You are vey welcome to contribute to this repository** by launching an issue or a pull request. If you find any missing resources or come across interesting new research works, please don’t hesitate to open an issue or submit a PR!

📫 **Contact us via emails:**  `zijin[dot]hong[at]connect[dot]polyu[dot]hk`

**📃 Please [cite our paper](#-citation)** if you find our survey or repository helpful!

## 🔥 News

* **[2025-09-14]** 🔥🔥 Repository launched based on our survey paper to keep track of recent progress in LLM-based text-to-SQL.
* **[2025-09-02]** 🎉🎉 Our paper *"Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL"* has been **accepted by *IEEE Transactions on Knowledge and Data Engineering (TKDE)*!**
* **[2025-05-01]** 🎉🎉 Our paper *"Struture-Guided Large Language Models for Text-to-SQL Generation"* has been **accepted by *International Conference of Machine Learning (ICML)*!**

---

<div>
<h3 align="center">
       <p align="center"><img width="80%" src="figures/overview.svg" /></p>
    <p align="center"><em>Overview of LLM-based Text-to-SQL Workflow </em></p>
</div>
A user asks a question about football leagues. The LLM takes this question together with the schema of the corresponding database as input and generates an SQL query as output. The generated SQL is then executed on the database, retrieving the result <em>"The 5 leagues with the highest matches"</em>, which answers the user's question.

## 📜 Catalog

> **[Awesome-LLM-based-Text2SQL](#-awesome-llm-based-text2sql)**
>
>  - **[🔥 News](#-news)**
>  - **[📜 Catalog](#-catalog)**
>  - **[📈 Trends](#-trends)**
>  - **[📰 Surveys](#-surveys)**
>  - **[🏆 Benchmarks](#-benchmarks)**
>  - **[🗃️ Datasets](#️-datasets)**
>    - [Original Datasets](#original-datasets)
>    - [Post-annotated Datasets](#post-annotated-datasets)
>  - **[🪴 Taxonomy](#-taxonomy)**
>    - [In-cotext Learning](#)
>      - [Decomposition](#)
>    - [Fine-tuning](#)
>      - [Pre-training](#)
>  - **[📃 Citation](#-citation)**

---


## 📈 Trends

<div>
<h3 align="center">
       <p align="center"><img width="100%" src="figures/trends.svg" /></p>
    <p align="center"><em>A Sketch of Research Trends in the Field of Text-to-SQL with Representative Works </em></p>
</div>
Before 2023, the focus is on a selection of representative traditional studies. However, from 2023 onward, the emphasis shifts to the rapid advancements driven by LLMs, marking a significant acceleration in the field.

## 📰 Surveys

* ![TKDE](https://img.shields.io/badge/TKDE2025-FF6347) Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL [[Paper]()] [[Code]()]
* ![CSUR2025](https://img.shields.io/badge/CSUR2025-3CB371) A Survey on Employing Large Language Models for Text-to-SQL Tasks [[Paper]()]
* ![TKDE](https://img.shields.io/badge/TKDE2025-FF6347?style=flat) A Survey of Text-to-SQL in the Era of LLMs: Where are We, and Where are We Going? [[Paper]()]
* ![TKDE](https://img.shields.io/badge/TKDE2024-FF6347?style=flat) Natural Language Interfaces for Tabular Data Querying and Visualization: A Survey [[Paper]()]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) Large Language Model Enhanced Text-to-SQL Generation: A Survey [[Paper]()]
* ![VLDBJ2023](https://img.shields.io/badge/VLDBJ2023-4B0082) A Survey on Deep Learning Approaches for Text-to-SQL [[Paper]()]
* ![VLDB2023](https://img.shields.io/badge/VLDB2023-800080) Natural Language Interfaces for Databases with Deep Learning [[Paper]()]
* ![arXiv2022](https://img.shields.io/badge/arXiv2022-B31B1B) A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions [[Paper]()]
* ![COLING2022](https://img.shields.io/badge/COLING2022-00CED1) Recent Advances in Text-to-SQL: A Survey of What We Have and What We Expect [[Paper]()]

## 🏆 Benchmarks

In the era of LLMs, two benchmarks and their variants/extensions are widely recognized for evaluating text-to-SQL capabilities. **We will continually update the top five methods on each benchmark** to showcase the latest advances in the text-to-SQL community. These benchmarks, along with other text-to-SQL dataset papers, are listed in the [datasets section](#-datasets) below.

#### [BIRD](https://bird-bench.github.io/) - A Big Bench for Large-Scale Database Grounded Text-to-SQL


| Method/Model | Dev EX (%) | Test EX (%) | Paper/Code | Date |
|--------------|------------|-------------|------------|------|
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) LongData-SQL | 74.32 | **77.53** | [<u>Proprietary</u>] | 2025-07-14 |
| ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) AskData + GPT-4o | **75.36** | 77.14 | [[Paper](https://arxiv.org/pdf/2505.19988)] | 2025-03-11 |
| ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) CHASE-SQL + Gemini | 74.90 | 76.02 | [[Paper](https://openreview.net/pdf?id=CvGqMD5OtX)] | 2025-04-16 |
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) TCDataAgent-SQL | 74.12 | 75.74 | [[Report](https://cloud.tencent.com/developer/article/2537769)] | 2025-05-30 |
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) Contextual-SQL | 73.50 | 75.63 | [[Report](https://contextual.ai/blog/open-sourcing-the-best-local-text-to-sql-system/)] [[Code](https://github.com/ContextualAI/bird-sql)] | 2025-02-27 |
| ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) XiYan-SQL | 73.34 | 75.63 | [[Paper](https://arxiv.org/pdf/2411.08599)] [[Code](https://github.com/XGenerationLab/XiYan-SQL)] | 2024-12-17 |

---

#### [Spider1.0](https://yale-lily.github.io/spider) - Semantic Parsing and Text-to-SQL Challenge

| Method/Model | Dev EX (%) | Test EX (%) | Paper/Code | Date |
|--------------|------------|-------------|------------|------|
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) MiniSeek | - | **91.2** | [[Report](https://www.seek.ai/blog/miniseek-first-model-to-surpass-90-accuracy-on-spider-test-benchmark)] | 2023-11-02 |
| ![VLDB2024](https://img.shields.io/badge/VLDB2024-800080) DAIL-SQL + GPT-4 | **82.4** | 86.6 | [[Paper](https://www.vldb.org/pvldb/vol17/p1132-gao.pdf)] [[Code](https://github.com/BeachWang/DAIL-SQL)] | 2023-08-20 |
| ![NeurIPS2025](https://img.shields.io/badge/NeurIPS2025-2E8B57) DIN-SQL + GPT-4 | 74.2 | 85.3 | [[Paper](https://openreview.net/pdf?id=p53QDxSIc5)] [[Code](https://github.com/MohammadrezaPourreza/Few-shot-NL2SQL-with-prompting)] | 2023-04-21 |
| ![arXiv2023](https://img.shields.io/badge/arXiv2023-B31B1B) C3 + ChatGPT | 81.8 | 82.3 | [[Paper](https://arxiv.org/pdf/2307.07306)] [[Code](https://github.com/bigbigwatermalon/C3SQL)] | 2023-06-01 |
| ![AAAI2025](https://img.shields.io/badge/AAAI2025-006400) RESDSQL-3B + NatSQL | 84.1 | 79.9 | [[Paper](https://arxiv.org/pdf/2302.05965)] [[Code](https://github.com/RUCKBReasoning/RESDSQL)] | 2023-02-27 |

---

#### [Spider2.0](https://spider2-sql.github.io/) - Evaluating Language Models on Real-World Enterprise Text-to-SQL Workflows

| Method/Model | Snow Score | Lite Score | Paper/Code | Date |
|--------------|------------|----------------|------------|------|
| ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) AgenticData + Qwen3 | - | **44.5** | [[Paper](https://arxiv.org/pdf/2508.05002)] | 2025-08-07 |
| ![ICLR2025](https://img.shields.io/badge/ICLR2025Workshop-7CFC00) ReFoRCE + o3 | **37.11** | 37.84 | [[Paper](https://openreview.net/pdf?id=OuFIfDBwQd)] [[Code](https://github.com/Snowflake-Labs/ReFoRCE)] | 2025-05-22 |
| ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) RSL-SQL + o3 | - | 33.09 | [[Paper](https://arxiv.org/pdf/2411.00073)] [[Code](https://github.com/Laqcce-cao/RSL-SQL)] | 2025-07-10 |
| ![EMNLP2025](https://img.shields.io/badge/EMNLP2025-00BFFF) LinkAlign + DeepSeek-R1 | - | 33.09 | [[Paper](https://arxiv.org/pdf/2503.18596)] [[Code](https://github.com/Satissss/LinkAlign)] | 2025-04-27 |
| ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) Spider-Agent + Claude-3.7-Sonnet | - | 28.52 | [[Paper](https://openreview.net/pdf?id=XmProj9cPs)] [[Code](https://github.com/xlang-ai/Spider2)] | 2025-03-16 |

---

#### [BIRD-CRITIC](https://bird-critic.github.io/) - Can LLMs Fix User Issues in Real-World Database Applications?


| Model | SR (%) | Date |
|-------|--------|------|
| ByteBrain-Agent | **43.33** | 2025-06-10 |
| GPT-5-High | 34.96 | 2025-09-04 |
| grok-4 | 33.68 | 2025-07-18 |
| DeepSeek-R1 | 33.51 | 2025-04-20 |
| o3-Mini | 33.33 | 2025-04-20 |

---

#### [BIRD-INTERACT](https://bird-interact.github.io/) - Re-imagining Text-to-SQL Evaluation via Lens of Dynamic Interactions


| Model/Method | Reward | Date |
|--------------|--------|------|
| Gemini-2.5-Pro | **20.92** | 2025-08-22 |
| o3-Mini | 20.27 | 2025-08-22 |
| Claude-Sonnet-4 | 18.35 | 2025-08-22 |
| Qwen-3-Coder-480B | 17.75 | 2025-08-22 |
| DeepSeek-V3 | 15.15 | 2025-08-22 |

## 🗃️ Datasets

**We categorize the datasets into *Original Datasets* and *Post-annotated Datasets*** based on whether they were released with the original dataset (question–SQL pairs) and databases, or were developed by adapting existing datasets and databases with special settings. The *Post-annotated Datasets* rely on the databases from [Spider 1.0](https://yale-lily.github.io/spider). For each original dataset, we list its characteristics, number of examples, and number of databases under the dataset title.

### Original Datasets

* ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) **BIRD-CRITIC** | SWE-SQL: Illuminating LLM Pathways to Solve User SQL Issues in Real-World Applications [[Paper]()] [[Code]()] [[Dataset]()]<br>
  *Knowledge-augmented, Long-context; #Example: 600; #DB: 95*
* ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) **Spider2.0** | Spider 2.0: Evaluating Language Models on Real-world Enterprise Text-to-SQL Workflows [[Paper]()] [[Code]()] [[Dataset]()]<br>
  *Knowledge-augmented, Long-context; #Example: 632; #DB: 213*
* ![SIGMOD2025](https://img.shields.io/badge/SIGMOD2025-8A2BE2) **BULL** | FinSQL: Model-Agnostic LLMs-based Text-to-SQL Framework for Financial Analysis [[Paper](https://arxiv.org/pdf/2401.10506)] [[Code](https://github.com/bigbigwatermalon/FinSQL)] [[Dataset](https://drive.google.com/file/d/1OtyFdH9cs-6bEVj8yKK4Zt53N52L_dBH/view?usp=sharing)]<br>
  *Knowledge-augmented, Long-context; #Example: 4,966; #DB: 3*
* ![NeurIPS2023](https://img.shields.io/badge/NeurIPS2023-2E8B57) **BIRD** | Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs [[Paper](https://openreview.net/pdf?id=dI4wzAE6uV)] [[Code]()] [[Dataset]()]<br>
  *Cross-domain, Knowledge-augmented; #Example: 12,751; #DB: 95*
* ![ACL2021](https://img.shields.io/badge/ACL2021-1E90FF) **KaggleDBQA** | KaggleDBQA: Realistic Evaluation of Text-to-SQL Parsers [[Paper](https://aclanthology.org/2021.acl-long.176.pdf)] [[Code](https://github.com/Chia-Hsuan-Lee/KaggleDBQA)] [[Dataset]()]<br>
  *Cross-domain; #Example: 272; #DB: 8*
* ![EMNLP2020](https://img.shields.io/badge/EMNLP2020-00BFFF) **DuSQL** | DuSQL: A Large-Scale and Pragmatic Chinese Text-to-SQL Dataset [[Paper](https://aclanthology.org/2020.emnlp-main.562.pdf)] [[Dataset](https://www.luge.ai/#/luge/dataDetail?id=13)]<br>
  *Cross-domain, Cross-lingual; #Example: 23,797; #DB: 200*
* ![Findings2020](https://img.shields.io/badge/EMNLP2020Findings-87CEFA) **SQUALL** | On the Potential of Lexico-logical Alignments for Semantic Parsing to SQL Queries [[Paper](https://aclanthology.org/2020.findings-emnlp.167.pdf)] [[Code](https://github.com/tzshi/squall)] <br>
  *Cross-domain, Cross-lingual; #Example: 11,468; #DB: 1,679*
* ![EMNLP2019](https://img.shields.io/badge/EMNLP2019-00BFFF) **CoSQL** | CoSQL: A Conversational Text-to-SQL Challenge Towards Cross-Domain Natural Language Interfaces to Databases [[Paper](https://aclanthology.org/D19-1204.pdf)] [[Code](https://github.com/taoyds/cosql)] [[Dataset](https://drive.usercontent.google.com/download?id=1Y3ydpFiQQ3FC0bzdfy3groV95O_f1nXF&export=download&authuser=0)]<br>
  *Cross-domain, Context-dependent; #Example: 15,598; #DB: 200*
* ![EMNLP2018](https://img.shields.io/badge/EMNLP2018-00BFFF) **Spider** | Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task [[Paper](https://aclanthology.org/D18-1425.pdf)] [[Code](https://github.com/taoyds/spider)] [[Dataset](https://drive.google.com/file/d/1403EGqzIDoHMdQF4c9Bkyl7dZLZ5Wt6J/view)]<br>
  *Cross-domain; #Example: 10,181; #DB: 200*
* ![arXiv2017](https://img.shields.io/badge/arXiv2017-B31B1B) **WikiSQL** | Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning [[Paper](https://arxiv.org/pdf/1709.00103)] [[Code](https://github.com/salesforce/WikiSQL)] [[Dataset](https://github.com/salesforce/WikiSQL/tree/master/collection)]<br>
  *Cross-domain; #Example: 80,654; #DB: 26,521*

### Post-annotated Datasets

* ![ICLR2023](https://img.shields.io/badge/ICLR2023-7CFC00) **Dr. Spider** | Dr.Spider: A Diagnostic Evaluation Benchmark towards Text-to-SQL Robustness [[Paper](https://openreview.net/pdf?id=Wc5bmZZU9cy)] [[Code](https://github.com/awslabs/diagnostic-robustness-text-to-sql)]<br>
  *Robustness; Perturbations in DB, query and SQL*
* ![ACL2022](https://img.shields.io/badge/ACL2022-1E90FF) **ADVETA** | Towards Robustness of Text-to-SQL Models Against Natural and Realistic Adversarial Table Perturbation [[Paper](https://aclanthology.org/2022.acl-long.142.pdf)] [[Code](https://github.com/microsoft/ContextualSP/tree/master/robustness_of_text_to_sql)] [[Dataset](https://github.com/microsoft/ContextualSP/blob/master/robustness_of_text_to_sql/adveta_1.0.zip)]<br>
  *Robustness; Adversarial table perturbation*
* ![Findings2022](https://img.shields.io/badge/NAACL2022Findings-87CEFA) **Spider-SS&CG** | Measuring and Improving Compositional Generalization in Text-to-SQL via Component Alignment [[Paper](https://aclanthology.org/2022.findings-naacl.62.pdf)] [[Code](https://github.com/ygan/SpiderSS-SpiderCG)] [[Dataset](https://github.com/ygan/SpiderSS-SpiderCG/tree/main/Spider-SS)]<br>
  *Context-dependent; Splitting example into sub-examples*
* ![EMNLP2021](https://img.shields.io/badge/EMNLP2021-00BFFF) **Spider-DK** | Exploring Underexplored Limitations of Cross-Domain Text-to-SQL Generalization [[Paper](https://aclanthology.org/2021.emnlp-main.702.pdf)] [[Code](https://github.com/ygan/Spider-DK)]<br>*Knowledge-augmented; Adding domain knowledge*
*  ![ACL2021](https://img.shields.io/badge/ACL2021-1E90FF) **Spider-SYN** | Towards Robustness of Text-to-SQL Models against Synonym Substitution [[Paper](https://aclanthology.org/2021.acl-long.195.pdf)] [[Code](https://github.com/ygan/Spider-Syn)]<br>*Knowledge-augmented; Adding domain knowledge*
* ![Findings2020](https://img.shields.io/badge/EMNLP2020Findings-87CEFA) **Spider-Vietnames** | A Pilot Study of Text-to-SQL Semantic Parsing for Vietnamese [[Paper](https://aclanthology.org/2020.findings-emnlp.364.pdf)] [[Code](https://github.com/VinAIResearch/ViText2SQL)]<br>
  *Cross-lingual; Vietnamese version of Spider*
* ![NAACL2021](https://img.shields.io/badge/NAACL2021-4682B4) **Spider-Realistic** | Structure-Grounded Pretraining for Text-to-SQL [[Paper](https://aclanthology.org/2021.naacl-main.105.pdf)] [[Dataset](https://zenodo.org/records/5205322)]<br>*Robustness; Removing column names in question*
* ![EMNLP2019](https://img.shields.io/badge/EMNLP2019-00BFFF) **CSpider** | A Pilot Study for Chinese SQL Semantic Parsing [[Paper](https://aclanthology.org/D19-1377.pdf)] [[Code](https://github.com/taolusi/chisp)]<br>*Cross-lingual; Chinese version of Spider*
* ![EMNLP2019](https://img.shields.io/badge/EMNLP2019-00BFFF) **SParC** | SParC: Cross-Domain Semantic Parsing in Context [[Paper](https://aclanthology.org/P19-1443.pdf)] [[Code](https://github.com/taoyds/sparc)] [[Dataset](https://drive.usercontent.google.com/download?id=1Uu7NMHTR1tdQw1t7bAuM7OPU4LElVKfg&export=download&authuser=0)]<br>*Context-dependent; Annotate conversational contents*

## 🪴 Taxonomy

The implementation of recent LLM-based text-to-SQL methods primarily relies on in-context learning and fine-tuning, enabled by the release of both powerful proprietary and well-architected open-source LLMs. **A detailed categorization of text-to-SQL methods can be found in [our paper](https://arxiv.org/pdf/2406.08426#page=3), and subsequent latest research papers will be continually updated and aligned with this taxonomy.**

### In-context Learning

* ![EMNLP2025](https://img.shields.io/badge/EMNLP2025-00BFFF) LinkAlign: Scalable Schema Linking for Real-World Large-Scale Multi-Database Text-to-SQL  [[Paper](https://arxiv.org/pdf/2503.18596)] [[Code](https://github.com/Satissss/LinkAlign)]
* ![ICLR2025](https://img.shields.io/badge/ICLR2025Workshop-7CFC00) ReFoRCE: A Text-to-SQL Agent with Self-Refinement, Consensus Enforcement, and Column Exploration [[Paper](https://openreview.net/pdf?id=OuFIfDBwQd)] [[Code](https://github.com/Snowflake-Labs/ReFoRCE)]

### Fine-tuning

* ![ACL2025](https://img.shields.io/badge/ACL2025-1E90FF) SHARE: An SLM-based Hierarchical Action CorREction Assistant for Text-to-SQL [[Paper](https://aclanthology.org/2025.acl-long.552.pdf)] [[Code](https://github.com/quge2023/SHARE)] 
* ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL [[Paper](https://openreview.net/pdf?id=BAglD6NGy0)] [[Code](https://github.com/D2I-ai/Route)]

## 📃 Citation

```
@article{hong2025next,
  title={Next-generation database interfaces: A survey of llm-based text-to-sql},
  author={Hong, Zijin and Yuan, Zheng and Zhang, Qinggang and Chen, Hao and Dong, Junnan and Huang, Feiran and Huang, Xiao},
  journal={IEEE Transactions on Knowledge and Data Engineering},
  year={2025}
}
```

