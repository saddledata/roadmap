SaddleData Public Roadmap

Welcome to the official public roadmap for SaddleData! This repository provides visibility into our product development process. It's where we track what we're working on, what's coming up next, and where we gather essential feedback from our community of users.

We believe in building in public and want to give you a voice in shaping the future of SaddleData.

Please Note: This roadmap is for informational purposes only and is subject to change. Priorities can shift based on customer feedback, market changes, and new opportunities.

How to Contribute

The best way to provide feedback or suggest a new feature is to:

Check the existing Issues to see if your idea is already being discussed.

If it is, please add your thoughts to the existing issue!

If it's a new idea, please open a new issue, providing as much detail as possible about the problem you're trying to solve.

The Roadmap: Now, Next, Later

We use the "Now, Next, Later" framework to communicate our priorities.

Legend

🚀 Shipped - Recently completed and deployed.

🚧 In Progress - Actively in the development and testing phase.

📝 In Planning - In the final stages of design and will be worked on next.

💡 Idea / Backlog - A feature or idea we want to work on in the future.

✅ Recently Shipped

AI Reliability & Trust (New!)

🚀 LLM Validation Gateway: A high-performance, synchronous API that acts as an opinionated contract layer for AI outputs. Automatically repairs malformed JSON and performs aggressive type coercion in real-time.

🚀 Autonomous AI SRE: An AI Site Reliability Engineer that monitors broken pipelines, analyzes raw logs/stack traces, and provides root-cause diagnosis in plain English.

🚀 Intelligent Auto-Map: Your personal AI Data Architect. Profiles raw source data (including MongoDB/Webhooks) to automatically suggest schema mappings and normalization strategies.

🚀 Hallucination Detection: Silent integration with pii-hound during the validation phase to detect and flag unexpected sensitive data (SSNs, Keys) hallucinated by AI models.

Data Governance & Catalog

🚀 Governance Control Center: Centralized UI to define global Data Tags (PII, PHI) and author mandatory transformation policies.

🚀 Execution Circuit Breakers: Worker-level runtime validation that physically aborts any sync attempting to bypass security policies (e.g., via rogue IaC scripts or API overrides).

🚀 Schema Time Machine: Automated version control and historical change tracking for source schemas, complete with human-readable AI summaries of upstream changes.

🚀 Global Impact Analysis (Blast Radius): Visual dependency mapping showing exactly which downstream flows will be affected by an upstream schema change.

Core Infrastructure & Security

🚀 Infrastructure as Code (IaC) & GitOps: Manage your entire data stack programmatically using declarative YAML configurations. Fully supports CI/CD automation and version control.

🚀 Developer API & Token Management: Generate secure API tokens to programmatically interact with the Saddle Data platform and deploy infrastructure.

🚀 Sync State (Cursors) & API Management: Full transparency and control over incremental sync progress. View, rewind, or reset cursors via the UI or REST API.

🚀 Remote Agents (Hybrid Data Plane): Securely run Saddle Data workers inside your own VPC or infrastructure with zero-trust outbound-only polling.

Real-Time Enterprise Streaming

🚀 High-Performance Stream Agents: Double-buffered architecture with asynchronous stats reporting, enabling high-volume bursts and sub-second latency for enterprise streaming flows.

🚀 ClickHouse Destination: High-throughput, batch-optimized event streaming into ClickHouse for real-time analytics.

🚧 In Progress

🚧 Cloud Storage & Data Lakes (AWS S3 / GCS): Building an "S3 Bucket Watcher" for robust file-drop ingestion and partitioned file writers for destination lakes. (Prerequisite for Redshift integration).

📝 Next (Up Next)

📝 SQLMesh Integration: Native support for triggering SQLMesh data transformation pipelines immediately after ingestion, alongside our existing dbt Core integration.

📝 Amazon Redshift (Destination): High-performance enterprise loading utilizing AWS S3 internal staging and native Redshift COPY commands for massive ingestion scale.

📝 Webhook & Slack Alert Destinations: Expanding the Alerting Engine to support generic webhooks and native Slack integrations.

📝 Fanout DAG Dependencies: Support for triggering multiple downstream flows from a single upstream flow (One-to-Many orchestration).

💡 Later / Ideas

💡 Unstructured Data Parsing (AI Ingestion): Ingest PDFs, Word docs, and images from S3/Google Drive, using AI to extract structured JSON on the fly.

💡 Data Quality Observability: Proactive alerting for "Inference Integrity." Detect anomalies in the data itself.

💡 Smart Schema Defaults: Community-powered auto-mapping suggestions for common data sources.