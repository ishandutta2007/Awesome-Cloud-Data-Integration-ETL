# Awesome-Cloud-Data-Integration-ETL

# Awesome-Cloud-Data-Integration-ETL



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Data Pipelines, ETL/ELT, Connectors & Orchestration*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Data Integration & ETL**. These tools help organizations move data from source systems to cloud data warehouses and lakes, transform it into analytics-ready formats, and orchestrate pipelines at scale.



**Examples** include Azure Data Factory, Fivetran, Stitch, Matillion, Informatica Cloud Data Integration, Talend Cloud, AWS Glue, Google Cloud Dataflow, Hevo Data, and Airbyte (the category leaders).



**Open-source emphasis**: Cloud data integration has a **mature open-source ecosystem**, with **Airbyte** leading connector breadth (300+ connectors) and **Apache Airflow** dominating orchestration. **dbt** has become the standard for transformation-as-code. **Meltano** offers a code-first Singer-based alternative, while **Apache NiFi** and **Kestra** serve visual and declarative orchestration use cases. However, **commercial platforms** (Fivetran, Matillion, Informatica) provide managed connectors, enterprise SLAs, and vendor support that open-source alternatives require significant operational investment to match.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## 📖 Table of Contents



- [☁️ SaaS/Hosted Platforms](#-saas-hosted-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🤝 How to Contribute](#-how-to-contribute)

- [⚠️ Disclaimer](#-disclaimer)



## ☁️ SaaS/Hosted Platforms



> **📊 Market Context**: The global data integration and ETL market is estimated at **~$14.8B in 2026**, growing toward **~$35B by 2031** at a **~18.7% CAGR**. The sector is **moderately fragmented** — Fivetran leads the managed ELT segment with **$600M ARR** and a **$5.87B valuation** , while Matillion ($99M revenue, $1.5B valuation)  and Talend ($140M revenue)  compete in the transformation-heavy enterprise tier. Hevo Data ($46.9M revenue, $281.6M valuation) serves the mid-market . No single vendor holds a winner-take-all position; enterprises typically run multi-vendor stacks combining ingestion (Fivetran/Airbyte), transformation (dbt/Matillion), and orchestration (Airflow).



| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |

|----------|-------------|------------------------|------------------|--------------|

| **[Fivetran](https://www.fivetran.com/)** | Fully managed ELT platform with 700+ connectors. Automated schema drift handling, log-based replication, and minimal configuration. | **$5/month minimum per connection** . Consumption-based pricing tied to Monthly Active Rows (MAR). Annual commits discount spend rates 5–36% . | **14-day free trial** with all connectors. **Free plan**: Unlimited connections, 500,000 MAR/month, 14-day free use per new connection after initial sync . | **$5.87B valuation, $600M ARR, $985M raised**  |

| **[Matillion](https://www.matillion.com/)** | Enterprise ELT/ETL platform with robust transformation capabilities. Native dbt integration, no-code and high-code options. | **Basic: $1,000/month** (from third-party listing); **Advanced: $2,000/month** . Consumption-based DPU pricing; annual contracts typical. | **30-day free trial** available. **No perpetual free tier** for paid plans. | **$1.5B valuation, $99M revenue, $365.7M raised**  |

| **[Stitch](https://www.stitchdata.com/)** | Cloud-first ETL platform (owned by Talend/Qlik). Focused on data replication from SaaS sources to warehouses. | **Standard: $100/month** for 10M rows; **Advanced: $1,500/month** (annual) for 100M rows; **Premium: $3,000/month** (annual) for 1B rows . | **Free plan**: Up to **5 integrations**, **5 million total rows per billing period** . **14-day free trial** of Standard plan . | **Part of Qlik/Talend ($140M revenue)**  |

| **[Hevo Data](https://hevodata.com/)** | Fully managed ELT platform with 150+ connectors. Near real-time replication with automated pipeline management. | **Starter: $1/credit** (starts at **$299/month**); **Professional: $1.50/credit** (starts at **$549/month**); **Business Critical: $2/credit** . Credits consumed per million events. | **Free plan**: Up to **1 million events/month** for limited connectors, unlimited pipelines, up to 5 users . **14-day free trial** with 24x7 support . | **$281.6M valuation, $46.9M revenue, $43M raised**  |

| **[AWS Glue](https://aws.amazon.com/glue/)** | Serverless ETL service on AWS. Native integration with S3, Redshift, and the AWS ecosystem. | **$0.44 per DPU-hour** (Data Processing Unit). Billed across six separately metered components: DPU-hours, Catalog objects, Catalog requests, interactive sessions, crawler runtime, and DataBrew sessions . | **AWS Free Tier**: 1 million Data Catalog objects and 1 million requests free per month. No perpetual free tier for Glue jobs. | **~$638B revenue (Amazon FY2025)** |

| **[Azure Data Factory](https://azure.microsoft.com/en-us/products/data-factory/)** | Microsoft's cloud data integration service. 100+ connectors, mapping data flows, and SSIS integration. | **Data Pipeline Orchestration**: ~$0.005/hour per activity run. **Data Flows**: ~$0.276/hour per vCore. **Integration Runtime**: From ~$0.10/hour. | **Azure free account**: **$200 credit for 30 days** + **12 months of free services**. No perpetual free tier for Data Factory. | **~$281B revenue (Microsoft FY2025)** |

| **[Google Cloud Dataflow](https://cloud.google.com/products/dataflow)** | Google's managed service for Apache Beam pipelines. Unified batch and streaming processing. | **vCPU/hour** and **GB/hour** pricing. **Committed Use Discounts (CUDs)**: **20% discount for 1-year** commitment, **40% for 3-year** . | **Google Cloud Free Tier**: **$300 credit for 90 days**. No perpetual free tier for Dataflow. | **~$350B revenue (Alphabet FY2025)** |

| **[Informatica Cloud Data Integration](https://www.informatica.com/)** | Enterprise iPaaS with cloud and on-premises deployment. Broad connectivity including SAP and Mainframe. | **Quote-based pricing**. IDMC uses **IPU (Informatica Processing Unit)** consumption model. Legacy PowerCenter uses perpetual licensing + 20–22% annual maintenance . | **Free 30-day trial** available. **Free tier** for basic data integration tasks via Informatica Intelligent Cloud Services. | **~$1.6B revenue, private (taken private by Permira, 2024)** |

| **[Talend Cloud](https://www.talend.com/)** | Unified data integration and data quality platform. Now part of Qlik. | **Quote-based pricing**. **Starter, Standard, Premium, Enterprise** editions . Consumption measured by data volume, job executions, and duration . | **Free trial** available. **No perpetual free tier** for enterprise editions. | **$140M revenue, part of Qlik**  |

| **[Airbyte Cloud](https://airbyte.com/)** | Fully managed cloud version of the leading open-source ELT platform. 300+ connectors. | **Standard: $20/month** (5 credits included); **Plus: $189/month** (40 credits); **Pro** and **Enterprise Flex** custom . Extra credits **$5 each** . | **Free Community Edition** (self-hosted). **Cloud**: 14-day free trial. **No perpetual free tier** for managed cloud. | **$1.5B valuation, $181M raised (private)** |



## 🔓 Open-Source GitHub Projects



Sorted by star count (descending). Star badge links to each repo's stargazers page.



| Repo | Description | Stars |

|---|---|---|

| **[Apache Airflow](https://github.com/apache/airflow)** — The de facto standard for programmatic workflow orchestration. Python DAGs, rich UI, extensive provider ecosystem. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/apache/airflow?style=social&color=white)](https://github.com/apache/airflow/stargazers) | ~38,000 |

| **[Airbyte](https://github.com/airbytehq/airbyte)** — Leading open-source ELT platform with **300+ connectors**. Full data replication and normalization. AGPL-3.0 (with commercial license for enterprise). | [![Stars](https://img.shields.io/github/stars/airbytehq/airbyte?style=social&color=white)](https://github.com/airbytehq/airbyte/stargazers) | ~18,000 |

| **[dbt Core](https://github.com/dbt-labs/dbt-core)** — The standard for SQL-based transformation. Modular SQL, version control, testing, and documentation. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/dbt-labs/dbt-core?style=social&color=white)](https://github.com/dbt-labs/dbt-core/stargazers) | ~11,000 |

| **[Apache NiFi](https://github.com/apache/nifi)** — Visual data flow orchestration with drag-and-drop interface. Strong for IoT, streaming, and enterprise integration. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/apache/nifi?style=social&color=white)](https://github.com/apache/nifi/stargazers) | ~5,300 |

| **[Meltano](https://github.com/meltano/meltano)** — Code-first data integration engine built on Singer. Declarative YAML pipelines, CLI-driven, Git-friendly. MIT. | [![Stars](https://img.shields.io/github/stars/meltano/meltano?style=social&color=white)](https://github.com/meltano/meltano/stargazers) | ~1,900 |

| **[Kestra](https://github.com/kestra-io/kestra)** — Declarative orchestration platform for data, AI, and infrastructure workflows. YAML-based, language-agnostic, event-driven. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/kestra-io/kestra?style=social&color=white)](https://github.com/kestra-io/kestra/stargazers) | ~18,000 |

| **[Apache Hop](https://github.com/apache/hop)** — Orchestration and data engineering platform. Visual pipeline designer, metadata-driven, Hadoop/Spark support. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/apache/hop?style=social&color=white)](https://github.com/apache/hop/stargazers) | ~800 |



**Additional open-source options worth exploring:**



| Repo | Description |

|---|---|

| **[Dagster](https://github.com/dagster-io/dagster)** — Data orchestrator for machine learning, analytics, and ETL. Asset-based programming model. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/dagster-io/dagster?style=social&color=white)](https://github.com/dagster-io/dagster/stargazers) |

| **[Prefect](https://github.com/PrefectHQ/prefect)** — Modern workflow orchestration framework. Python-native, hybrid execution model. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/PrefectHQ/prefect?style=social&color=white)](https://github.com/PrefectHQ/prefect/stargazers) |

| **[Apache SeaTunnel](https://github.com/apache/seatunnel)** — High-performance data integration platform for massive data. 100+ connectors. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/apache/seatunnel?style=social&color=white)](https://github.com/apache/seatunnel/stargazers) |

| **[Flink CDC](https://github.com/apache/flink-cdc)** — Streaming data integration with exactly-once semantics. MySQL, PostgreSQL, Oracle, MongoDB. Apache-2.0. | [![Stars](https://img.shields.io/github/stars/apache/flink-cdc?style=social&color=white)](https://github.com/apache/flink-cdc/stargazers) |



## 🤝 How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Data integration platforms handle sensitive organizational data; ensure compliance with data protection regulations and internal security policies.

- **Open-source reality**: The open-source ecosystem for data integration is **mature and production-proven** at the **ingestion layer** (**Airbyte**, 300+ connectors) and **transformation layer** (**dbt Core**), with **orchestration** covered by **Airflow**, **Dagster**, **Prefect**, and **Kestra**. **Meltano** provides a code-first Singer-based alternative. However, **commercial platforms** (Fivetran, Matillion, Informatica) provide **managed connectors, automated schema drift handling, enterprise SLAs, and vendor support** that open-source alternatives require significant operational investment to match. The open-source path is **genuinely viable** for organizations with strong data platform engineering capacity.

- **Pricing caveat**: All pricing figures above are **verified against cited search results** but may change without notice. Enterprise contracts typically involve volume discounts, multi-year commitments, and bundled pricing that differs significantly from list rates. Always request a formal quote for accurate budgeting.



---



**Made for data engineers, analytics engineers, platform teams, and data architects.**

Let's make data integration more open, transparent, and accessible.
