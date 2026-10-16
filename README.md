# Awesome-Semantic-Data-Processing

A curated list of research papers on semantic operators, query optimization, execution strategies, and LLM-powered data systems.

## Surveys & Tutorials

- [Semantic Data Processing with Large Language Models: A Survey](https://www.preprints.org/manuscript/202608.1168)（Preprints.org 2026；Survey；Semantic Data Processing）
- [A Survey of LLM-Powered Question Answering Through the Lens of Query Processing](https://www.preprints.org/manuscript/202606.1165)（Preprints.org 2026；Survey；Query Processing & Planning）
- [Large Language Models in Database Management System Optimization: A Survey](https://doi.org/10.1145/3829078)（ACM TIST 2026；Survey；Related: LLM-assisted DBMS Optimization）
- [Data+AI: LLM4Data and Data4LLM](https://doi.org/10.1145/3722212.3725641)（SIGMOD Companion 2025；Tutorial）

## 1. 通用语义算子与端到端系统（Systems & Operators）

- [Aryn - The Design of an LLM-powered Unstructured Analytics System](https://vldb.org/cidrdb/2025/the-design-of-an-llm-powered-unstructured-analytics-system.html)（CIDR 2025）
- [FlockMTL - Beyond Quacking: Deep Integration of Language Models and RAG into DuckDB](https://www.vldb.org/pvldb/vol18/p5415-mhedhbi.pdf)（PVLDB 2025；Demo；基于：DuckDB）
- [iPDB - iPDB: Optimizing SQL Queries with ML and LLM Predicates](https://arxiv.org/abs/2601.16432)（arXiv 2026；基于：DuckDB）
- [Sema - Sema: A High-performance System for LLM-based Semantic Query Processing](https://www.vldb.org/pvldb/vol19/p3231-zhao.pdf)（PVLDB 2026；基于：DuckDB）
- [Palimpzest - Palimpzest: Optimizing AI-Powered Analytics with Declarative Query Processing](https://www.vldb.org/cidrdb/2025/palimpzest-optimizing-ai-powered-analytics-with-declarative-query-processing.html)（CIDR 2025）
  - [Palimpzest - A Declarative System for Optimizing AI Workloads](https://arxiv.org/abs/2405.14696)（arXiv 2024；Technical Report）
- [LOTUS - Semantic Operators and Their Optimization: Enabling LLM-Based Data Processing with Accuracy Guarantees in LOTUS](https://www.vldb.org/pvldb/vol18/p4171-patel.pdf)（PVLDB 2025）
- [UQE - UQE: A Query Engine for Unstructured Databases](https://proceedings.neurips.cc/paper_files/paper/2024/hash/34b3a40ec9752c1ae48fe85fef8fe8dc-Abstract-Conference.html)（NeurIPS 2024）
- [SABER - SABER: A SQL-Compatible Semantic Document Processing System Based on Extended Relational Algebra](https://arxiv.org/abs/2509.00277)（arXiv 2025）
- [Cortex AISQL - Cortex AISQL: A Production SQL Engine for Unstructured Data](https://doi.org/10.1145/3788853.3803093)（SIGMOD Companion 2026；Industry；Snowflake）
- [AnDB - AnDB: Breaking Boundaries with an AI-Native Database for Universal Semantic Analysis](https://arxiv.org/abs/2502.13805)（arXiv 2025）
- [Unify - Unify: An Unstructured Data Analytics System](https://doi.org/10.1109/ICDE65448.2025.00374)（ICDE 2025；Research）
  - [Unify - Unify: A System for Unstructured Data Analytics](https://www.vldb.org/pvldb/vol18/p5287-wang.pdf)（PVLDB 2025；Demo）
- [SEMA-SQL - SEMA-SQL: Beyond Traditional Relational Querying with Large Language Models](https://arxiv.org/abs/2604.23477)（arXiv 2026）
- [OmniTQA - OmniTQA: A Cost-Aware System for Hybrid Query Processing over Semi-Structured Data](https://arxiv.org/abs/2604.02444)（arXiv 2026）
- [KEN - KEN: An Execution Engine for Unstructured Database Systems](https://www.vldb.org/pvldb/vol19/p902-kossmann.pdf)（PVLDB 2026）
- [ELEET - ELEET: Efficient Learned Query Execution over Text and Tables](https://www.vldb.org/pvldb/vol17/p4867-urban.pdf)（PVLDB 2024）

## 2. 语义查询优化（Semantic Query Optimization）

- [Abacus - Abacus: A Cost-Based Optimizer for Semantic Operator Systems](https://www.vldb.org/pvldb/vol19/p1060-russo.pdf)（PVLDB 2026；基于：Palimpzest）
- [Nirvana - Beyond Relational: Semantic-Aware Multi-Modal Analytics with LLM-Native Query Optimization](https://arxiv.org/abs/2511.19830)（SIGMOD 2026）
- [PLOP - PLOP: Cost-Based Placement of Semantic Operators in Hybrid Query Plans](https://arxiv.org/abs/2604.09944)（arXiv 2026；基于：DuckDB）
- [QUEST - QUEST: Query Optimization in Unstructured Document Analysis](https://www.vldb.org/pvldb/vol18/p4560-chai.pdf)（PVLDB 2025；相关 Demo：DocDB）
- [DocETL - DocETL: Agentic Query Rewriting and Evaluation for Complex Document Processing](https://www.vldb.org/pvldb/vol18/p3035-shankar.pdf)（PVLDB 2025）
- [MOAR - Multi-Objective Agentic Rewrites for Unstructured Data Processing](https://www.vldb.org/pvldb/vol19/p3062-shankar.pdf)（PVLDB 2026；基于：DocETL）
- [STRETTO - The Stretto Execution Engine for Semantic Data Systems](https://arxiv.org/abs/2602.04430)（arXiv 2026）
- [KathDB-FAO - KathDB-FAO: Synthesized Query Plans in a Multimodal DBMS](https://arxiv.org/abs/2609.28761)（arXiv 2026；基于：KathDB）
- [When Plans Change Answers: Formalizing Cost-Accuracy Optimization for Semantic Queries](https://arxiv.org/abs/2610.08089)（arXiv 2026）
- [Larch - Larch: Learned Query Optimization for Semantic Predicates](https://arxiv.org/abs/2606.07923)（arXiv 2026）
- [ThalamusDB - ThalamusDB: Approximate Query Processing on Multi-Modal Data](https://doi.org/10.1145/3654989)（SIGMOD 2024；基于：DuckDB）
- [SemStats - Bridging the Gap: Cardinality Estimation for Semantic Queries on Unstructured Data](https://doi.org/10.1145/3802024)（SIGMOD 2026）
- [Galois - Logical and Physical Optimizations for SQL Query Execution over Large Language Models](https://doi.org/10.1145/3725411)（SIGMOD 2025）
- [CADENZA - Compiling Natural-Language Intent into Task-Specific Operator DAGs for Semantic Query Processing](https://arxiv.org/abs/2606.29151)（SIGMOD 2027；Research；已接收）
  - [CADENZA in Action - Breaking the Monolith with Intent-Dependent Plan Spaces for Semantic Queries](https://arxiv.org/abs/2607.01468)（VLDB 2026；Demo；基于：CADENZA）

## 3. 语义算子实现与执行加速（Operator Implementation & Execution）

- [JEVDB - Prune First, Decide Fast: Scalable Semantic Query Processing with JEVDB](https://arxiv.org/abs/2610.02046)（arXiv 2026）
- [100x Cost & Latency Reduction: Performance Analysis of AI Query Approximation using Lightweight Proxy Models](https://arxiv.org/abs/2603.15970)（SIGMOD 2026）
- [ScaleDoc - ScaleDoc: Scaling LLM-based Predicates over Large Document Collections](https://github.com/Seurgul/ScaleDoc)（SIGMOD 2026）
- [ScaleLLM - ScaleLLM: A Technique for Scalable LLM-augmented Data Systems](https://2025.sigmod.org/sigmod_demo_papers.shtml)（SIGMOD Companion 2025；Demo）
- [TaskCascades - Task Cascades for Efficient Unstructured Data Processing](https://arxiv.org/abs/2601.05536)（SIGMOD 2026）
- [BARGAIN - Cut Costs, Not Accuracy: LLM-Powered Data Processing with Guarantees](https://arxiv.org/abs/2509.02896)（SIGMOD 2026；集成于：DocETL）
- [OPHR and GGR - Optimizing LLM Queries in Relational Data Analytics Workloads](https://proceedings.mlsys.org/paper_files/paper/2025/hash/b5dc49f44db2fadc5c4d717c57f4a424-Abstract-Conference.html)（MLSYS 2025）
- [SUPG-IT and GAMCAL - Streaming Model Cascades for Semantic SQL](https://arxiv.org/abs/2604.00660)（arXiv 2026）
- [CSV - Beyond Linear LLM Invocation: An Efficient and Effective Semantic Filter Paradigm](https://arxiv.org/abs/2603.04799)（arXiv 2026）
- [HoldUp - Semantic Data Processing with Holistic Data Understanding](https://arxiv.org/abs/2604.02655)（arXiv 2026）
- [FDJ - Featurized-Decomposition Join: Low-Cost Semantic Joins with Guarantees](https://www.vldb.org/pvldb/vol19/p3048-zeighami.pdf)（PVLDB 2026）
- [Implementing Semantic Join Operators Efficiently](https://arxiv.org/abs/2510.08489)（arXiv 2025）
- [JoinML - Accelerating Approximate Analytical Join Queries over Unstructured Data with Statistical Guarantees](https://arxiv.org/abs/2603.16153)（SIGMOD 2026）
- [Access Paths for Efficient Ordering with Large Language Models](https://arxiv.org/abs/2509.00303)（arXiv 2025）
- [ListK - ListK: Semantic ORDER BY and LIMIT K with Listwise Prompting](https://arxiv.org/abs/2603.17223)（arXiv 2026）
- [Selectivity Estimation for Semantic Filters on Image Data](https://arxiv.org/abs/2606.04610)（arXiv 2026）
- [SemBaker - From Interpretation to Compilation: A Compilation-Based Execution Engine for Semantic Operator Systems](https://arxiv.org/abs/2608.06677)（arXiv 2026；适配：Palimpzest、LOTUS、Nirvana、DocETL）
- [SemJoin - SemJoin: Semantic Join Optimization](https://arxiv.org/abs/2606.29532)（NOVAS @ VLDB 2026；Workshop）
- [Low-Latency Semantic Processing with Optimal Prompt-Level Batching](https://github.com/joycequu/prompt-level-batching)（NOVAS @ VLDB 2026；Workshop；链接为项目仓库）

## 4. 基准测试与工作负载（Benchmarks & Workloads）

- [Bench-U / UDABench - Unstructured Data Analysis using LLMs: A Comprehensive Benchmark](https://www.vldb.org/pvldb/vol19/p2398-deng.pdf)（VLDB 2026 Volume 19, Issue 9）
- [LROBench - Large Language Model-Enhanced Relational Operators: Taxonomy, Benchmark, and Analysis](https://arxiv.org/abs/2603.02537)（arXiv 2026）
- [SemBench - SemBench: A Benchmark for Semantic Query Processing Engines](https://www.vldb.org/pvldb/vol19/p1754-trummer.pdf)（PVLDB 2026）
- [TAG - Text2SQL is Not Enough: Unifying AI and Databases with TAG](https://www.vldb.org/cidrdb/2025/text2sql-is-not-enough-unifying-ai-and-databases-with-tag.html)（CIDR 2025）
- [SWAN - Hybrid Querying Over Relational Databases and Large Language Models](https://www.vldb.org/cidrdb/2025/hybrid-querying-over-relational-databases-and-large-language-models.html)（CIDR 2025）
- [FDABench - FDABench: A Benchmark for Data Agents on Analytical Queries over Heterogeneous Data](https://fdabench.github.io/)（KDD 2026）
- [DAB - Can ai agents answer your data questions? a benchmark for data agents](https://arxiv.org/abs/2603.20576)（arXiv 2026）
- [SemCEB - SemCEB: A Cardinality Estimation Benchmark for Semantic Operators](https://arxiv.org/abs/2606.23081)（NOVAS @ VLDB 2026）

## 5. 相关系统与基础研究（Related Systems & Foundations）

- [VectraFlow - VectraFlow: Long-Horizon Semantic Processing over Data and Event Streams with LLMs](https://arxiv.org/abs/2604.03855)（arXiv 2026）
- [ZenDB - Querying Templatized Document Collections with Large Language Models](https://doi.org/10.1109/ICDE65448.2025.00183)（ICDE 2025）
- [AOP - AOP: Automated and Interactive LLM Pipeline Orchestration for Answering Complex Queries](https://vldb.org/cidrdb/2025/aop-automated-and-interactive-llm-pipeline-orchestration-for-answering-complex-queries.html)（CIDR 2025）
- [SUQL - SUQL: Conversational search over structured and unstructured data with large language models](https://aclanthology.org/2024.findings-naacl.283/)（Findings of NAACL 2024）
- [Evaporate - Language Models Enable Simple Systems for Generating Structured Views of Heterogeneous Data Lakes](https://www.vldb.org/pvldb/vol17/p92-arora.pdf)（PVLDB 2023；VLDB 2024）
- [DocWrangler - Steering Semantic Data Processing With DocWrangler](https://arxiv.org/abs/2504.14764)（UIST 2025；基于：DocETL）
- [PalimpChat - PalimpChat: Declarative and Interactive AI analytics](https://arxiv.org/abs/2502.03368)（SIGMOD Companion 2025；Demo；基于：Palimpzest）
- [DocDB - DocDB: A Database for Unstructured Document Analysis](https://www.vldb.org/pvldb/vol18/p5387-chai.pdf)（PVLDB 2025；Demo；相关系统：QUEST）
- [iDataLake - iDataLake: An LLM-Powered Analytics System on Data Lakes](https://dbgroup.cs.tsinghua.edu.cn/ligl/papers/iDataLake.pdf)（DEB 2025）
- [Databases unbound: Querying all of the world’s bytes with AI](https://www.vldb.org/pvldb/vol17/p4546-madden.pdf)（PVLDB 2024）
- [KathDB - KathDB: Explainable Multimodal Database Management System with Human-AI Collaboration](https://www.vldb.org/cidrdb/2026/kathdb-explainable-multimodal-database-management-system-with-human-ai-collaboration.html)（CIDR 2026）
- [Data Agent - Data Agent: A Holistic Architecture for Orchestrating Data+AI Ecosystems](https://arxiv.org/abs/2507.01599)（DEB 2025）
- [CAESURA - CAESURA: Language Models as Multi-Modal Query Planners](https://www.vldb.org/cidrdb/2024/caesura-language-models-as-multi-modal-query-planners.html)（CIDR 2024）
- [Symphony - Symphony: Towards Natural Language Query Answering over Multi-modal Data Lakes](https://vldb.org/cidrdb/2023/symphony-towards-natural-language-query-answering-over-multi-modal-data-lakes.html)（CIDR 2023）
- [Pneuma - Pneuma: Leveraging LLMs for Tabular Data Representation and Retrieval in an End-to-End System](https://arxiv.org/abs/2504.09207)（SIGMOD 2025）
- [Solo - Solo: Data discovery using natural language questions via a self-supervised approach](https://doi.org/10.1145/3626756)（SIGMOD 2024）
- [AgenticScholar - AgenticScholar: Agentic Data Management with Pipeline Orchestration for Scholarly Corpora](https://arxiv.org/abs/2603.13774)（SIGMOD 2026）
- [NL2Pipe - Bridge the Last-Mile Gap to Semantic Analytics: Compiling Natural-Language Queries into Semantic Operator Pipelines](https://arxiv.org/abs/2606.04641)（arXiv 2026）
- [SIC - Semantic Integrity Constraints: Declarative Guardrails for AI-Augmented Data Processing Systems](https://www.vldb.org/pvldb/vol18/p4073-lee.pdf)（PVLDB 2025）
- [Deep Research is the New Analytics System: Towards Building the Runtime for AI-Driven Analytics](https://www.cidrdb.org/cidr2026/program.html)（CIDR 2026）
- [Information extraction](https://doi.org/10.1561/1900000003)（FNTDB 2008）
- [Large language models for generative information extraction: A survey](https://doi.org/10.1007/s11704-024-40555-y)（FCS 2024）
- [Openie6: Iterative grid labeling and coordination analysis for open information extraction](https://aclanthology.org/2020.emnlp-main.306/)（EMNLP 2020）
- [Text-to-table: A new way of information extraction](https://aclanthology.org/2022.acl-long.180/)（ACL 2022）
- [FrugalGPT: How to Use Large Language Models While Reducing Cost and Improving Performance](https://arxiv.org/abs/2305.05176)（TMLR 2024）
- [ThriftLLM - ThriftLLM: On Cost-Effective Selection of Large Language Models for Classification Queries](https://www.vldb.org/pvldb/vol18/p4410-huang.pdf)（PVLDB 2025）
- [SUPG - Approximate selection with guarantees using proxies](https://www.vldb.org/pvldb/vol13/p1990-kang.pdf)（VLDB 2020）
- [SMART - Smart: Automatically scaling down language models with accuracy guarantees for reduced processing fees](https://arxiv.org/abs/2403.13835)（arXiv 2024）
- [CascadeServe - Cascadeserve: Unlocking model cascades for inference serving](https://arxiv.org/abs/2406.14424)（arXiv 2024）
- [SPEAR - Making Prompts First-Class Citizens for Adaptive LLM Pipelines](https://www.vldb.org/cidrdb/2026/making-prompts-first-class-citizens-for-adaptive-llm-pipelines.html)（CIDR 2026）
- [Predicate Migration - Predicate migration: Optimizing queries with expensive predicates](https://doi.org/10.1145/170035.170078)（SIGMOD 1993）
- [Optimization of queries with user-defined predicates](https://doi.org/10.1145/320248.320249)（TODS 1999）
- [Bypass Processing - Optimizing disjunctive queries with expensive predicates](https://doi.org/10.1145/191843.191906)（SIGMOD 1994）
- [Cost estimation of user-defined methods in object-relational database systems](https://dblp.org/rec/journals/sigmod/BoulosO99)（SIGMOD Record 1999）
- [Batch prompting: Efficient inference with large language model apis](https://aclanthology.org/2023.emnlp-industry.74/)（EMNLP Industry 2023）
- [BatchPrompt - Batchprompt: Accomplish more with less](https://proceedings.iclr.cc/paper_files/paper/2024/hash/5d8c01de2dc698c54201c1c7d0b86974-Abstract-Conference.html)（ICLR 2024）
- [CUCB-SC and CLCB-SC-LS - Semantic Caching for Low-Cost LLM Serving: From Offline Learning to Online Adaptation](https://arxiv.org/abs/2508.07675)（INFOCOM 2026）
- [AgenticData - AgenticData: An Agentic Data Analytics System for Heterogeneous Data](https://arxiv.org/abs/2508.05002)（arXiv 2025）
- [SEED - SEED: Domain-specific data curation with large language models](https://arxiv.org/abs/2310.00749)（arXiv 2023）
- [CPs - Continuous Prompts: LLM-Augmented Pipeline Processing over Unstructured Streams](https://arxiv.org/abs/2512.03389)（arXiv 2025）
- [Doctopus - Doctopus: Budget-aware Structural Table Extraction from Unstructured Documents](https://www.vldb.org/pvldb/vol18/p3695-chai.pdf)（PVLDB 2025）
- [ReDD - Relational Deep Dive: Error-Aware Queries Over Unstructured Data](https://doi.org/10.14778/3811243.3811256)（PVLDB 2026）
- [NOMA - Rethinking Query Optimization for Multi-Agent Systems](https://arxiv.org/abs/2512.11001)（PVLDB 2027；Vision）
- [Expanding the Physical Design Space of LLM Data Systems](https://www.eurecom.edu/en/publication/8925)（IEEE Data Engineering Bulletin 2026；Perspective）