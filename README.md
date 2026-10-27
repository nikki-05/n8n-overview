# n8n-overview

A personal knowledge base and workflow archive for learning and documenting n8n, the open-source workflow automation tool.

📌 What this repo is for

This repo is where I'm tracking my journey learning n8n — concepts, setup notes, example workflows I build, and reference material. The goal is to have one place that covers:

What n8n is and how it compares to other automation tools
Core concepts (nodes, triggers, items, expressions, credentials)
Installation & setup notes (Docker, npm, cloud)
My own exported workflows (.json files) with explanations
Screenshots and walkthroughs of workflows I've built
Tips, gotchas, and things I learn along the way

Think of it as a living "notes + examples" repo rather than a finished product — it'll grow as I learn more.

🤖 What is n8n?

n8n (pronounced "n-eight-n", short for "nodemation") is an open-source workflow automation platform. It lets you connect different apps, APIs, and services together into automated pipelines using a visual, node-based editor — similar to tools like Zapier, Make (Integromat), or Power Automate, but:

Open-source & self-hostable — run it for free on your own server or in Docker, or use their paid cloud version
Fair-code licensed — source-available; you can view and modify the code (not a fully permissive MIT license, but not closed-source either)
Node-based visual editor — every workflow is a canvas of connected "nodes": triggers, logic steps, and actions
Code-friendly — when the built-in nodes aren't enough, you can drop into a JavaScript or Python "Code" node directly inside the workflow
Core concepts
Concept	What it means
Workflow	The full automation — a canvas of connected nodes
Trigger node	Starts the workflow (webhook, schedule, form submission, chat message, etc.)
Node	A single step — calls an API, transforms data, branches logic, or talks to a service (Slack, Sheets, OpenAI, etc.)
Connections	The lines between nodes that define data flow and execution order
Items	The individual pieces of data passed between nodes
Expressions	{{ }} syntax used to reference data from earlier nodes dynamically
Credentials	Saved authentication (API keys, OAuth tokens) reused across nodes
Executions	A single run of a workflow, logged for debugging
Common use cases
Syncing data between apps (e.g. Google Sheets ↔ CRM)
Sending automated Slack/Discord/email notifications
Building AI agents that use tools, memory, and an LLM (e.g. OpenAI) to respond to chat input
Scraping or polling APIs on a schedule and reacting to changes
Internal ops automation (onboarding, ticket routing, reporting)

🚧 Status

Actively learning — this repo will be updated as I build more workflows and dig into more of n8n's features (AI Agents, webhooks, custom nodes, self-hosting, etc.).