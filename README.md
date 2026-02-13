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

Core Infrastructure & Orchestration

🚀 Remote Agents (Hybrid Data Plane): Securely run Saddle Data workers inside your own VPC or infrastructure. Zero-trust architecture with outbound-only polling.

🚀 Lightweight Orchestration (DAGs): Chain flows together (e.g., Run Flow B only after Flow A succeeds) to build reliable data dependencies.

🚀 Observability & Visualization: Visual graph view of your flow dependencies and detailed execution traces.

Transformations

🚀 dbt Core Integration: Native support for running dbt projects immediately after data ingestion. Includes secure Git authentication and dynamic version management.

🚀 Visual Schema Mapping: Explicit control over destination column types (Schema Mapping) with intelligent implicit casting for data cleanup.

New Connectors

🚀 Snowflake Destination: Enterprise-grade loading using internal stages for high volume and Merge support for upserts.

🚀 Databricks Destination: Native integration for Delta Lake.

🚀 Webhook Source: High-throughput event ingestion gateway with built-in rate limiting and buffering (Redis-backed).

🚀 MongoDB Source: Automatic flattening of BSON documents to SQL tables.

🚧 In Progress

Google Analytics 4 (GA4) Source: Extracting raw event and traffic data from GA4 properties.

Reverse ETL Patterns: Templates for syncing warehouse data back to operational tools (Salesforce/HubSpot).

📝 Next (Up Next)

Security: Two-Factor Authentication (2FA/MFA): Add support for users to secure their accounts with an authenticator app.

Shopify Source (OAuth): Upgrading the Shopify connector to a Public App model for easier one-click onboarding.

Fanout DAG Dependencies: Support for triggering multiple downstream flows from a single upstream flow (One-to-Many orchestration).

💡 Later / Ideas

ClickHouse Destination: Real-time analytical database support.

S3 / GCS Data Lake Destination: Outputting data as Parquet/Iceberg files.

Git Source: Analytics for engineering metrics (PRs, Commits).