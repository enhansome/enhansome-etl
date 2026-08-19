# Awesome ETL with stars

A curated list of notable ETL (extract, transform, load) frameworks, libraries and software.

The premise of this list: you don't need fancy, specialized ETL frameworks. Well-structured code using mainstream, well-supported libraries gets you surprisingly far and is easier to test, review, and version control than tools that make those things difficult. Tools here are selected for real-world adoption and staying power, not novelty.

Open source tools are strongly preferred. Proprietary or restrictively licensed tools are only included when they're mainstream enough to be genuinely hard to ignore. See CONTRIBUTING.md for full inclusion criteria.

## Contents

* [Workflow Management/Engines](#workflow-managementengines)
* [Job Scheduling](#job-scheduling)
* [Java](#java)
* [Python](#python)
* [Ruby](#ruby)
* [Go](#go)
* [Cloud Services](#cloud-services)
* [Big Data (Hadoop Stack)](#big-data-hadoop-stack)
* [ETL Tools (GUI)](#etl-tools-gui)
* [Further Reading](#further-reading)

## Workflow Management/Engines

* [Airflow](https://github.com/apache/airflow) ⭐ 46,535 | 🐛 1,895 | 🌐 Python | 📅 2026-08-19 - "Use airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed."
* [prefect](https://github.com/PrefectHQ/prefect) ⭐ 23,641 | 🐛 862 | 🌐 Python | 📅 2026-08-19 - "a workflow orchestration framework for building resilient data pipelines in Python."
* [Luigi](https://github.com/spotify/luigi) ⭐ 18,766 | 🐛 167 | 🌐 Python | 📅 2026-07-18 - "a Python module that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization etc. It also comes with Hadoop support built in."
* [Argo](https://argoproj.github.io/) - "an open source container-native workflow engine for orchestrating parallel jobs on Kubernetes."
* [Dagster](https://dagster.io) - "Dagster is a data orchestrator for machine learning, analytics, and ETL. It lets you define pipelines in terms of the data flow between reusable, logical components, then test locally and run anywhere. With a unified view of pipelines and the assets they produce, Dagster can schedule and orchestrate Pandas, Spark, SQL, or anything else that Python can invoke."
* [Temporal](https://temporal.io) - "a scalable and reliable runtime for durable function executions called Temporal Workflow Executions."
* [Toil](https://toil.readthedocs.io/en/latest/) - "an open-source pure-Python workflow engine that lets people write better pipelines."

## Job Scheduling

* [Jenkins](https://github.com/jenkinsci/jenkins) ⭐ 26,468 | 🐛 3,623 | 🌐 Java | 📅 2026-08-19 - "the leading open-source automation server. Built with Java, it provides over 1000 plugins to support automating virtually anything, so that humans can actually spend their time doing things machines cannot."

## Java

* [Apache Camel](https://github.com/apache/camel) ⭐ 6,291 | 🐛 61 | 🌐 Java | 📅 2026-08-19 - "an open source integration framework that empowers you to quickly and easily integrate various systems consuming or producing data."
* [Spring Batch](https://spring.io/projects/spring-batch) - "A lightweight, comprehensive batch framework designed to enable the development of robust batch applications that are vital for the daily operations of enterprise systems."

## Python

### Libraries

* [polars](https://github.com/pola-rs/polars) ⭐ 39,391 | 🐛 2,860 | 🌐 Rust | 📅 2026-08-19 - "Extremely fast Query Engine for DataFrames, written in Rust."
* [Dask](https://github.com/dask/dask) ⭐ 13,891 | 🐛 1,310 | 🌐 Python | 📅 2026-08-17 - "a flexible parallel computing library for analytics."
* [dbt-core](https://github.com/dbt-labs/dbt-core) ⭐ 13,661 | 🐛 1,528 | 🌐 Rust | 📅 2026-08-19 - "enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications."
* [tenacity](https://github.com/jd/tenacity) ⭐ 8,751 | 🐛 43 | 🌐 Python | 📅 2026-08-06 - "a general-purpose retrying library, written in Python, to simplify the task of adding retry behavior to just about anything."
* [xmltodict](https://github.com/martinblech/xmltodict) ⭐ 5,751 | 🐛 7 | 🌐 Python | 📅 2026-06-15 - "Python module that makes working with XML feel like you are working with JSON."
* [ingestr](https://github.com/bruin-data/ingestr) ⭐ 3,848 | 🐛 15 | 🌐 Go | 📅 2026-08-19 - "a CLI tool to copy data between any databases with a single command seamlessly."
* [lxml](https://github.com/lxml/lxml) ⭐ 3,047 | 🐛 12 | 🌐 Python | 📅 2026-08-18 - "the most feature-rich and easy-to-use library for processing XML and HTML in the Python language."
* [hamilton](https://github.com/DAGWorks-Inc/hamilton) ⭐ 2,569 | 🐛 151 | 🌐 Jupyter Notebook | 📅 2026-08-19 - "helps data scientists and engineers define testable, modular, self-documenting dataflows, that encode lineage/tracing and metadata. Runs and scales everywhere python does."
* [parse](https://github.com/r1chardj0n3s/parse) ⭐ 1,790 | 🐛 38 | 🌐 Python | 📅 2026-08-01 - "Parse strings using a specification based on the Python format() syntax."
* [PETL](https://github.com/petl-developers/petl) ⭐ 1,315 | 🐛 89 | 🌐 Python | 📅 2026-08-05 - "a general purpose Python package for extracting, transforming and loading tables of data."
* [ijson](https://github.com/ICRAR/ijson) ⭐ 1,093 | 🐛 11 | 🌐 Python | 📅 2026-08-10 - "Iterative JSON parser with Pythonic interfaces."
* [BeautifulSoup](http://www.crummy.com/software/BeautifulSoup/) - "a Python library for pulling data out of HTML and XML files."
* [Celery](https://docs.celeryq.dev/) - "an asynchronous task queue/job queue based on distributed message passing. It is focused on real-time operation, but supports scheduling as well."
* [dataset](https://dataset.readthedocs.org/en/latest/) - A wrapper around SQLAlchemy that simplifies database operations (including upserting).
* [dlt](https://dlthub.com/docs) - "an open-source Python library that loads data from various, often messy data sources into well-structured datasets."
* [DuckDB](https://duckdb.org) - "an analytical in-process SQL database management system."
* [Great Expectations](https://docs.greatexpectations.io/) - "a Python library for validating, documenting, and profiling your data to maintain quality and improve communication between teams about data and data pipelines."
* [Joblib](https://joblib.readthedocs.io/) - "a set of tools to provide lightweight pipelining in Python."
* [Meltano](https://meltano.com/) - "the declarative code-first data integration engine."
* [Pandas](http://pandas.pydata.org/) - "Flexible and powerful data analysis / manipulation library for Python, providing labeled data structures similar to R data.frame objects, statistical functions, and much more."
* [PyQuery](https://pyquery.readthedocs.io/) - "A jquery-like library for python."
* [Scrapy](https://scrapy.org) - "a fast high-level web crawling & scraping framework for Python."
* [SQLAlchemy](http://www.sqlalchemy.org/) - "the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL."
* [Toolz](https://toolz.readthedocs.org/en/latest/) - "A functional standard library for Python."

## Ruby

* [nokogiri](https://github.com/sparklemotion/nokogiri) ⭐ 6,276 | 🐛 115 | 🌐 C | 📅 2026-08-14 - "Nokogiri makes it easy and painless to work with XML and HTML from Ruby."
* [Sequel](https://github.com/jeremyevans/sequel) ⭐ 5,092 | 🐛 1 | 🌐 Ruby | 📅 2026-08-19 - "a simple, flexible, and powerful SQL database access toolkit for Ruby."
* [Embulk](https://github.com/embulk/embulk) ⭐ 1,783 | 🐛 162 | 🌐 Java | 📅 2026-06-19 - "a parallel bulk data loader that helps data transfer between various storages, databases, NoSQL and cloud services."
* [Kiba](https://github.com/thbar/kiba) ⭐ 1,775 | 🐛 0 | 🌐 Ruby | 📅 2026-01-10 - "lets you define and run high-quality ETL jobs using Ruby."

## Go

* [CloudQuery](https://github.com/cloudquery/cloudquery) ⭐ 6,484 | 🐛 166 | 🌐 Go | 📅 2026-08-18 - "a cloud asset inventory built for platform teams. Sync your cloud infrastructure metadata into your data warehouse, powering insights and automation."
* [Pachyderm](https://github.com/pachyderm/pachyderm) ⭐ 6,305 | 🐛 939 | 🌐 Go | 📅 2025-02-03 - "provides parallelized processing of multi-stage, language-agnostic pipelines with data versioning and data lineage tracking."
* [Redpanda Connect](https://www.redpanda.com/connect) - "a declarative data streaming and integration tool with 300+ pre-built connectors, configured via YAML."

## Cloud Services

* [Airbyte](https://airbyte.com/) - "Airbyte is an open-source data integration engine that helps you consolidate your data in your data warehouses, lakes and databases."
* [Alteryx](http://www.alteryx.com/) - "combines data preparation, data blending, and analytics — predictive, statistical, and spatial — in a visual workflow designer."
* [AWS Batch](https://aws.amazon.com/batch/) - "enables developers, scientists, and engineers to easily and efficiently run hundreds of thousands of batch computing jobs on AWS."
* [AWS Glue](https://aws.amazon.com/glue/) - "a serverless data integration service that makes it easy for analytics users to discover, prepare, move, and integrate data from multiple sources."
* [Cloud Data Fusion](https://cloud.google.com/data-fusion) - "Fully managed, cloud-native data integration platform."
* [Fivetran](https://www.fivetran.com/) - "automates data movement from disparate sources into your destination."
* [Google Dataflow](https://cloud.google.com/products/dataflow) - "Google Cloud Dataflow provides a simple, powerful model for building both batch and streaming parallel data processing pipelines."
* [Hevo](https://hevodata.com/) - "a no-code data movement platform that is usable by your most technical as well as your non-technical and business users."
* [Microsoft Azure Data Factory](https://azure.microsoft.com/en-us/services/data-factory/) - "A fully managed, serverless data integration service that helps you visually integrate data sources with more than 90 built-in, maintenance-free connectors."
* [Stitch](https://www.stitchdata.com/) - "Stitch is a cloud-first, open source platform for rapidly moving data. A simple, powerful ETL service, Stitch connects to all your data sources – from databases like MySQL and MongoDB, to SaaS applications like Salesforce and Zendesk – and replicates that data to a destination of your choosing."

## Big Data (Hadoop Stack)

* [Apache Beam](https://beam.apache.org/) - "a unified programming model for Batch and Streaming data processing."
* [Apache Flink](https://flink.apache.org/) - "a framework and distributed processing engine for stateful computations over unbounded and bounded data streams."
* [Debezium](https://debezium.io) - "Change data capture for a variety of databases."
* [Kafka Connect](https://kafka.apache.org/documentation/#connect) - "a tool for scalably and reliably streaming data between Apache Kafka and other systems. It makes it simple to quickly define connectors that move large collections of data into and out of Kafka."
* [Spark](https://spark.apache.org/) - "a fast and general-purpose cluster computing system. It provides high-level APIs in Scala, Java, and Python that make parallel jobs easy to write, and an optimized engine that supports general computation graphs. It also supports a rich set of higher-level tools including Shark (Hive on Spark), MLlib for machine learning, GraphX for graph processing, and Spark Streaming."

## ETL Tools (GUI)

*Warning*: If you're already familiar with a scripting language, GUI ETL tools are not a good replacement for a well structured application written with a scripting language. These tools lack flexibility and are a good example of the ["inner-platform effect"](https://en.wikipedia.org/wiki/Inner-platform_effect). With a large project, you will most likely run into instances where "the tool doesn't do that" and end up implementing something hacky with a script run by the GUI ETL tool. Also, the GUI can conceal complexity and the files these tools generate are impossible to code review. However, the GUI and out-of-the-box functionality can make some tasks simpler, especially for people not comfortable with writing code.

* [Apache NiFi](https://nifi.apache.org/) - "a rich, web-based interface for designing, controlling, and monitoring a dataflow."
* [CDAP](https://cdap.io/) - "Use Cask Data Application Platform to visually build and manage data applications in hybrid and multi-cloud environments."
* [Informatica PowerCenter](https://www.informatica.com/products/data-integration/powercenter.html) - An ETL tool for extracting data from source systems, transforming it, and loading it into target systems using a visual mapping and workflow designer.
* [Microsoft SSIS](https://learn.microsoft.com/en-us/sql/integration-services/sql-server-integration-services) - "a component of the Microsoft SQL Server database software that can be used to perform a broad range of data migration tasks."
* [N8n](https://github.com/n8n-io/n8n) ⭐ 201,179 | 🐛 1,073 | 🌐 TypeScript | 📅 2026-08-19 - "Free and open fair-code licensed node based Workflow Automation Tool. Easily automate tasks across different services."
* [Pentaho Data Integration (PDI)](https://www.hitachivantara.com/en-us/products/pentaho-platform/data-integration-analytics.html) - "a graphical ETL tool for designing data integration workflows using a drag-and-drop interface, also known as Kettle."

## Further Reading

* [Fundamentals of Data Engineering](https://www.oreilly.com/library/view/fundamentals-of-data/9781098108298/) - Joe Reis & Matt Housley's tool-agnostic overview of the data engineering lifecycle, including the ETL-to-ELT shift (2022).
* [The Rise of Data Contracts](https://dataproducts.substack.com/p/the-rise-of-data-contracts) - Chad Sanderson on formalizing schema and quality guarantees between data producers and consumers.
* [ELT 101: The Why and What of ELT](https://meltano.com/blog/elt-101-the-why-and-what-of-elt-or-the-why-not-of-etl/) - Why cheap cloud warehouse compute flipped the ETL paradigm to ELT.

## Contributing

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## Related Lists

* [awesome-pipeline](https://github.com/pditommaso/awesome-pipeline) ⭐ 6,619 | 🐛 34 | 📅 2026-08-04 - A curated list of awesome pipeline toolkits.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-19._
