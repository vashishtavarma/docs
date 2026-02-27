# Documentation structure

This file explains how EduTube docs are organized. It follows practices used by companies like Stripe, Twilio, and ReadMe.

## Audience separation

- **For users** — End-user guides: getting started, journeys, notes, explore, profile, chatbot. Task-oriented, plain language.
- **For developers** — Technical content: API, architecture, local setup, authentication, integration, troubleshooting. Technical language and code examples.

## Diátaxis framework

Content is organized into four types:

| Type | Purpose | Examples |
|------|---------|----------|
| **Tutorials** | Hands-on learning | Developer quickstart |
| **How-to guides** | Accomplish specific tasks | Local setup, integration guide |
| **Reference** | Complete technical facts | API reference (OpenAPI) |
| **Explanation** | Concepts and reasoning | Architecture |

## Developer journey

Docs support five stages:

1. **Discovery** — What does EduTube do? (index, API introduction)
2. **Evaluation** — How hard to implement? (architecture, integration)
3. **First implementation** — Quick start, authentication, first API call
4. **Troubleshooting** — Error resolution (troubleshooting, FAQ)
5. **Advanced usage** — Contributing, local development

## File layout

```
docs/
├── index.mdx              # Home (users + developers)
├── quickstart.mdx         # User quickstart
├── guides/                # User guides
├── developers/            # Developer docs
│   ├── getting-started.mdx
│   ├── local-setup.mdx
│   ├── architecture.mdx
│   ├── authentication.mdx
│   ├── integration.mdx
│   ├── troubleshooting.mdx
│   └── contributing.mdx
├── api-reference/         # OpenAPI + endpoint pages
└── docs.json              # Mintlify config (navigation, theme)
```

## Theme

Docs use a black & white theme: primary (#000000), light (#ffffff), dark (#000000). Configured in `docs.json` under `colors`.
