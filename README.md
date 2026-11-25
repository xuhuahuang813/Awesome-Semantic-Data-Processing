# Awesome-Semantic-Data-Processing

A curated list of research papers on LLM-powered semantic data processing: systems and operators, query optimization, execution, benchmarks, streaming, and reliability.

收录范围：利用 LLM/ML 解释数据内容、执行自然语言谓词或语义转换的查询与分析，包括语义过滤、映射/抽取、连接、排序和聚合，以及关系算子与语义算子的混合执行。技术基础单列，仅保留直接支撑这些方法的代理选择、模型级联、批处理和昂贵谓词优化研究；通用 Text-to-SQL、DBMS 调优、数据发现、NLP 抽取和模型服务不单独收录。

## Surveys

- [Semantic Data Processing with Large Language Models: A Survey](https://www.preprints.org/manuscript/202608.1168)（Preprints.org 2026；Survey；Semantic Data Processing）
- [A Survey of LLM-Powered Question Answering Through the Lens of Query Processing](https://www.preprints.org/manuscript/202606.1165)（Preprints.org 2026；Survey；Query Processing & Planning）

## 1. 通用语义算子与端到端系统（Systems & Operators）

### 1.1 语义查询引擎与混合分析

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
- [NousDB - A Fast Query Engine for Semantic Analytics](https://arxiv.org/abs/2610.28551)（arXiv 2026；基于：Apache DataFusion）
- [ThalamusDB - ThalamusDB: Approximate Query Processing on Multi-Modal Data](https://doi.org/10.1145/3654989)（SIGMOD 2024；基于：DuckDB）
- [ZenDB - Querying Templatized Document Collections with Large Language Models](https://doi.org/10.1109/ICDE65448.2025.00183)（ICDE 2025）
- [SUQL - SUQL: Conversational search over structured and unstructured data with large language models](https://aclanthology.org/2024.findings-naacl.283/)（Findings of NAACL 2024）
- [BlendSQL - BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra](https://aclanthology.org/2024.findings-acl.25/)（Findings of ACL 2024；基于：SQLite）
- [iDataLake - iDataLake: An LLM-Powered Analytics System on Data Lakes](https://dbgroup.cs.tsinghua.edu.cn/ligl/papers/iDataLake.pdf)（DEB 2025）
- [KathDB - KathDB: Explainable Multimodal Database Management System with Human-AI Collaboration](https://www.vldb.org/cidrdb/2026/kathdb-explainable-multimodal-database-management-system-with-human-ai-collaboration.html)（CIDR 2026）
- [Meta Engine - Beyond Single-Modal Analytics: A Framework for Integrating Heterogeneous LLM-Based Query Systems for Multi-Modal Data](https://arxiv.org/abs/2602.01701)（arXiv 2026）

### 1.2 自然语言规划与分析流水线

- [AOP - AOP: Automated and Interactive LLM Pipeline Orchestration for Answering Complex Queries](https://vldb.org/cidrdb/2025/aop-automated-and-interactive-llm-pipeline-orchestration-for-answering-complex-queries.html)（CIDR 2025）
- [CAESURA - CAESURA: Language Models as Multi-Modal Query Planners](https://www.vldb.org/cidrdb/2024/caesura-language-models-as-multi-modal-query-planners.html)（CIDR 2024）
- [Symphony - Symphony: Towards Natural Language Query Answering over Multi-modal Data Lakes](https://vldb.org/cidrdb/2023/symphony-towards-natural-language-query-answering-over-multi-modal-data-lakes.html)（CIDR 2023）
- [AgenticData - AgenticData: An Agentic Data Analytics System for Heterogeneous Data](https://arxiv.org/abs/2508.05002)（arXiv 2025）
- [AgenticScholar - AgenticScholar: Agentic Data Management with Pipeline Orchestration for Scholarly Corpora](https://arxiv.org/abs/2603.13774)（SIGMOD 2026）

### 1.3 文档抽取与数据整理

- [Evaporate - Language Models Enable Simple Systems for Generating Structured Views of Heterogeneous Data Lakes](https://www.vldb.org/pvldb/vol17/p92-arora.pdf)（PVLDB 2023；VLDB 2024）
- [SEED - SEED: Domain-specific data curation with large language models](https://arxiv.org/abs/2310.00749)（arXiv 2023）
- [Doctopus - Doctopus: Budget-aware Structural Table Extraction from Unstructured Documents](https://www.vldb.org/pvldb/vol18/p3695-chai.pdf)（PVLDB 2025）

### 1.4 交互与系统演示

- [DocWrangler - Steering Semantic Data Processing With DocWrangler](https://arxiv.org/abs/2504.14764)（UIST 2025；基于：DocETL）
- [PalimpChat - PalimpChat: Declarative and Interactive AI analytics](https://arxiv.org/abs/2502.03368)（SIGMOD Companion 2025；Demo；基于：Palimpzest）
- [DocDB - DocDB: A Database for Unstructured Document Analysis](https://www.vldb.org/pvldb/vol18/p5387-chai.pdf)（PVLDB 2025；Demo；相关系统：QUEST）

## 2. 语义查询优化（Semantic Query Optimization）

### 2.1 计划生成、重写与代价—质量优化

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
- [Galois - Logical and Physical Optimizations for SQL Query Execution over Large Language Models](https://doi.org/10.1145/3725411)（SIGMOD 2025）
- [CADENZA - Compiling Natural-Language Intent into Task-Specific Operator DAGs for Semantic Query Processing](https://arxiv.org/abs/2606.29151)（SIGMOD 2027；Research；已接收）
  - [CADENZA in Action - Breaking the Monolith with Intent-Dependent Plan Spaces for Semantic Queries](https://arxiv.org/abs/2607.01468)（VLDB 2026；Demo；基于：CADENZA）
- [NL2Pipe - Bridge the Last-Mile Gap to Semantic Analytics: Compiling Natural-Language Queries into Semantic Operator Pipelines](https://arxiv.org/abs/2606.04641)（arXiv 2026）

### 2.2 基数与选择率估计

- [SemStats - Bridging the Gap: Cardinality Estimation for Semantic Queries on Unstructured Data](https://doi.org/10.1145/3802024)（SIGMOD 2026）
- [Selectivity Estimation for Semantic Filters on Image Data](https://arxiv.org/abs/2606.04610)（arXiv 2026）

### 2.3 跨查询复用与语义视图

- [Semantic Views: Certified Reuse of LLM Labels Across Semantic Queries](https://arxiv.org/abs/2610.12768)（arXiv 2026）
- [Demo of SemWeave: Semantic Common Expressions for LLM-powered Query Processing](https://dl.acm.org/doi/epdf/10.1145/3788853.3801593)（SIGMOD Companion 2026；Demo）
- [SemReuse: Certified Reuse of Cached Natural-Language Views for Semantic Operators](https://arxiv.org/abs/2610.16035)（arXiv 2026）
- [OCTOPUS - OCTOPUS: Towards A Tag Model for Cross-Query Reuse in Semantic Query Processing](https://arxiv.org/abs/2610.32586)（arXiv 2026）

## 3. 语义算子实现与执行加速（Operator Implementation & Execution）

### 3.1 语义过滤与模型级联

- [JEVDB - Prune First, Decide Fast: Scalable Semantic Query Processing with JEVDB](https://arxiv.org/abs/2610.02046)（arXiv 2026）
- [100x Cost & Latency Reduction: Performance Analysis of AI Query Approximation using Lightweight Proxy Models](https://arxiv.org/abs/2603.15970)（SIGMOD 2026）
- [ScaleDoc - ScaleDoc: Scaling LLM-based Predicates over Large Document Collections](https://github.com/Seurgul/ScaleDoc)（SIGMOD 2026）
- [Oasis - Towards Online Adaptive LLM-based Semantic Filtering](https://arxiv.org/abs/2611.24518)（arXiv 2026）
- [ScaleLLM - ScaleLLM: A Technique for Scalable LLM-augmented Data Systems](https://2025.sigmod.org/sigmod_demo_papers.shtml)（SIGMOD Companion 2025；Demo）
- [TaskCascades - Task Cascades for Efficient Unstructured Data Processing](https://arxiv.org/abs/2601.05536)（SIGMOD 2026）
- [BARGAIN - Cut Costs, Not Accuracy: LLM-Powered Data Processing with Guarantees](https://arxiv.org/abs/2509.02896)（SIGMOD 2026；集成于：DocETL）
- [OPHR and GGR - Optimizing LLM Queries in Relational Data Analytics Workloads](https://proceedings.mlsys.org/paper_files/paper/2025/hash/b5dc49f44db2fadc5c4d717c57f4a424-Abstract-Conference.html)（MLSYS 2025）
- [SUPG-IT and GAMCAL - Streaming Model Cascades for Semantic SQL](https://arxiv.org/abs/2604.00660)（arXiv 2026）
- [CSV - Beyond Linear LLM Invocation: An Efficient and Effective Semantic Filter Paradigm](https://arxiv.org/abs/2603.04799)（arXiv 2026）

### 3.2 语义连接

- [FDJ - Featurized-Decomposition Join: Low-Cost Semantic Joins with Guarantees](https://www.vldb.org/pvldb/vol19/p3048-zeighami.pdf)（PVLDB 2026）
- [Implementing Semantic Join Operators Efficiently](https://arxiv.org/abs/2510.08489)（arXiv 2025）
- [JoinML - Accelerating Approximate Analytical Join Queries over Unstructured Data with Statistical Guarantees](https://arxiv.org/abs/2603.16153)（SIGMOD 2026）
- [SemJoin - SemJoin: Semantic Join Optimization](https://arxiv.org/abs/2606.29532)（NOVAS @ VLDB 2026；Workshop）

### 3.3 语义排序与聚合

- [Access Paths for Efficient Ordering with Large Language Models](https://arxiv.org/abs/2509.00303)（arXiv 2025）
- [ListK - ListK: Semantic ORDER BY and LIMIT K with Listwise Prompting](https://arxiv.org/abs/2603.17223)（arXiv 2026）
- [OLLA - LLM-Driven Online Aggregation for Unstructured Text Analytics](https://arxiv.org/abs/2603.08443)（arXiv 2026）

### 3.4 跨算子执行、编译与批处理

- [HoldUp - Semantic Data Processing with Holistic Data Understanding](https://arxiv.org/abs/2604.02655)（arXiv 2026）
- [SemBaker - From Interpretation to Compilation: A Compilation-Based Execution Engine for Semantic Operator Systems](https://arxiv.org/abs/2608.06677)（arXiv 2026；适配：Palimpzest、LOTUS、Nirvana、DocETL）
- [Low-Latency Semantic Processing with Optimal Prompt-Level Batching](https://github.com/joycequu/prompt-level-batching)（NOVAS @ VLDB 2026；Workshop；链接为项目仓库）
- [Kalypso - Kalypso: Relational LLM Serving](https://arxiv.org/abs/2607.23815)（arXiv 2026）

## 4. 基准测试与实证评测（Benchmarks & Empirical Studies）

### 4.1 语义算子与查询引擎

- [Bench-U / UDABench - Unstructured Data Analysis using LLMs: A Comprehensive Benchmark](https://www.vldb.org/pvldb/vol19/p2398-deng.pdf)（PVLDB 2026） [Code](https://bit-datalab.github.io/bench-u-page/)
- [LROBench - Large Language Model-Enhanced Relational Operators: Taxonomy, Benchmark, and Analysis](https://arxiv.org/abs/2603.02537)（arXiv 2026）
- [SemBench - SemBench: A Benchmark for Semantic Query Processing Engines](https://www.vldb.org/pvldb/vol19/p1754-trummer.pdf)（PVLDB 2026） [Code](https://github.com/SemBench/SemBench/tree/main) [Web](https://sembench.github.io/SemBench/)
- [Same Query, Different Answer: Run-to-Run Variance in Semantic Query Processing](https://arxiv.org/abs/2610.13823)（arXiv 2026）
- [Cascadeability and the Realization Gap: An Empirical Study of LLM-Powered Semantic Filtering](https://arxiv.org/abs/2611.23898)（arXiv 2026）
- [SemCEB - SemCEB: A Cardinality Estimation Benchmark for Semantic Operators](https://arxiv.org/abs/2606.23081)（NOVAS @ VLDB 2026）

### 4.2 混合查询与异构数据分析

覆盖关系数据、模型知识或非结构化数据的联合分析；与语义算子专用基准区分列出。

- [TAG - Text2SQL is Not Enough: Unifying AI and Databases with TAG](https://www.vldb.org/cidrdb/2025/text2sql-is-not-enough-unifying-ai-and-databases-with-tag.html)（CIDR 2025；提出 TAG 范式与 TAG-Bench）
- [SWAN - Hybrid Querying Over Relational Databases and Large Language Models](https://www.vldb.org/cidrdb/2025/hybrid-querying-over-relational-databases-and-large-language-models.html)（CIDR 2025；混合查询基准）
- [HyQBench - Automating End-to-End Hybrid Query Processing: Benchmark, Solution, and Insights](https://dl.acm.org/doi/epdf/10.1145/3770855.3817487)（SIGKDD 2026）
- [FDABench - FDABench: A Benchmark for Data Agents on Analytical Queries over Heterogeneous Data](https://fdabench.github.io/)（KDD 2026）

## 5. 流式语义处理（Streaming Semantic Processing）

- [CPs - Continuous Prompts: LLM-Augmented Pipeline Processing over Unstructured Streams](https://arxiv.org/abs/2512.03389)（arXiv 2025）
- [VectraFlow - VectraFlow: Long-Horizon Semantic Processing over Data and Event Streams with LLMs](https://arxiv.org/abs/2604.03855)（arXiv 2026）

## 6. 可靠性、约束与溯源（Reliability, Constraints & Provenance）

- [SIC - Semantic Integrity Constraints: Declarative Guardrails for AI-Augmented Data Processing Systems](https://www.vldb.org/pvldb/vol18/p4073-lee.pdf)（PVLDB 2025）
- [ReDD - Relational Deep Dive: Error-Aware Queries Over Unstructured Data](https://doi.org/10.14778/3811243.3811256)（PVLDB 2026）
- [Evergreen - Evergreen: Efficient Claim Verification for Semantic Aggregates](https://arxiv.org/abs/2604.26180)（arXiv 2026）

## 7. 技术基础与研究展望（Foundations & Perspectives）

### 7.1 代理选择、模型级联与批处理

以下是语义过滤、模型选择与批量推理的相关技术基础，并非语义查询系统本身。

- [SUPG - Approximate selection with guarantees using proxies](https://www.vldb.org/pvldb/vol13/p1990-kang.pdf)（VLDB 2020）
- [FrugalGPT: How to Use Large Language Models While Reducing Cost and Improving Performance](https://arxiv.org/abs/2305.05176)（TMLR 2024）
- [ThriftLLM - ThriftLLM: On Cost-Effective Selection of Large Language Models for Classification Queries](https://www.vldb.org/pvldb/vol18/p4410-huang.pdf)（PVLDB 2025）
- [SMART - Smart: Automatically scaling down language models with accuracy guarantees for reduced processing fees](https://arxiv.org/abs/2403.13835)（arXiv 2024）
- [Batch prompting: Efficient inference with large language model apis](https://aclanthology.org/2023.emnlp-industry.74/)（EMNLP Industry 2023）
- [BatchPrompt - Batchprompt: Accomplish more with less](https://proceedings.iclr.cc/paper_files/paper/2024/hash/5d8c01de2dc698c54201c1c7d0b86974-Abstract-Conference.html)（ICLR 2024）

### 7.2 昂贵谓词与用户自定义函数优化

传统数据库中有关昂贵谓词的研究，为语义谓词的放置、重排和代价估计提供基础。

- [Predicate Migration - Predicate migration: Optimizing queries with expensive predicates](https://doi.org/10.1145/170035.170078)（SIGMOD 1993）
- [Optimization of queries with user-defined predicates](https://doi.org/10.1145/320248.320249)（TODS 1999）
- [Bypass Processing - Optimizing disjunctive queries with expensive predicates](https://doi.org/10.1145/191843.191906)（SIGMOD 1994）
- [Cost estimation of user-defined methods in object-relational database systems](https://dblp.org/rec/journals/sigmod/BoulosO99)（SIGMOD Record 1999）

### 7.3 研究展望与扩展方向

- [Databases unbound: Querying all of the world’s bytes with AI](https://www.vldb.org/pvldb/vol17/p4546-madden.pdf)（PVLDB 2024）
- [SPEAR - Making Prompts First-Class Citizens for Adaptive LLM Pipelines](https://www.vldb.org/cidrdb/2026/making-prompts-first-class-citizens-for-adaptive-llm-pipelines.html)（CIDR 2026）
- [Deep Research is the New Analytics System: Towards Building the Runtime for AI-Driven Analytics](https://www.cidrdb.org/cidr2026/program.html)（CIDR 2026）
- [NOMA - Rethinking Query Optimization for Multi-Agent Systems](https://arxiv.org/abs/2512.11001)（PVLDB 2027；Vision；扩展：多智能体数据流水线）
- [Expanding the Physical Design Space of LLM Data Systems](https://www.eurecom.edu/en/publication/8925)（IEEE Data Engineering Bulletin 2026；Perspective）
