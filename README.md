# Awesome AI Security 

> Securing and attacking AI systems, large language models, and autonomous agents.

Maintained by [Kaimi](https://kaimi.ai). Contributions are welcome, see [Contributing](#contributing).

## Contents

- [Threat Taxonomies & Frameworks](#threat-taxonomies--frameworks)
- [Governance, Standards & Regulation](#governance-standards--regulation)
- [Prompt Injection & Jailbreaks](#prompt-injection--jailbreaks)
- [Red Teaming & Offensive Tooling](#red-teaming--offensive-tooling)
- [Guardrails & Defensive Tooling](#guardrails--defensive-tooling)
- [AI Gateways](#ai-gateways)
- [Detection Engineering & Monitoring](#detection-engineering--monitoring)
- [Model & Supply Chain Security](#model--supply-chain-security)
- [Agent, MCP & Memory Security](#agent-mcp--memory-security)
- [OSINT, Recon & Secrets Exposure](#osint-recon--secrets-exposure)
- [Benchmarks & Evaluations](#benchmarks--evaluations)
- [AI in OT & Critical Infrastructure](#ai-in-ot--critical-infrastructure)
- [Incident Response & Operations](#incident-response--operations)
- [Incidents & Threat Intelligence](#incidents--threat-intelligence)
- [Vulnerability Research & Bug Bounty](#vulnerability-research--bug-bounty)
- [Foundational Papers & Research](#foundational-papers--research)
- [Training, CTFs & Labs](#training-ctfs--labs)
- [Contributing](#contributing)

---

## Threat Taxonomies & Frameworks

- [MITRE ATLAS](https://atlas.mitre.org/) - Knowledge base of adversary tactics and techniques against AI-enabled systems.
- [MITRE ATLAS: SAFE-AI Report](https://atlas.mitre.org/pdf-files/SAFEAI_Full_Report.pdf) - MITRE's framework for securing AI-enabled systems, mapped to ATLAS.
- [ATLAS Knowledge Base Agent](https://github.com/mitre-atlas/atlas-knowledge-base-agent) - Agent for querying the MITRE ATLAS knowledge base.
- [OWASP Top 10 for LLM Applications](https://genai.owasp.org/llm-top-10/) - The reference list of the most critical risks in LLM applications.
- [OWASP Agentic AI: Threats and Mitigations](https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/) - OWASP GenAI Security Project's threat model for agentic systems.
- [OWASP Agentic Skills Top 10](https://owasp.github.io/www-project-agentic-skills-top-10/) - OWASP's top risks for agent skills.
- [NIST AI 100-2: Adversarial Machine Learning](https://csrc.nist.gov/pubs/ai/100/2/e2025/final) - NIST taxonomy and terminology of attacks and mitigations for predictive and generative AI.
- [Google SAIF](https://saif.google/) - Google's Secure AI Framework and risk map.
- [CSA MAESTRO](https://cloudsecurityalliance.org/blog/2025/02/06/agentic-ai-threat-modeling-framework-maestro) - Cloud Security Alliance's layered threat-modeling framework for agentic AI.
- [AI Security Attack Taxonomy](https://ai.securityattack.fyi/attacks/indirect-prompt-injection) - Attack catalogue for AI systems, starting with indirect prompt injection.
- [securitycontrols.ai](https://securitycontrols.ai/) - Security controls reference for AI systems.
- [It's Broken: AI Security Cheatsheet](https://itsbroken.ai/cheatsheet/) - Quick-reference cheatsheet for AI attacks and defenses.

## Governance, Standards & Regulation

- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) - Voluntary framework for managing AI risk, with the Generative AI profile.
- [ISO/IEC 42001](https://www.iso.org/standard/81230.html) - Management system standard for AI, the certifiable baseline for AI governance.
- [EU AI Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) - Regulation (EU) 2024/1689, including cybersecurity and robustness obligations for high-risk AI.
- [EU Cyber Resilience Act](https://eur-lex.europa.eu/eli/reg/2024/2847/oj) - Regulation (EU) 2024/2847 on security requirements for products with digital elements, AI products included.
- [NIS2 Directive](https://eur-lex.europa.eu/eli/dir/2022/2555/oj) - Directive (EU) 2022/2555, the security baseline for essential and important entities deploying AI.
- [ENISA: Multilayer Framework for Good Cybersecurity Practices for AI](https://www.enisa.europa.eu/publications/multilayer-framework-for-good-cybersecurity-practices-for-ai) - ENISA's layered good-practice framework for AI security.

## Prompt Injection & Jailbreaks

- [Prompt Injection in the Wild](https://cybershujin.github.io/Prompt-Injection-in-the-Wild/) - Collection of real-world prompt injection cases.
- [Prompt Injection Email Samples](https://github.com/cyb3rmik3/prompt-injection-email-samples) - Sample emails for testing indirect prompt injection in email-processing agents.
- [Prompting Guide: Adversarial Prompting](https://www.promptingguide.ai/risks/adversarial) - Overview of injection, leaking, and jailbreak techniques.
- [PromptIntel](https://promptintel.novahunting.ai/) - Threat intelligence feed for malicious prompts.
- [jailbreaks](https://github.com/togg53192-cmd/jailbreaks) - Jailbreak prompt collection for model evaluation.
- [pliny.gg](https://pliny.gg/) - Pliny's LLM jailbreaking research hub.

## Red Teaming & Offensive Tooling

- [garak](https://github.com/NVIDIA/garak) - NVIDIA's LLM vulnerability scanner with a large probe library.
- [PyRIT](https://github.com/Azure/PyRIT) - Microsoft's Python Risk Identification Toolkit for generative AI red teaming.
- [promptfoo](https://github.com/promptfoo/promptfoo) - LLM eval and red teaming CLI with CI integration.
- [DeepTeam](https://github.com/confident-ai/deepteam) - Open-source LLM red teaming framework.
- [Giskard](https://github.com/Giskard-AI/giskard) - Testing and vulnerability scanning for LLM and ML models.
- [Adversarial Robustness Toolbox](https://github.com/Trusted-AI/adversarial-robustness-toolbox) - Library for evasion, poisoning, extraction, and inference attacks and defenses on ML models.
- [OpenHack](https://github.com/openhackai/OpenHack) - Open-source agentic code security scanner and verifier built on open models.
- [Talon](https://github.com/CarbeneAI/Talon) - MCP server connecting Claude Code to a pentesting VM for AI-assisted penetration testing.
- [OpenA2A CLI](https://opena2a.org/cli) - CLI for agent-to-agent security testing.
- [HackMyAgent: Red Teaming MCP](https://github.com/opena2a-org/hackmyagent/blob/main/docs/use-cases/red-team-mcp.md) - Use case guide for red teaming MCP servers.
- [AI Red Teaming Guide](https://github.com/requie/AI-Red-Teaming-Guide) - Practical guide to AI red teaming methodology.
- [AI Red Teaming by Virdoex_hunter](https://nebulous-gem-db8.notion.site/AI-RED-TEAMING-by-Virdoex_hunter-3e7d108d10ab80d49818eed4e636892c) - Community AI red teaming notes.
- [Yellow Team AI](https://yellowteam.ai/) - AI security project and resources.

## Guardrails & Defensive Tooling

- [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) - NVIDIA toolkit for programmable input, output, and dialog rails.
- [LLM Guard](https://github.com/protectai/llm-guard) - Protect AI's input and output scanners for prompt injection, PII, and secrets.
- [PurpleLlama](https://github.com/meta-llama/PurpleLlama) - Meta's Llama Guard and Prompt Guard classifiers, plus CyberSecEval.
- [Presidio](https://github.com/data-privacy-stack/presidio) - PII detection and de-identification for text, images, and structured data, useful for redacting prompts and model outputs. Maintained by [Data Privacy Stack](https://github.com/data-privacy-stack).
- [Protect AI](https://github.com/protectai) - Open-source AI/ML security tools from Protect AI.
- [Pipelock](https://github.com/luckyPipewrench/pipelock) - Open-source AI agent firewall for verifiable egress control.
- [Laya Security Guardrail](https://github.com/shashvik/laya-security-guardrail) - Local, non-generative classifier suite for low-latency security inspection.
- [SkillSpector](https://github.com/NVIDIA/SkillSpector) - NVIDIA tool for inspecting agent skills.
- [Defending Code Reference Harness](https://github.com/anthropics/defending-code-reference-harness) - Anthropic reference harness for code defense evaluation.

## AI Gateways

Proxies sitting between applications and model providers. A good place to enforce authentication, key isolation, rate limits, guardrails, and audit logging.

- [Bifrost](https://github.com/maximhq/bifrost) - High-performance gateway unifying 20+ providers behind one OpenAI-compatible API, with failover and governance.
- [LiteLLM](https://github.com/BerriAI/litellm) - Python SDK and proxy for 100+ LLMs with virtual keys, spend tracking, and guardrail hooks.
- [Portkey AI Gateway](https://github.com/Portkey-AI/gateway) - Gateway routing to 250+ LLMs with fallbacks, retries, and guardrails.
- [agentgateway](https://github.com/agentgateway/agentgateway) - Open-source LLM, MCP, and A2A proxy with built-in security, guardrails, and observability.
- [Agent Router (formerly Envoy AI Gateway)](https://github.com/envoyproxy/ai-gateway) - Envoy-based gateway for models and MCP servers with centralized credentials, quotas, and attribution.
- [Kong Gateway](https://github.com/Kong/kong) - API, LLM, and MCP gateway with AI plugins for multi-LLM routing and semantic security.
- [TensorZero](https://github.com/tensorzero/tensorzero) - Low-latency LLM gateway combined with observability, evaluation, and optimization.
- [Helicone](https://github.com/Helicone/helicone) - AI gateway and LLM observability platform with routing, fallbacks, and agent tracing.

## Detection Engineering & Monitoring

- [Uber ADR](https://github.com/uber/ADR) - Agentic AI Detection and Response: discovery, observability, detection, and prevention for enterprise agents.
- [OpenTelemetry GenAI Semantic Conventions](https://opentelemetry.io/docs/specs/semconv/gen-ai/) - Standard telemetry schema for model calls, agent spans, and tool use. A good logging baseline for AI detections.

## Model & Supply Chain Security

- [ModelScan](https://github.com/protectai/modelscan) - Scans serialized models for unsafe code across formats.
- [picklescan](https://github.com/mmaitre314/picklescan) - Detects dangerous imports in Python pickle files.
- [fickling](https://github.com/trailofbits/fickling) - Trail of Bits decompiler, static analyzer, and rewriter for pickle files.
- [safetensors](https://github.com/huggingface/safetensors) - Safe tensor serialization format that avoids arbitrary code execution.
- [model-transparency](https://github.com/sigstore/model-transparency) - Sigstore-based model signing and verification.
- [OWASP AIBOM Generator](https://huggingface.co/spaces/GenAISecurityProject/OWASP-AIBOM-Generator) - Generate AI Bills of Materials for Hugging Face models.
- [AI SBOM Generator](https://aisuf.org/blogs/f/ai-sbom-generator) - AISUF write-up and tool for AI SBOMs.
- [How Abliterated Models Can Get You Pwned](https://projectdiscovery.io/research/how-abliterated-models-can-get-you-pwned) - ProjectDiscovery research on risks of safety-stripped models.
- [Poison in the Pipeline](https://0din.ai/blog/poison-in-the-pipeline-liberating-models-with-basilisk-venom) - 0DIN research on training-pipeline poisoning.

## Agent, MCP & Memory Security

- [MCP Security Best Practices](https://modelcontextprotocol.io/specification/draft/basic/security_best_practices) - Official Model Context Protocol security guidance.
- [mcp-scan](https://github.com/invariantlabs-ai/mcp-scan) - Scanner for MCP servers: tool poisoning, rug pulls, and cross-origin escalation.
- [MCP Security Demo](https://github.com/k8sautom8/mcp-security-demo) - Vulnerable MCP setup for practicing MCP attacks.
- [Agent Memory: Build, Break, Secure](https://www.ryvane.ai/journal/agent-memory-build-break-secure) - Attacks on and defenses for agent memory.
- [Context Bombs](https://agentic.tracebit.com/context-bombs/) - Tracebit research on context-based attacks against agents.

## OSINT, Recon & Secrets Exposure

Exposed inference servers, unauthenticated AI dashboards, and leaked LLM provider keys or model-hub tokens are among the most common real-world AI compromises.

### Internet Exposure Search

- [Censys](https://censys.com/) - Internet-wide host and certificate search engine for finding exposed AI services such as Ollama, vLLM, and Open WebUI.
- [Shodan](https://www.shodan.io/) - Search engine for internet-connected devices, widely used to enumerate exposed LLM servers.
- [Detecting Exposed LLM Servers: A Shodan Case Study on Ollama](https://blogs.cisco.com/security/detecting-exposed-llm-servers-shodan-case-study-on-ollama) - Cisco research on discovering and fingerprinting publicly exposed Ollama instances.

### Recon & Asset Discovery

- [OWASP Amass](https://github.com/owasp-amass/amass) - Attack surface mapping and external asset discovery from open sources and active recon.
- [subfinder](https://github.com/projectdiscovery/subfinder) - Passive subdomain enumeration for scoping AI endpoints and staging environments.
- [Nuclei](https://github.com/projectdiscovery/nuclei) - Template-based vulnerability scanner.
- [nuclei-templates](https://github.com/projectdiscovery/nuclei-templates) - Community templates, including detections for exposed Ollama, vLLM, LiteLLM, Open WebUI, Flowise, Langflow, MLflow, Ray, and Jupyter.

### Secrets Scanning

- [TruffleHog](https://github.com/trufflesecurity/trufflehog) - Finds, verifies, and analyzes leaked credentials across git, cloud, and SaaS sources.
- [Gitleaks](https://github.com/gitleaks/gitleaks) - Fast secret scanner for git repositories, files, and pre-commit hooks.

## Benchmarks & Evaluations

- [AgentDojo](https://github.com/ethz-spylab/agentdojo) - Dynamic environment for evaluating prompt injection attacks and defenses on tool-using agents.
- [InjecAgent](https://github.com/uiuc-kang-lab/InjecAgent) - Benchmark for indirect prompt injection in tool-integrated agents.
- [HarmBench](https://github.com/centerforaisafety/HarmBench) - Standardized evaluation framework for automated red teaming and refusal robustness.
- [CyberSecEval](https://github.com/meta-llama/PurpleLlama/tree/main/CybersecurityBenchmarks) - Meta's benchmarks for cybersecurity risks and capabilities of LLMs.
- [Inspect](https://github.com/UKGovernmentBEIS/inspect_ai) - UK AI Security Institute's framework for LLM evaluations.

## AI in OT & Critical Infrastructure

- [Deploying AI Systems Securely](https://media.defense.gov/2024/Apr/15/2003439257/-1/-1/0/CSI-DEPLOYING-AI-SYSTEMS-SECURELY.PDF) - NSA-led joint guidance for operating externally developed AI systems.
- [Principles for the Secure Integration of AI in OT](https://www.cisa.gov/resources-tools/resources/principles-secure-integration-artificial-intelligence-operational-technology) - CISA and partners' guidance for AI in operational technology environments.

## Incident Response & Operations

- [Agentic Incident Response with Human Approval](https://pisinger.github.io/posts/agentic-incident-response-foundry-logic-apps-human-approval/) - Agentic IR with Azure AI Foundry, Logic Apps, and human-in-the-loop.
- [OpenSRE](https://github.com/Tracer-Cloud/opensre) - Open-source AI SRE agent tooling.

## Incidents & Threat Intelligence

- [AI Incident Database](https://incidentdatabase.ai/) - Index of real-world harms and near-harms caused by AI systems.
- [AVID](https://avidml.org/) - AI Vulnerability Database of failure modes and vulnerability reports.
- [Adversarial Misuse of Generative AI](https://cloud.google.com/blog/topics/threat-intelligence/adversarial-misuse-generative-ai) - Google Threat Intelligence on how threat actors use Gemini.

## Vulnerability Research & Bug Bounty

- [AI Vulnerability Exploitation for Initial Access](https://cloud.google.com/blog/topics/threat-intelligence/ai-vulnerability-exploitation-initial-access) - Google Threat Intelligence on AI-assisted exploitation.
- [Security Research Without Asking Permission](https://www.provos.org/p/security-research-without-asking-permission/) - Niels Provos on AI-driven security research.
- [Agentic Bug Hunter](https://github.com/Awarexone/Agentic-Bug-Hunter) - Agent-based bug hunting.
- [reverse-skill](https://github.com/zhaoxuya520/reverse-skill) - Agent skill for reverse engineering.
- [honeyslop](https://github.com/gadievron/honeyslop/) - Code canaries for triaging AI-hallucinated vulnerability reports.

## Foundational Papers & Research

- [Not What You've Signed Up For](https://arxiv.org/abs/2302.12173) - Greshake et al., the paper that defined indirect prompt injection.
- [Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043) - Zou et al., the GCG adversarial suffix attack.
- [Extracting Training Data from Large Language Models](https://arxiv.org/abs/2012.07805) - Carlini et al. on memorization and training-data extraction.
- [Sleeper Agents](https://arxiv.org/abs/2401.05566) - Hubinger et al. on backdoored LLMs that persist through safety training.
- [The Assistant Axis](https://www.anthropic.com/research/assistant-axis) - Anthropic research on assistant persona stability and model behavior.

## Training, CTFs & Labs

### Courses

- [LLM Training for Cybersecurity](https://sachin-sharma.gitbook.io/llm-training-for-cybersecurity) - GitBook course on LLMs for security.
- [AISec University](https://aisec.university/courses) - AI security courses.
- [TryHackMe: AI Security Path](https://tryhackme.com/path/outline/aisecurity) - Hands-on AI security learning path.

### CTFs & Competitions

- [Gandalf](https://gandalf.lakera.ai/) - Lakera's progressive prompt injection challenge.
- [Crucible](https://crucible.dreadnode.io/) - Dreadnode's AI red teaming CTF platform.
- [HackAPrompt](https://www.hackaprompt.com/) - Prompt hacking competition and dataset.
- [DARPA AI Cyber Challenge (AIxCC)](https://aicyberchallenge.com/) - DARPA competition for AI-driven vulnerability discovery and patching.
- [OWASP FinBot CTF](https://owasp-finbot-ctf.org/portals) - OWASP agentic AI CTF in a fintech scenario.
- [Matrix AI Agent CTF](https://github.com/alexdevassy/Machine_Learning_CTF_Challenges/tree/master/Matrix_AI_Agent_CTF_Challenge) - Agent-focused ML CTF challenge.

### Demo Environments

- [Damn Vulnerable LLM Agent](https://github.com/WithSecureLabs/damn-vulnerable-llm-agent) - WithSecure's intentionally vulnerable ReAct agent for injection practice.
- [OpenA2A Demos](https://opena2a.org/demos) - Agent security demos.

---

## Contributing

Pull requests welcome. Please:

1. Add one link per PR where possible, in the most fitting section.
2. Use the format `- [Name](link) - Short description.` The description must say what the resource does, not who made it.
3. Prefer original sources over aggregators; no paywalled or pirated content.
4. Resources must be AI-security specific (or, like secret scanners, directly address a common AI attack path) and actively maintained.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the maintainers have waived all copyright and related rights to this work.
