# Awesome Sandboxes [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, neutral list of **every kind of sandbox**: AI-agent code-execution runtimes, enterprise/cloud/API test environments, and regulatory sandboxes.

Maintained alongside **[comparesandboxes.com](https://comparesandboxes.com)**, which carries the always-current specs, a dated benchmark and a cost calculator. Corrections and additions welcome via PR.

> [!NOTE]
> Figures move fast. This list links to primary sources; the maintained, dated numbers live on comparesandboxes.com.

## Contents
- [AI-agent code-execution sandboxes](#ai-agent-code-execution-sandboxes)
- [Enterprise, cloud & API sandboxes](#enterprise-cloud--api-sandboxes)
- [Regulatory & fintech sandboxes](#regulatory--fintech-sandboxes)
- [Benchmarks & tools](#benchmarks--tools)

## AI-agent code-execution sandboxes
Isolated compute where AI agents run untrusted code: compared on cold start, isolation, pricing, GPU and SDK support. → [full comparison](https://comparesandboxes.com/ai-agent-sandboxes)

- **[E2B](https://e2b.dev)**: Firecracker microVM, ~150ms cold start, pause/resume + snapshots. Cleanest SDK; official OpenAI Agents SDK provider.
- **[Daytona](https://www.daytona.io)**: Open-source (70K+★), container isolation, sub-90ms create, persistent workspaces, GPU.
- **[Modal](https://modal.com)**: Python-first, gVisor, sub-second cold start, **GPU inside the sandbox** (T4→B200).
- **[Vercel Sandbox](https://vercel.com/docs/vercel-sandbox)**: Firecracker, JS/TS-native, persistent by default.
- **[Cloudflare Sandbox SDK](https://developers.cloudflare.com/workers/)**: V8 isolates (~50ms) + containers, bundled with Workers.
- **[Northflank](https://northflank.com)**: Kata/gVisor microVM, lowest published vCPU rate, unlimited sessions, BYOC, GPU.
- **[Blaxel](https://blaxel.ai)**: ~25ms resume from hibernation, $0 idle compute.
- **[Runloop](https://www.runloop.ai)**: Enterprise coding-agent devboxes, SOC 2, 10K+ parallel, built-in SWE-bench.
- **[Fly.io Machines](https://fly.io)**: microVMs, persistent ext4, ~300ms checkpoints, native MCP, zero idle cost.
- **[CodeSandbox SDK](https://codesandbox.io/docs/sdk)**: Firecracker, git-versioned FS, sub-second forking (rebranding as Together Code Sandbox).
- **[Freestyle](https://freestyle.sh)**: Full Linux KVM VMs with real root for AI app builders.
- **[Morph](https://morphllm.com)**: Fast-apply model for editing files in a sandbox via MCP (a layer, not a full host).

- **[Lizard Sandboxes](https://lizard.build/sandboxes)**: Firecracker microVMs with Python and TypeScript SDKs, shell and file APIs, stateful Python execution, snapshots, and Persistent Volumes. [Documentation](https://lizard.build/docs/sandboxes/).

## Enterprise, cloud & API sandboxes
Vendor test environments for building against a platform without touching production. → [full comparison](https://comparesandboxes.com/enterprise-sandboxes)

- **[Salesforce Sandbox](https://www.salesforce.com/platform/sandboxes-environments/salesforce-sandbox-guide/)**: Developer / Developer Pro / Partial Copy / Full. → [types explained](https://comparesandboxes.com/guides/salesforce-sandbox-types)
- **[ServiceNow PDI](https://developer.servicenow.com)**: free, full-featured Personal Developer Instance.
- **[Stripe Sandbox](https://docs.stripe.com/sandboxes)**: isolated account copies, now the default over legacy test mode.
- **[Plaid Sandbox](https://plaid.com/docs/sandbox/)**: free, mock financial data (Development env retired 2024).
- **[AWS Sandbox](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-builder-center-sandbox/)**: Builder Center Sandbox / Sandbox OU / Innovation Sandbox (three different things).
- **[Mastercard](https://developer.mastercard.com)**, **[Visa](https://developer.visa.com)**, **[PayPal](https://developer.paypal.com/tools/sandbox/)**: payment API sandboxes.
- **[Shopify dev stores](https://shopify.dev/docs/api/development-stores)**, **[SAP API sandbox](https://api.sap.com)**, **[Twilio test credentials](https://www.twilio.com/docs/iam/test-credentials)**.

## Regulatory & fintech sandboxes
Supervised environments to trial regulated financial products. → [full comparison](https://comparesandboxes.com/regulatory-sandboxes)

- **[FCA Regulatory & Digital Sandbox](https://www.fca.org.uk/firms/innovation/regulatory-sandbox)** (UK)
- **[MAS FinTech Regulatory Sandbox](https://www.mas.gov.sg/development/fintech/regulatory-sandbox)** (Singapore)
- **[NayaOne](https://nayaone.com)**: fintech vendor-testing/evaluation sandbox for banks & FIs.

## Benchmarks & tools
- **[Sandbox benchmark (dated)](https://comparesandboxes.com/benchmark)**: cold start + pricing, sourced.
- **[Cost calculator](https://comparesandboxes.com/tools/cost-calculator)**: model your workload across providers.

## Dataset
A machine-readable version of this list (specs plus vendor-published cold-start and pricing figures) lives in [`data/sandboxes.json`](data/sandboxes.json) and [`data/sandboxes.csv`](data/sandboxes.csv), regenerated from [comparesandboxes.com](https://comparesandboxes.com) and licensed CC-BY-4.0.

## Contributing
Open a PR to add or correct an entry. Keep it neutral, cite a primary source, and it'll be reflected on comparesandboxes.com.

## License
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). Reuse freely with attribution to comparesandboxes.com.
