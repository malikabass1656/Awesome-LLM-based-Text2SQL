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

📫 **Contact us via emails:** Please drop an email   `zijin[dot]hong[at]connect[dot]polyu[dot]hk`,  `qinggang[dot]zhang[at]polyu[dot]edu[dot]hk`

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
A user asks a question about football leagues. The LLM takes this question together with the schema of the corresponding database as input and generates an SQL query as output. The generated SQL is then executed on the database, retrieving the result *"The 5 leagues with the highest matches"*, which answers the user's question.

## 📜 Catalog

> **[Awesome-LLM-based-Text2SQL](#-awesome-llm-based-text2sql)**
>
>  - **[🔥 News](#-news)**
>  - **[📜 Catalog](#-catalog)**
>  - **[📈 Trends](#-trends)**
>  - **[📰 Surveys](#-surveys)**
>  - **[🗃️ Datasets](#-datasets)**
>    - [Original Datasets](#)
>      - [Long-context](#)
>    - [Post-annotated Datasets](#)
>      - [Robustness](#)
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

* ![TKDE](https://img.shields.io/badge/TKDE2025-FF6347?style=flat) Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL [[Paper]()] [[Code]()]
* ![CSUR2025](https://img.shields.io/badge/CSUR2025-3CB371) A Survey on Employing Large Language Models for Text-to-SQL Tasks [[Paper]()]
* ![TKDE](https://img.shields.io/badge/TKDE2024-FF6347?style=flat) Natural Language Interfaces for Tabular Data Querying and Visualization: A Survey [[Paper]()]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) Large Language Model Enhanced Text-to-SQL Generation: A Survey [[Paper]()]
* ![VLDBJ2023](https://img.shields.io/badge/VLDBJ2023-4B0082) A Survey on Deep Learning Approaches for Text-to-SQL [[Paper]()]
* ![VLDB2023](https://img.shields.io/badge/VLDB2023-800080) Natural Language Interfaces for Databases with Deep Learning [[Paper]()]
* ![arXiv2022](https://img.shields.io/badge/arXiv2022-B31B1B) A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions [[Paper]()]
* ![COLING2022](https://img.shields.io/badge/COLING2022-00CED1) Recent Advances in Text-to-SQL: A Survey of What We Have and What We Expect [[Paper]()]

## 🏆 Benchmarks

In the era of LLMs, two benchmarks and their variants/extensions are widely recognized for evaluating text-to-SQL capabilities. **We will continually update the top five methods on each benchmark** to showcase the latest advances in the text-to-SQL community. These benchmarks, along with other text-to-SQL dataset papers, are listed in the [datasets section](#-datasets) below.

<div style="overflow-x: auto; font-size: 14px;">
<table>
  <thead>
    <tr>
      <th style="min-width:160px;">Method/Model</th>
      <th style="min-width:100px;">Dev EX (%)</th>
      <th style="min-width:100px;">Test EX (%)</th>
      <th style="min-width:300px;">Institute - Paper/Code</th>
      <th style="min-width:90px;">Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>LongData-SQL</td>
      <td>74.32</td>
      <td><b>77.53</b></td>
      <td><i>LongShine AI Research</i> - Proprietary</td>
      <td>2025-07-14</td>
    </tr>
    <tr>
      <td>AskData + GPT-4o</td>
      <td><b>75.36</b></td>
      <td>77.14</td>
      <td><i>AT&amp;T CDO - DSAIR</i> - <img src="https://img.shields.io/badge/arXiv2025-B31B1B"> 
          <a href="https://arxiv.org/pdf/2505.19988">[Paper]</a></td>
      <td>2025-03-11</td>
    </tr>
    <!-- 其余行照此格式 -->
  </tbody>
</table>

#### [BIRD](https://bird-bench.github.io/) - A Big Bench for Large-Scale Database Grounded Text-to-SQL

<div style="overflow-x: auto;">

| Method/Model       | Dev EX (%) | Test EX (%) | Institute - Paper/Code                                       | Date       |
| ------------------ | ---------- | ----------- | ------------------------------------------------------------ | ---------- |
| LongData-SQL       | 74.32      | **77.53**   | *LongShine AI Research* - Proprietary                        | 2025-07-14 |
| AskData + GPT-4o   | **75.36**  | 77.14       | *AT&T CDO - DSAIR* - ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) [[Paper](https://arxiv.org/pdf/2505.19988)] | 2025-03-11 |
| CHASE-SQL + Gemini | 74.90      | 76.02       | *Google Cloud* - ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) [[Paper](https://openreview.net/pdf?id=CvGqMD5OtX)] | 2025-04-16 |
| TCDataAgent-SQL    | 74.12      | 75.74       | *Tencent Cloud* - [[Report](https://cloud.tencent.com/developer/article/2537769)] | 2025-05-30 |
| Contextual-SQL     | 73.50      | 75.63       | *Contextual AI* - [[Report](https://contextual.ai/blog/open-sourcing-the-best-local-text-to-sql-system/)] [[Code](https://github.com/ContextualAI/bird-sql)] | 2025-02-27 |
| XiYan-SQL          | 73.34      | 75.63       | *Alibaba Cloud* - ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) [[Paper](https://arxiv.org/pdf/2411.08599)] [[Code](https://github.com/XGenerationLab/XiYan-SQL)] | 2024-12-17 |

</div>

| Date       | Method/Model       | Dev EX (%) | Test EX (%) | Institute - Paper/Code                                       |
| ---------- | ------------------ | ---------- | ----------- | ------------------------------------------------------------ |
| 2025-07-14 | LongData-SQL       | 74.32      | **77.53**   | *LongShine AI Research* - Proprietary                        |
| 2025-03-11 | AskData + GPT-4o   | **75.36**  | 77.14       | *AT&T CDO - DSAIR* - ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) [[Paper](https://arxiv.org/pdf/2505.19988)] |
| 2025-04-16 | CHASE-SQL + Gemini | 74.90      | 76.02       | *Google Cloud* - ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) [[Paper](https://openreview.net/pdf?id=CvGqMD5OtX)] |
| 2025-05-30 | TCDataAgent-SQL    | 74.12      | 75.74       | *Tencent Cloud* - [[Report](https://cloud.tencent.com/developer/article/2537769)] |
| 2025-02-27 | Contextual-SQL     | 73.50      | 75.63       | *Contextual AI* - [[Report](https://contextual.ai/blog/open-sourcing-the-best-local-text-to-sql-system/)] [[Code](https://github.com/ContextualAI/bird-sql)] |
| 2024-12-17 | XiYan-SQL          | 73.34      | 75.63       | *Alibaba Cloud* - ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) [[Paper](https://arxiv.org/pdf/2411.08599)] [[Code](https://github.com/XGenerationLab/XiYan-SQL)] |

#### [Spider1.0](https://yale-lily.github.io/spider) - Semantic Parsing and Text-to-SQL Challenge

| Date       | Method/Model        | Dev EX (%) | Test EX (%) | Institute - Paper/Code                                       |
| ---------- | ------------------- | ---------- | ----------- | ------------------------------------------------------------ |
| 2023-11-02 | MiniSeek            | -          | **91.2**    | *Seek AI Labs* - [[Report](https://www.seek.ai/blog/miniseek-first-model-to-surpass-90-accuracy-on-spider-test-benchmark)] |
| 2023-08-20 | DAIL-SQL + GPT-4    | **82.4**   | 86.6        | *Alibaba Group* - ![VLDB2024](https://img.shields.io/badge/VLDB2024-800080) [[Paper](https://www.vldb.org/pvldb/vol17/p1132-gao.pdf)] [[Code](https://github.com/BeachWang/DAIL-SQL)] |
| 2023-04-21 | DIN-SQL + GPT-4     | 74.2       | 85.3        | *University of Alberta* - ![NeurIPS2025](https://img.shields.io/badge/NeurIPS2025-2E8B57) [[Paper](https://openreview.net/pdf?id=p53QDxSIc5)] [[Code](https://github.com/MohammadrezaPourreza/Few-shot-NL2SQL-with-prompting)] |
| 2023-06-01 | C3 + ChatGPT        | 81.8       | 82.3        | *Zhejiang University* - ![arXiv2023](https://img.shields.io/badge/arXiv2023-B31B1B) [[Paper](https://arxiv.org/pdf/2307.07306)] [[Code](https://github.com/bigbigwatermalon/C3SQL)] |
| 2023-02-27 | RESDSQL-3B + NatSQL | 84.1       | 79.9        | *Renmin University of China* - ![AAAI2025](https://img.shields.io/badge/AAAI2025-006400) [[Paper](https://arxiv.org/pdf/2302.05965)] [[Code](https://github.com/RUCKBReasoning/RESDSQL)] |

#### [Spider2.0](https://spider2-sql.github.io/) - Evaluating Language Models on Real-World Enterprise Text-to-SQL Workflows

| Date       | Method/Model                     | Snow Score | Lite Score (%) | Institute - Paper/Code                                       |
| ---------- | -------------------------------- | ---------- | -------------- | ------------------------------------------------------------ |
| 2025-08-07 | AgenticData + Qwen3              | -          | **44.5**       | *Tsinghua University* - ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) [[Paper](https://arxiv.org/pdf/2508.05002)] |
| 2025-05-22 | ReFoRCE + o3                     | **37.11**  | 37.84          | *Hao AI Lab x Snowflake* - ![ICLR2025](https://img.shields.io/badge/ICLR2025Workshop-7CFC00) [[Paper](https://openreview.net/pdf?id=OuFIfDBwQd)] |
| 2025-07-0  | RSL-SQL + o3                     | -          | 33.09          | *HUST VLR Lab* - ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) [[Paper](https://arxiv.org/pdf/2411.00073)] [[Code](https://github.com/Laqcce-cao/RSL-SQL)] |
| 2025-04-27 | LinkAlign + DeepSeek-R1          | -          | 33.09          | *Renmin University of China* - ![EMNLP2025](https://img.shields.io/badge/EMNLP2025-00BFFF) [[Paper](https://arxiv.org/pdf/2503.18596)] [[Code](https://github.com/Satissss/LinkAlign)] |
| 2025-03-16 | Spider-Agent + Claude-3.7-Sonnet | -          | 28.52          | *University of Hong Kong* - ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) [[Paper](https://openreview.net/pdf?id=XmProj9cPs)] [[Code](https://github.com/xlang-ai/Spider2)] |

#### [BIRD-CRITIC](https://bird-critic.github.io/) - Can LLMs Fix User Issues in Real-World Database Applications?

| Date       | Model           | SR (%)    | Institute         |
| ---------- | --------------- | --------- | ----------------- |
| 2025-06-10 | ByteBrain-Agent | **43.33** | *ByteDance x RUC* |
| 2025-09-04 | GPT-5-High      | 34.96     | *OpenAI*          |
| 2025-07-18 | grok-4          | 33.68     | *xAI*             |
| 2025-04-20 | DeepSeek-R1     | 33.51     | *DeepSeek*        |
| 2025-04-20 | o3-Mini         | 33.33     | *OpenAI*          |

#### [BIRD-INTERACT](https://bird-interact.github.io/) - Re-imagining Text-to-SQL Evaluation via Lens of Dynamic Interactions
| Date       | Model/Method      | Reward    | Institute  |
| ---------- | ----------------- | --------- |---------- |
| 2025-08-22 | Gemini-2.5-Pro    | **20.92**  | *Google*    |
| 2025-08-22 | o3-Mini           | 20.27     |  *OpenAI*    |
| 2025-08-22 | Claude-Sonnet-4   | 18.35     | *Anthropic* |
| 2025-08-22 | Qwen-3-Coder-480B | 17.75     | *Qwen Team* |
| 2025-08-22 | DeepSeek-V3       | 15.15     | *DeepSeek*  |

## 🗃️ Datasets

## 🪴 Taxonomy

The text-to-SQL methods are carefully categorized based on our paper.

### In-context Learning

### Fine-tuning

## 📃 Citation

```
@article{hong2024next,
  title={Next-generation database interfaces: A survey of llm-based text-to-sql},
  author={Hong, Zijin and Yuan, Zheng and Zhang, Qinggang and Chen, Hao and Dong, Junnan and Huang, Feiran and Huang, Xiao},
  journal={IEEE Transactions on Knowledge and Data Engineering},
  year={2025}
}
```

