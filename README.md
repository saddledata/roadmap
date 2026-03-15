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

Data Governance & Catalog (New!)

🚀 Centralized Data Asset Registry: Decoupled schemas from individual flows into a centralized, reusable asset library acting as a single source of truth.

🚀 Global Impact Analysis (Blast Radius): Visual dependency mapping showing exactly which downstream flows will be affected by an upstream schema change.

🚀 Centralized Security Policies & PII: Column-level tagging (PII, PHI, Sensitive) with Automated Enforcement that auto-injects Hash/Mask transformations across all dependent flows.

🚀 Schema Time Machine: Automated version control and historical change tracking for source schemas, complete with human-readable AI summaries of upstream changes.

AI Data Infrastructure

🚀 Vector Database Destinations: Native sinking to Pinecone, Qdrant, Milvus, and PostgreSQL (pgvector) to power AI RAG directly from operational data.

🚀 In-Flight AI Embeddings: Zero-config Google Gemini and OpenAI (BYOK) embedding middleware. Transform text columns into dense mathematical vectors in transit without custom Python scripts.

Enterprise & Analytics Connectors

🚀 Enterprise SFTP (Source & Destination): Secure file transfer protocol support for legacy system integration and partner data exchange (CSV, JSON, JSONL) with smart auto-type inference.

🚀 Email & Excel Delivery (Destination): Automated Reverse ETL delivery of formatted Microsoft Excel (.xlsx) and CSV reports directly to executive inboxes via SMTP2Go/SendGrid.

🚀 Google Sheets Source: Directly ingest data from Google Workspace spreadsheets.

🚀 Snowflake Destination: Enterprise-grade loading using internal stages for high volume and Merge support for upserts.

🚀 Databricks Destination: Native integration for Delta Lake.

🚀 ClickHouse Destination: High-throughput, batch-optimized event streaming into ClickHouse for real-time analytics.

🚀 Webhook Source: High-throughput event ingestion gateway with built-in rate limiting and buffering (Redis-backed).

🚀 MongoDB Source: Automatic flattening of BSON documents to SQL tables.

🚀 Google Analytics 4 (GA4) Source: Extracting raw event and traffic data from GA4 properties.

Real-Time Enterprise Streaming

🚀 High-Performance Stream Agents: Double-buffered architecture with asynchronous stats reporting, enabling high-volume bursts and sub-second latency for enterprise streaming flows.

🚀 WebSocket Gateway Optimization: Tuned the stream-gateway for larger fetch sizes and reduced latency, including automatic ws:// to wss:// protocol upgrades.

🚀 Streaming UI Dashboard: Tailored Flow Detail pages specifically for real-time throughput, hiding irrelevant batch metrics and replacing them with persistent Total Rows and Total Errors counters.

Observability & Monitoring

🚀 Self-Serve UI Telemetry: Lightweight, first-party tracking SDK piping UI usage data and backend system_events directly into our own ClickHouse analytics tables for end-to-end user journey visibility.

🚀 Advanced Streaming Observability: Ingestion error tracking detects webhook failures (e.g., rate limits/body read errors) and pushes them directly to the flow's health dashboard.

🚀 Observability & Alerting Engine: Real-time Activity Feed and Alert Rules. All stream lifecycle events provide a clear audit trail.

🚀 Remote Agent Monitoring: Heartbeat tracking for self-hosted agents with automated "Agent Offline" alerting.

Core Infrastructure & Security

🚀 Agent Resilience & Self-Healing: Non-blocking connection logic prevents panics during destination DB blips. Includes automatic reconciliation loops.

🚀 Developer Experience (DX): Streamlined local agent testing with SADDLEDATA_SKIP_TLS_VERIFY and standardized API URL environment variables.

🚀 Security (2FA/MFA): Secured user accounts with TOTP-based authentication.

🚀 Remote Agents (Hybrid Data Plane): Securely run Saddle Data workers inside your own VPC or infrastructure with zero-trust outbound-only polling.

Transformations & Activation

🚀 Intelligent Auto-Map: Your personal AI Data Scientist that handles schema profiling, normalization, and suggests multi-table pipeline structures on the fly.

🚀 Saddle Data AI SRE: Autonomous error diagnosis. Analyzes worker logs to explain failures in plain English and provides step-by-step remediation (e.g., fixing schema drift).

🚀 Reverse ETL Templates: Pre-built patterns for syncing warehouse data back to operational tools.

🚀 dbt Core Integration: Native support for running dbt projects immediately after data ingestion.

🚀 Visual Schema Mapping: Explicit control over destination column types with intelligent implicit casting.

🚧 In Progress

🚧 Cloud Storage & Data Lakes (AWS S3 / GCS): Building an "S3 Bucket Watcher" for robust file-drop ingestion (CSV/JSON/Parquet), and partitioned file writers for destination lakes. (This is a core prerequisite for our upcoming Redshift integration).

📝 Next (Up Next)

📝 Amazon Redshift (Destination): High-performance enterprise loading utilizing AWS S3 internal staging and native Redshift COPY commands for massive ingestion scale.

📝 Webhook & Slack Alert Destinations: Expanding the Alerting Engine to support generic webhooks and native Slack integrations.

📝 Fanout DAG Dependencies: Support for triggering multiple downstream flows from a single upstream flow (One-to-Many orchestration).

📝 Shopify Source (OAuth): Upgrading the Shopify connector to a Public App model.

💡 Later / Ideas

New Connectors

💡 Amazon Redshift (Source): Extracting aggregated analytics models out of Redshift for operational syncing.

💡 Enterprise Spreadsheet Connectors: Microsoft Excel / Office 365 (OneDrive/SharePoint) via Microsoft Graph OAuth.

💡 Marketing & Sales Connectors: Google Search Console, Apollo.io, YouTube Analytics API.

💡 ClickHouse Source: Reverse ETL capabilities to extract aggregated metrics from ClickHouse and sync them back to operational tools.

Advanced Features

💡 Unstructured Data Parsing (AI Ingestion): Ingest PDFs, Word docs, and images from S3/Google Drive, using AI to extract structured JSON on the fly.

💡 Data Quality Observability: Proactive alerting for "Inference Integrity." Detect anomalies in the data itself.

💡 Developer API & Token Management: API token generation to allow programmatic access to Saddle Data.

💡 Smart Schema Defaults: Community-powered auto-mapping suggestions for common data sources.

💡 GitOps (Flows as Code): Manage Saddle Data pipeline configurations natively via Git pull requests.