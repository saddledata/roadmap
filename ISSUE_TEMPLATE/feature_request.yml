name: 💡 Feature Request or Idea
description: Suggest a new feature, connector, or improvement for Saddle Data.
title: "[Feature]: <Short description>"
labels: ["enhancement", "triage"]
body:
  - type: markdown
    attributes:
      value: |
        ### 🤠 Welcome to the Saddle Data Roadmap!
        Thank you for helping us build a better data platform. Please fill out this form to give us the context we need to evaluate your idea.
  
  - type: dropdown
    id: category
    attributes:
      label: Feature Category
      description: Which area of Saddle Data does this relate to?
      options:
        - 🔌 New Source Connector
        - 🎯 New Destination Connector
        - 🛠️ Transformations / dbt
        - 🤖 AI Features (Pipeline Medic, Mapper, etc.)
        - 🔀 Orchestration / DAGs
        - 🔐 Core Platform / Infrastructure
        - 📝 Documentation
        - 🤷 Other
    validations:
      required: true

  - type: textarea
    id: problem
    attributes:
      label: What problem are you trying to solve?
      description: Is your feature request related to a specific problem or friction point? 
      placeholder: "e.g., When I try to sync nested JSON from MongoDB to Snowflake, I have to write a lot of manual SQL..."
    validations:
      required: true

  - type: textarea
    id: solution
    attributes:
      label: Describe the solution you'd like
      description: A clear and concise description of what you want to happen.
      placeholder: "e.g., I would love an AI button that profiles the MongoDB schema and auto-generates the flattening rules."
    validations:
      required: true

  - type: textarea
    id: alternatives
    attributes:
      label: Have you considered any alternatives or workarounds?
      description: How are you currently solving this problem?
      placeholder: "e.g., Right now I am dumping the raw JSON into Snowflake and using dbt LATERAL FLATTEN, but it's tedious."
    validations:
      required: false

  - type: textarea
    id: context
    attributes:
      label: Additional Context
      description: Add any other context, links to API docs, or screenshots here.
    validations:
      required: false

  - type: checkboxes
    id: contact
    attributes:
      label: Customer Discovery
      description: We love talking to our users!
      options:
        - label: I am willing to be contacted for a brief chat to help design this feature.
          required: false
