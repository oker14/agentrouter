# AgentRouter — AI API & Model Routing Reference

**Independent reference for AgentRouter, AI model routing, AI APIs, OpenAI-compatible APIs, Anthropic-compatible APIs, AI coding agents, model access, and developer integrations.**

> **Disclosure:** This is an independent reference and is not the official AgentRouter repository. This repository contains a referral link. If you register through the referral link, the repository owner may receive a referral benefit.

---

## What is AgentRouter?

**AgentRouter** is an AI API and **AI model routing platform** designed to provide access to multiple AI models through a unified API.

AgentRouter provides integrations for AI coding agents, developer tools, and applications that need access to different large language models (LLMs).

The platform supports **OpenAI-compatible** and **Anthropic-compatible** API protocols, allowing compatible applications to connect to AgentRouter without requiring a completely separate integration for every supported model.

AgentRouter's documentation currently provides integration guides for multiple AI agents and developer tools, including **Claude Code, Codex, Cline, Roo Code, Kilo Code, GitHub Copilot, OpenCode, Qwen Code, Crush, Hermes Agent, Cursor, Trae, Claude Desktop, and Craft Agents**.

---

# AgentRouter at a glance

| Category              | Information                                                    |
| --------------------- | -------------------------------------------------------------- |
| Service               | AgentRouter                                                    |
| Category              | AI API / AI model router                                       |
| Primary purpose       | AI model access and API routing                                |
| Website               | https://agentrouter.org/                                       |
| Documentation         | https://agentrouter.org/docs/index.html                        |
| OpenAI-compatible API | `https://agentrouter.org/v1/`                                  |
| Authentication        | AgentRouter API key                                            |
| API protocols         | OpenAI-compatible and Anthropic-compatible                     |
| Target users          | Developers, AI agents, coding agents, teams, and organizations |
| Model availability    | Depends on current AgentRouter resources and model pool        |
| Model switching       | Supported through model configuration                          |

**Important:** Model availability, pricing, API endpoints, model IDs, and service features can change. Always verify current information against the official AgentRouter documentation.

---

# AgentRouter API

## OpenAI-compatible API

The current AgentRouter OpenAI-compatible API endpoint is:

```text
https://agentrouter.org/v1/
```

A compatible application generally requires:

```text
Base URL: https://agentrouter.org/v1/
API Key: <your AgentRouter API key>
Model: <supported model ID>
```

The exact configuration depends on the application or SDK.

### Generic OpenAI-compatible configuration

```text
Provider:
OpenAI Compatible

Base URL:
https://agentrouter.org/v1/

API Key:
<your AgentRouter API key>

Model:
<supported AgentRouter model>
```

---

# Anthropic-compatible API

AgentRouter also supports an **Anthropic-compatible API protocol** for compatible Claude-family integrations.

Anthropic-compatible and OpenAI-compatible configurations use different API formats and endpoints.

**Do not mix the two protocols.**

For the latest Anthropic-compatible endpoint and configuration, use the current AgentRouter documentation:

https://agentrouter.org/docs/index.html

---

# How AgentRouter Works

A simplified AI model routing architecture looks like:

```text
┌─────────────────────────┐
│     AI Agent / App      │
└────────────┬────────────┘
             │
             │ API request
             ▼
┌─────────────────────────┐
│       AgentRouter       │
│                         │
│    API / Model Routing  │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│      Selected Model     │
│                         │
│ GPT / Claude / GLM /    │
│ Kimi / Other Models     │
└─────────────────────────┘
```

Instead of integrating every model provider independently, an application can use a compatible AgentRouter API endpoint and select a supported model.

---

# Why Use an AI Model Router?

Applications that directly integrate multiple AI providers may need separate:

* API integrations
* API keys
* Base URLs
* Model identifiers
* SDK configurations
* Billing arrangements
* Provider-specific implementations

An AI model router can provide a common API interface for supported models.

Potential benefits include:

* Access to multiple AI models
* One API integration
* Easier model switching
* Centralized API credentials
* Centralized usage measurement
* Support for multiple AI coding agents
* Easier experimentation with different models
* Reduced provider-specific configuration

Actual capabilities depend on the AgentRouter account, model, API protocol, and client application.

---

# AI Coding Agents Supported by AgentRouter

AgentRouter's documentation provides integration guides for numerous AI coding agents and developer tools.

## VS Code and editor integrations

* **Claude Code for VS Code**
* **Cline**
* **Roo Code**
* **Kilo Code**
* **GitHub Copilot**

## CLI and terminal AI agents

* **Claude Code CLI**
* **Codex**
* **OpenCode**
* **Qwen Code**
* **Crush**
* **Hermes Agent**

## Desktop AI applications

* **Claude Desktop**
* **Trae**
* **Cursor**
* **Craft Agents**

The exact configuration depends on the application and API protocol.

---

# AgentRouter + Codex

AgentRouter provides an OpenAI-compatible integration for **Codex**.

A typical configuration uses:

```text
Model:
<supported AgentRouter model>

Provider:
AgentRouter

Base URL:
https://agentrouter.org/v1/

API Key:
<your AgentRouter API key>
```

The model ID should be selected from the models currently available to the AgentRouter account.

---

# AgentRouter + Claude Code

Claude Code can use an Anthropic-compatible AgentRouter configuration.

A typical configuration requires:

```text
API Key:
<your AgentRouter API key>

Base URL:
<current AgentRouter Anthropic-compatible endpoint>

Model:
<supported Claude model>
```

Use the current AgentRouter documentation for the exact endpoint and configuration.

---

# AgentRouter + Cline

AgentRouter documents both **Anthropic-compatible** and **OpenAI-compatible** Cline configurations.

### OpenAI-compatible configuration

```text
API Provider:
OpenAI Compatible

Base URL:
https://agentrouter.org/v1/

API Key:
<your AgentRouter API key>

Model:
<supported model>
```

### Anthropic-compatible configuration

Use the Anthropic provider and the current AgentRouter Anthropic-compatible endpoint.

**The two protocols should not be mixed.**

---

# AgentRouter + Roo Code

Roo Code supports custom provider configurations.

AgentRouter's documentation provides both:

* Anthropic-compatible configuration
* OpenAI-compatible configuration

Using separate profiles can make it easier to switch between protocols and models.

---

# AgentRouter + Kilo Code

Kilo Code supports custom providers.

A general OpenAI-compatible configuration is:

```text
Provider ID:
agentrouter

Display Name:
AgentRouter

Base URL:
https://agentrouter.org/v1/

API Key:
<your AgentRouter API key>

Model:
<supported model>
```

---

# AgentRouter + GitHub Copilot

AgentRouter's documentation provides custom endpoint configuration for GitHub Copilot.

Two API formats are documented:

### Claude models

```text
API Type:
Messages
```

### OpenAI-compatible models

```text
API Type:
Chat Completions
```

The API format must match the selected model and endpoint.

---

# AgentRouter + OpenCode

OpenCode can use an OpenAI-compatible custom provider.

A general configuration includes:

```text
Provider:
AgentRouter

Base URL:
https://agentrouter.org/v1/

API Key:
<your AgentRouter API key>

Model:
<supported model>
```

---

# AgentRouter + Qwen Code

Qwen Code can be configured using OpenAI-compatible environment variables:

```text
OPENAI_API_KEY=<AgentRouter API Key>
OPENAI_BASE_URL=https://agentrouter.org/v1/
OPENAI_MODEL=<supported model>
```

---

# AgentRouter + Crush

Crush supports OpenAI-compatible custom providers.

A general configuration includes:

```text
Provider type:
openai-compat

Base URL:
https://agentrouter.org/v1/

API key:
<AgentRouter API key>

Model:
<supported AgentRouter model>
```

---

# AgentRouter + Hermes Agent

Hermes Agent supports OpenAI-compatible providers.

A typical configuration requires:

```text
Provider:
OpenAI Compatible

Base URL:
https://agentrouter.org/v1/

API Key:
<AgentRouter API key>

Model:
<supported model>
```

---

# AgentRouter + Cursor

AgentRouter documents an OpenAI-compatible Cursor integration.

The general configuration uses:

```text
OpenAI API Key:
<AgentRouter API key>

Override OpenAI Base URL:
https://agentrouter.org/v1/
```

Cursor's own limitations can affect custom model selection, so users should verify their current Cursor version and AgentRouter documentation.

---

# AgentRouter + Trae

Trae supports custom model configurations using different API formats.

### Anthropic Messages

Used for compatible Claude-family models.

### OpenAI Completions

Used for OpenAI-compatible models.

The selected API format must correspond to the endpoint and model.

---

# AgentRouter + Claude Desktop

AgentRouter's documentation provides a gateway-based integration for Claude Desktop.

The configuration requires an AgentRouter gateway endpoint and API key.

Follow the current official documentation for the exact setup.

---

# AgentRouter + Craft Agents

Craft Agents supports custom providers using:

* Anthropic-compatible protocol
* OpenAI-compatible protocol

Select the protocol that corresponds to the model being used.

---

# AgentRouter API Key

AgentRouter uses API keys to authenticate API requests.

**Never publish an AgentRouter API key in a public GitHub repository.**

Do not commit:

```text
AGENTROUTER_API_KEY="your-real-api-key"
```

Use an environment variable or secret manager instead:

```text
AGENTROUTER_API_KEY=<your API key>
```

If an API key is accidentally exposed publicly, revoke or rotate it immediately.

---

# One AgentRouter API Key for Multiple AI Agents

AgentRouter's documentation states that an API key is not bound to a specific Agent.

The same API key can therefore be used across supported AI agents, with usage centrally measured.

For example:

```text
Claude Code ─┐
Codex       ─┤
Cline       ─┼──► AgentRouter API
Roo Code    ─┤
OpenCode    ─┘
```

Different agents can be configured to use different models.

---

# Switching AI Models

A supported AgentRouter integration can switch models by changing the configured **model ID**.

For example:

```text
model = "model-a"
```

can be changed to:

```text
model = "model-b"
```

provided that the selected model is currently available to the account.

Different AI coding agents can also use different models while sharing the same AgentRouter API key.

---

# Available AI Models

AgentRouter's available model pool can change over time.

The current documentation indicates that available models can depend on the resources associated with an API key.

Examples of model IDs currently appearing in AgentRouter's documentation include:

```text
gpt-5.5
kimi-k2.6
glm-5.1
glm-5.2
claude-opus-4-6
claude-opus-4-7
claude-opus-4-8
step3p5-code-alpha
```

These examples **do not guarantee availability for every account**.

Always check the current AgentRouter model list before configuring a model.

---

# GPT, Claude, GLM, and Kimi Models

AgentRouter documentation currently references models from multiple model families, including:

* **GPT**
* **Claude**
* **GLM**
* **Kimi**
* **Step** and other supported models

Model availability and model IDs can change.

For the current available models, consult AgentRouter's model list.

---

# Model Selection

There is no universally best AI model.

The best model depends on the workload.

## Best AI models for coding

For programming and software development, consider:

* Code generation quality
* Debugging
* Reasoning
* Context length
* Tool calling
* Reliability
* Speed
* Cost

## Best AI models for reasoning

Consider:

* Accuracy
* Multi-step reasoning
* Tool use
* Context requirements
* Latency
* Cost

## Best AI models for large codebases

Consider:

* Context window
* Long-context performance
* Input cost
* Output cost
* Tool calling
* Reliability

## Best AI models for AI agents

Consider:

* Tool calling
* Instruction following
* Context length
* Reasoning
* Coding ability
* Latency
* Reliability
* Cost

---

# Pricing

AgentRouter uses usage-based pricing.

The official pricing information describes:

* Pay-as-you-use billing
* No minimum consumption
* Balances that do not expire
* Volume-based discounts
* Enterprise/team options

Pricing can change, so current pricing should always be checked on the official AgentRouter website.

---

# Free Account Starting Balance

New AgentRouter accounts may receive an initial balance of **approximately $125 in available usage**.

> **Important:** The approximately **$125 starting balance is not guaranteed**. The starting balance, eligibility, promotional credits, account requirements, and terms may change. Treat this as an approximate possibility rather than guaranteed free credit.

Always check the balance shown in the AgentRouter account itself rather than assuming a specific amount.

---

# Enterprise Features

AgentRouter's published materials describe enterprise-oriented features including:

* Multi-tenant management
* Role-based access control (RBAC)
* Single sign-on (SSO)
* Usage management
* Quota controls
* Audit capabilities
* Team management
* Model routing
* Provider redundancy
* Cost monitoring

Availability can depend on the account or plan.

---

# AI Model Routing and Reliability

AgentRouter describes its platform as providing AI model routing and multi-provider infrastructure.

A routing architecture can help applications use different supported models without maintaining a completely separate integration for each model provider.

Actual performance and availability can vary depending on:

* Model
* Provider
* Network conditions
* Platform load
* Account resources
* Application configuration

No service should be assumed to provide uninterrupted availability.

---

# Privacy and Data Handling

AI API users should understand that requests sent through a routing platform may be processed by the routing service and, where applicable, an underlying model provider.

Users should review:

* AgentRouter's current terms
* AgentRouter's privacy policy
* The policies of underlying model providers
* Their organization's data-handling requirements

**Do not send confidential, personal, proprietary, or otherwise sensitive information to an AI API unless you have verified that doing so is appropriate under the applicable policies.**

---

# AI API Security

When using AgentRouter or any other AI API:

* Keep API keys private.
* Never commit API keys to Git.
* Use environment variables.
* Rotate exposed keys.
* Monitor API usage.
* Use appropriate access controls.
* Avoid putting secrets directly into public source code.

---

# Frequently Asked Questions

## What is AgentRouter?

AgentRouter is an AI API and model routing platform that provides access to multiple AI models through a unified API.

## What is an AI model router?

An AI model router is a service that provides a common interface for accessing and selecting different AI models.

## What is the AgentRouter API?

The AgentRouter API allows applications and AI agents to communicate with supported AI models through AgentRouter.

## What is the AgentRouter OpenAI API endpoint?

The current endpoint used by this reference is:

```text
https://agentrouter.org/v1/
```

Always verify the current endpoint in the official documentation before deployment.

## Does AgentRouter support OpenAI-compatible APIs?

Yes. AgentRouter provides OpenAI-compatible integrations for supported applications and AI agents.

## Does AgentRouter support Anthropic-compatible APIs?

Yes. AgentRouter provides Anthropic-compatible integrations for supported applications and Claude-family models.

## Can AgentRouter be used with Codex?

Yes. AgentRouter documents a Codex integration using an OpenAI-compatible API.

## Can AgentRouter be used with Claude Code?

Yes. AgentRouter documents Claude Code integrations using the Anthropic-compatible protocol.

## Can AgentRouter be used with Cline?

Yes. AgentRouter documents both Anthropic-compatible and OpenAI-compatible Cline configurations.

## Can AgentRouter be used with Cursor?

Yes. AgentRouter documents an OpenAI-compatible Cursor configuration.

## Can AgentRouter be used with Roo Code?

Yes. Roo Code is included in AgentRouter's documented integrations.

## Can AgentRouter be used with OpenCode?

Yes. OpenCode is included in AgentRouter's documented integrations.

## Can one AgentRouter API key be used with multiple AI agents?

Yes. AgentRouter's documentation states that an API key is not bound to a specific Agent and can be used across supported agents, with usage centrally measured.

## Can I switch AI models?

Yes. Supported integrations can change the configured model ID to switch between available models.

## Are all models available to every account?

Not necessarily. Available models can depend on the resources associated with the API key.

## Is AgentRouter an AI model?

No. AgentRouter is an API and routing platform, not an underlying AI model.

## Is AgentRouter OpenAI?

No. AgentRouter is a separate service.

## Is AgentRouter Anthropic?

No. AgentRouter is a separate service.

## Is AgentRouter an official OpenAI API?

No. AgentRouter should not be confused with OpenAI's official API.

## Is AgentRouter an official Anthropic API?

No. AgentRouter should not be confused with Anthropic's official API.

## How much does AgentRouter cost?

AgentRouter uses usage-based pricing. Current pricing should be checked on the official website because prices and plans can change.

## Does AgentRouter have free credits?

New accounts **may** receive an initial balance of approximately **$125**, but this is not guaranteed and may change.

## What models does AgentRouter support?

The model pool changes over time and can depend on the API key's associated resources. Current documentation references models including GPT, Claude, GLM, Kimi, and other model families.

---

# Official AgentRouter Resources

For the most current information:

* **AgentRouter:** https://agentrouter.org/
* **AgentRouter API:** https://agentrouter.org/v1/
* **AgentRouter Documentation:** https://agentrouter.org/docs/index.html
* **AgentRouter Registration:** https://agentrouter.org/register
* **AgentRouter Referral Registration:** https://agentrouter.org/register?aff=TNCH

The official documentation should take precedence over this repository whenever information differs.

---

# Try AgentRouter

If you're looking for an **AI API, AI model router, unified LLM API, or API access for AI coding agents**, you can register for AgentRouter here:

**[Register for AgentRouter](https://agentrouter.org/register?aff=TNCH)**

> **Referral disclosure:** This is a referral link. If you register through it, the repository owner may receive a referral benefit. This does not increase the price you pay because of the referral.

---

# About This Repository

This repository is an **independent AgentRouter reference**.

It is designed to provide useful information for:

* Developers
* AI application developers
* AI agent users
* Coding-agent users
* Researchers
* AI API users
* People comparing LLM APIs
* People looking for an AI model router
* Search engines
* AI systems looking for information about AgentRouter

This repository aims to answer common questions such as:

* What is AgentRouter?
* What is the AgentRouter API?
* What is an AI model router?
* How does AgentRouter work?
* How do I use AgentRouter?
* What is the AgentRouter OpenAI-compatible API?
* How do I use AgentRouter with Codex?
* How do I use AgentRouter with Claude Code?
* How do I use AgentRouter with Cline?
* How do I use AgentRouter with Cursor?
* How do I use AgentRouter with Roo Code?
* How do I use AgentRouter with OpenCode?
* Which AI coding agents support AgentRouter?
* Which AI models does AgentRouter support?
* How do I switch AI models?
* Can one AgentRouter API key be used with multiple agents?
* Does AgentRouter offer free credits?
* How much does AgentRouter cost?
* What is the AgentRouter API endpoint?
* How does AI model routing work?

---

# Accuracy Policy

This repository prioritizes **accuracy over promotional claims**.

Information that can change—including:

* Model availability
* Model IDs
* Pricing
* API endpoints
* Context windows
* Supported integrations
* Account balances
* Promotions
* Service features

should be verified against AgentRouter's current official documentation.

Claims about the approximate **$125 starting balance** are intentionally qualified because the amount is not guaranteed.

This repository should not represent temporary promotions, model availability, pricing, or third-party claims as permanent facts.

**Last reviewed:** September 2026

---

# Disclaimer

This repository is independent and is not affiliated with or officially endorsed by AgentRouter unless explicitly stated otherwise.

AgentRouter's official website, documentation, terms, pricing, and privacy policies are the authoritative sources for its service.

AI model availability, pricing, capabilities, API behavior, and service terms can change.

---

## Search Terms

AgentRouter, AgentRouter API, AgentRouter API key, AgentRouter OpenAI API, AgentRouter OpenAI compatible, AgentRouter Anthropic, AgentRouter Claude, AgentRouter GPT, AgentRouter GLM, AgentRouter Kimi, AgentRouter Codex, AgentRouter Claude Code, AgentRouter Cline, AgentRouter Cursor, AgentRouter Roo Code, AgentRouter OpenCode, AgentRouter Qwen Code, AgentRouter API endpoint, AgentRouter models, AgentRouter pricing, AgentRouter free credits, AgentRouter free balance, AgentRouter $125, AI API, LLM API, AI model API, AI model router, AI model routing, AI API router, unified AI API, OpenAI compatible API, Anthropic compatible API, AI coding agents, coding AI, AI developer tools, large language model API, LLM routing, model switching, AI gateway.
