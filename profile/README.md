<!-- The organization's front door. Every sentence here about what Planton is or does mirrors the
     Planton story, which is told once and projected onto this page, the website, and the
     open-source README. The printed counts (700+, 8, 18, 17, 4) come from
     site/src/data/platform-stats.ts in plantonhq/planton, which records how each one was counted.
     Never retype a number here; change it there first. -->

<p align="center">
  <img src="https://github.com/plantonhq/planton/raw/main/.github/icon.png" alt="Planton" width="72">
</p>

# Planton: The Self-Service Cloud Platform

Your coding agent can already create cloud infrastructure. What it creates is unverified, unrecorded, and unrepeatable: nobody priced it, nobody checked the permissions, nothing remembers what was made, and the next environment starts from a blank prompt.

Planton turns your own cloud account into a self-service platform. AI designs the infrastructure, the platform verifies the cost and permissions before anything is created, and the design is published as an Infra Chart, a template your whole team can deploy. Your services then ship onto that infrastructure straight from Git. It sits beside the coding agent and the cloud CLI you already use; nothing about how you work changes.

- **Infra Hub** is Cursor for cloud infrastructure: describe what you need, watch it compose, see the monthly cost and the IAM policy before anything exists, deploy, and publish it as an Infra Chart.
- **Service Hub** is Vercel for backend, in your own cloud: connect a repository and every push becomes a running deployment, with the result written back into GitHub checks and deployments. No pipeline YAML, no Dockerfile required.

## Proof at Creation, Not Observation After

Every change Planton deploys is:

- **Priced before it exists**, with its coverage stated: an exact monthly figure with line items, a range, or plainly "unpriced". A zero never stands in for unknown. The least-privilege permission policy is derived from exactly what is composed, and every covered component states which of a fixed list of 17 technical controls it enforces, with evidence.
- **Held to your rules no matter who asked.** A deployment budget pauses a deploy whose verified cost exceeds it, for a human decision. Protected environments refuse self-approval. The catalog can be curated to the component kinds your organization allows. A sensitive field takes a managed secret, never a pasted value. The console, the CLI, and the coding agent see the same list and refuse the same things.
- **Left behind as a record.** One immutable stack job holds the exact configuration that was deployed, the cost fact, the budget verdict, who approved and why, and a snapshot of what exists afterward, queryable by resource, environment, time, and outcome.

## Runs Where You Decide

Hosted at [planton.ai](https://planton.ai), self-hosted on your own Kubernetes cluster with a license that verifies offline, or free on your laptop as Planton Desktop. In every shape it is your cloud account, your keys, your state, and your bill. Connections can be keyless, so no long-lived cloud credential is ever stored. If you leave, you take your manifests and keep deploying them with the open-source CLI.

## What Is Open Source Here

Every infrastructure module is Apache 2.0. Audit it, fork it, or run it without the platform.

| Repository | What it holds |
|---|---|
| [planton](https://github.com/plantonhq/planton) | The catalog: 700+ component kinds across 8 cloud providers, each a typed schema with a cost fact sheet, a control posture with evidence (17 controls, 4 framework crosswalks), and least-privilege runner permissions. 18 Infra Charts. The `planton` CLI and the IaC engine. The source of [planton.ai](https://planton.ai). |
| [skills](https://github.com/plantonhq/skills) | The agent skills Cursor, Claude Code, Codex, and every Agent Skills host load, so your agent composes, validates, prices, and deploys from the same craft the platform's own assistant uses. |
| [planton-mcp-server](https://github.com/plantonhq/planton-mcp-server) | The platform's own operations over MCP, for agents that want to build, apply, and deploy directly. |
| [homebrew-tap](https://github.com/plantonhq/homebrew-tap) | `brew install plantonhq/tap/planton`. |
| [install-planton-cli-action](https://github.com/plantonhq/install-planton-cli-action), [planton-cli-login-action](https://github.com/plantonhq/planton-cli-login-action) | The CLI inside GitHub Actions. |

## Start Tonight

- **Planton Desktop** is free for individuals forever, commercial use included: [planton.ai](https://planton.ai).
- **Teach your coding agent**: `npx skills add plantonhq/skills`, then read [Coding Agents](https://planton.ai/docs/coding-agents).
- **From the terminal**: `brew install plantonhq/tap/planton`, then the [Getting Started guide](https://planton.ai/docs/getting-started).
- **For a team**: the hosted free tier needs no card, and nobody below the self-serve ceiling talks to sales. [Pricing](https://planton.ai/pricing).

## In Their Words

> "As a junior DevOps engineer with almost no AWS experience, Planton enabled me to provide a very mature developer experience to our entire 7-person dev team. They can quickly deploy services to multiple environments without me having to deal with learning AWS from scratch or rewriting complex infrastructure code."
>
> Sai Saketh, Junior DevOps Engineer, iorta TechNext

Teams have run production on Planton since 2023. Planton runs on Planton.

## Community

- Questions and ideas: [Discord](https://discord.gg/pwcSapdQAp)
- Bugs and requests: [issues on plantonhq/planton](https://github.com/plantonhq/planton/issues)
- Contributing: [CONTRIBUTING.md](https://github.com/plantonhq/planton/blob/main/CONTRIBUTING.md) and the [CLA](https://github.com/plantonhq/planton/blob/main/CLA.md)
- Documentation: [planton.ai/docs](https://planton.ai/docs)

The code is [Apache 2.0](https://github.com/plantonhq/planton/blob/main/LICENSE). The Planton name and logo are trademarks of Planton Cloud, Inc.; see [TRADEMARKS.md](https://github.com/plantonhq/planton/blob/main/TRADEMARKS.md).
