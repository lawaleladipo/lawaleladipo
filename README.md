# Olawale Oladipo

Detection and Response Engineer | Cloud and endpoint DFIR | AI tooling for security operations

I write detections as code, investigate incidents across cloud, identity and endpoint telemetry, and build AI tooling for security operations that analysts can review and control. My work covers SIEM, EDR, CNAPP and Kubernetes environments.

## Focus areas

- Detection as code: behavioural detections written and linted in CI for Google SecOps (YARA-L 2.0), CrowdStrike Falcon (CQL, Custom IOAs, IOC APIs) and Wiz (OPA Rego, KQL, Security Graph controls, shift-left IaC).
- Detection quality: Median/MAD baselines for rule noise, log-source downtime, ingestion latency and allow-list hygiene.
- Cloud and identity DFIR: reconstructing incidents that span WAF, Kubernetes, cloud IAM, identity and SSO, SASE and DLP, and endpoints.
- AI for security operations: browser-side redaction of PII and secrets, and deterministic pre-flight compilers and linters.

## Projects

| Project | Description | Stack |
| :--- | :--- | :--- |
| [SIFT-AIR](https://github.com/lawaleladipo/sift-air) | DFIR, threat hunting and multi-platform detection-as-code workbench. Parses `.pdf` and `.docx` advisories and redacts secrets in the browser. | TypeScript, React 19, Vertex AI / Gemini, YARA-L 2.0, Falcon CQL/IOA/IOC, Wiz Rego/KQL/Graph |
| RulePulse (architecture case study, not public) | Read-only agent for detection quality and SIEM drift. Uses 12-week Median/MAD baselines for rule noise and log health, audits detection files statically, and limits LLM second opinions to bounded checks. | Python, Median/MAD, YARA-L AST, Docker, cost ledger |
| [AI SOC Autonomous Agents](https://github.com/lawaleladipo/ai-soc-autonomous-agents) | Multi-agent SecOps microservice for triage, threat detection, threat hunting, CVE risk and incident documentation. Weights false positives around maintenance windows, uses a P1 to P5 priority matrix and has fallback scorers. | Python, FastAPI, Groq (Llama 3.3), Docker, ReportLab, MITRE ATT&CK |
| [Omni-Scraper](https://github.com/lawaleladipo/omni-scraper) | Crawler and leak-hunting CLI for `.onion` sites. Uses `socks5h://` to prevent DNS leaks, rotates Tor circuits with `stem` `NEWNYM`, checks breaches through Intelligence X and correlates hosts with Shodan. | Python, Click, aiohttp-socks, Tor/Stem, IntelX, Shodan |
| [FishAgent](https://github.com/lawaleladipo/FishAgent) | Phishing triage CLI for raw RFC 5322 `.eml` files. Checks DMARC and DKIM alignment, PSL lookalike domains and HTML `<a href>` spoofing, then scores intent with an LLM at `temperature=0`. | Python, BytesParser, tldextract, OpenAI |

## Technical stack

YARA-L 2.0, CrowdStrike CQL and Custom IOA (RE2), OPA Rego, KQL, Python, TypeScript, GCP, AWS, Kubernetes, Terraform, GitLab CI, GitHub Actions, MITRE ATT&CK

## Links

- Medium: [medium.com/@lawaleladipo](https://medium.com/@lawaleladipo)
- LinkedIn: [linkedin.com/in/olawale-oladipo-cybersecurity](https://www.linkedin.com/in/olawale-oladipo-cybersecurity/)
- Email: [lawaleladipo@gmail.com](mailto:lawaleladipo@gmail.com)
