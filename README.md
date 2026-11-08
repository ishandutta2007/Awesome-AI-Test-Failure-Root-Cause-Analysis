# Awesome-AI-Test-Failure-Root-Cause-Analysis

# Awesome-AI-Test-Failure-Root-Cause-Analysis
**Top AI Test Failure Root Cause Analysis (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Failure Triage, Flaky Test Detection, Test Impact Analysis & Self-Hosted Test Intelligence*
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Test Failure & Root Cause Analysis**. These tools enable engineering and QA teams to stop scrolling logs and start fixing problems—automatically classifying failures, correlating them with code changes, and recommending fixes before engineers lose hours to investigation.

**Examples** include BrowserStack Test Failure Analysis Agent, Datadog Test Optimization, Sauce Labs Failure Analytics, Launchable, Testkube AI, ReportPortal, Develocity Predictive Test Selection, Sentry Seer, SeaLights, and Thundra Foresight (the category leaders in commercial and open-source space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted RCA, failure classification, and open test analytics. **Critical note**: The open-source landscape is anchored by **ReportPortal**—the most mature Apache 2.0 test analytics platform with ML-based Auto-Analyzer for failure classification —and **Testkube**—which brought one-click AI analysis to its open-source edition in June 2026 . **TeamCity QA Intelligence** is a newer MCP-based solution specifically for TeamCity users . No open-source project matches BrowserStack's one-click agent with full test-context access or Datadog's test-to-APM correlation, but for self-hosted test intelligence, the options are production-capable.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **BrowserStack Test Failure Analysis Agent**
  **One-click AI root cause analysis** with full test context access. **Features**: Agent combs through logs, test history, and traces to pinpoint root cause; **automatic categorization** as product, environment, or automation bug (or custom categories); **actionable fixes** with recommended next steps . Described as a "real time-saver during triage" by competitors . **Pricing**: Bundled with BrowserStack AI; requires enabled AI and Owner/Admin permissions. **Free tier**: No free tier for AI agent; trial available. **Best for**: teams already on BrowserStack wanting one-click RCA integrated with their automation dashboard—**trade-off**: requires BrowserStack subscription; AI agent gated by plan.

- **Datadog Test Optimization**
  **Test analytics within Datadog observability** with flaky detection and TIA. **Features**: **Early Flake Detection**—retries new tests before merge to catch flakiness; **Auto Test Retries**—retries failing tests to survive nondeterministic failures; **Test Impact Analysis**—runs only tests relevant to a code change using coverage and Git metadata . **Unique advantage**: test-to-APM/RUM correlation only Datadog can provide . **Pricing**: **$20/active committer/month** (annual), $24 month-to-month, $29 on-demand; 1M test spans per committer included, $3 per additional million; CI Pipeline Visibility separate at $8/committer/month . **Free tier**: Trial available. **Best for**: Datadog organizations wanting test intelligence integrated with existing observability—**trade-off**: pricing scales with headcount; less useful if not already on Datadog.

- **Sauce Labs Failure Analytics**
  **Enterprise test analytics** with flaky test identification. **Features**: Test analytics identify systemic flakiness and failure trends across builds; enterprise security (SSO, private device pools, audit trails); Backtrace error monitoring . **Pricing**: **From $39/month** (entry live-testing); automated testing priced by parallel sessions . **Free tier**: Free trial; free tier for open-source projects. **Best for**: enterprises needing cross-build analytics with strong security posture—**trade-off**: **inflexible pricing model** noted by reviewers, challenging for smaller organizations.

- **Launchable**
  **Predictive test selection and flaky insights**. **Features**: **ML model identifies tests with highest probability of failing** based on code and test metadata; **predictive test selection** builds subsets for faster feedback; **flaky test insights**—test session duration, frequency, failure ratio, test entropy measurement . **Pricing**: **Starting at $12,000/year**; usage-based . **Free tier**: Trial available. **Best for**: teams wanting to run fewer tests while catching failures early—**trade-off**: **predictive selection, not RCA**—it tells you what to run, not why something failed.

- **Testkube AI**
  **Native AI agents for failure analysis and remediation**. **Features**: **Advanced failure analysis**—detects patterns across environments, delivers plain-language summary; **investigation time drops from 30 minutes to under 5**; **automated remediation**—analyzes failures, correlates with code changes, generates fixes, opens pull requests (with guardrails: scoped tokens, no auto-merge) . **Free during preview**: Full access at no additional cost while refining . **Pricing**: Free during preview; pricing TBD. **Free tier**: Yes, during preview. **Best for**: teams wanting agentic failure analysis with remediation proposals—**trade-off**: preview status; remediation requires GitHub/GitLab MCP setup.

- **Sentry Seer**
  **AI debugger for runtime errors**. **Features**: Uses stack traces, environment details, spans, commits, logs, and profiling data; **identifies root causes with 94.5% accuracy**; suggests fixes; **opens pull requests automatically**; actionability score prioritizes fixable issues . **Pricing**: **$20/month** includes $25/month in credits; available on any paid Sentry plan . **Free tier**: 14-day trial. **Best for**: teams wanting AI debugging integrated with error monitoring—**trade-off**: **runtime errors, not test failures**—it diagnoses production issues, not CI failures.

- **Develocity Predictive Test Selection**
  **ML-based test selection for Gradle/Maven**. **Features**: **Predictive model** learns from code changes and test outcomes; selects only tests most relevant to a code change; Build Scan shows selected tests and time saved; Predictive Test Selection dashboard visualizes impact . **Pricing**: Commercial; quote-only. **Free tier**: None. **Best for**: enterprises using Gradle/Maven wanting faster feedback—**trade-off**: **test selection, not RCA**; build-system focused.

- **SeaLights**
  **Test Impact Analysis** for CI optimization. **Features**: **TIA**—analyzes code changes in PR and determines impacted tests; only affected tests execute; **build-based or test-cycle-based recommendations**; full run policy ensures data accuracy . **Pricing**: Paid; tiered by lines of code. **Free tier**: None. **Best for**: teams wanting to optimize test execution—**trade-off**: **TIA, not RCA**—it prevents failures by testing the right code.

- **Thundra Foresight**
  **Test debugging and tracing** for CI/CD. **Features**: Demonstrates root cause understanding for erroneous tests using distributed testing and debugging in CI/CD pipelines . **Note**: Limited current search results; appears to be part of Thundra's broader observability platform. **Best for**: teams wanting CI test tracing—**trade-off**: limited public pricing and feature detail in available results.

## Open-Source GitHub Projects

- **ReportPortal**
  **AI-powered test automation dashboard** (Apache 2.0) — **the most mature open-source test analytics platform**, with ML-based Auto-Analyzer for failure classification . **Features**: **Auto-Analysis**—categorizes failures with ML, links defects automatically; **Immediate Auto-Analysis**—kicks off before launch finishes to flag failures sooner; **Pattern Analysis**—define string/regex rules to detect known error patterns; **Unique Error Analysis**—groups identical errors to speed triage; **ML Suggestions**—AI-powered suggestions for similar failures during triage; **models retrain per project** using XGBoost with ~30 features including cosine similarity and Random Forest probability . **Tech stack**: Java, Docker/Kubernetes. **Deploy**: Self-hosted (Apache 2.0, Docker/K8s) or cloud. **Trade-off**: **Report-first platform with ML labels**—not an autonomous agent; requires test result ingestion. **Best for**: teams wanting proven, self-hosted test analytics with ML-based failure classification—especially those already using ReportPortal for test reporting.

- **Testkube**
  **Test orchestration with AI analysis** (open source) — **the most accessible open-source AI test analysis**, with one-click analysis in the OSS edition as of June 2026 . **Features**: **AI Analyze button** at execution and workflow level—generates functional report covering pass/fail trends, resource usage, outliers, and optimization recommendations; **no setup, no prompt crafting**; **baseline report** lets you start conversation with agent from position of understanding; **token consumption visible** in AI chats; AI Agents available for deeper analysis and remediation . **Tech stack**: Kubernetes-native. **Deploy**: Self-hosted (OSS) or cloud. **Trade-off**: **Test orchestration platform first**—AI analysis is a feature, not a standalone RCA tool; requires Testkube for test execution. **Best for**: teams running tests in Kubernetes wanting AI analysis without additional tooling—especially those already using Testkube for orchestration.

- **TeamCity QA Intelligence**
  **Open-source MCP server for TeamCity failure diagnosis** (open source) — **the first QA-focused MCP solution for TeamCity**, built by Kateryna Horshchar . **Features**: **19 read-only tools**—collects and normalizes data from TeamCity (build failures, log excerpts, test history, cross-project failure analysis); **classifies cause** into three categories: code change (linked to specific commit and author), test instability, or infrastructure problem; **recommendations** for fixing each issue; **Claude plugin with 7 commands** for common scenarios; deployed at organizational level, updates propagate in one click . **Tech stack**: MCP server. **Deploy**: TeamCity integration. **Trade-off**: **TeamCity-specific**—not for GitHub Actions, GitLab CI, or Jenkins; newer project with limited validation. **Best for**: TeamCity users wanting AI-powered failure diagnosis without copy-pasting stack traces into chat—especially those with Claude access.

### Additional Strong Open-Source Options

- **No mature open-source equivalent to BrowserStack's one-click agent exists.** BrowserStack, Datadog, Sauce Labs, Launchable, Testkube, Sentry, Develocity, and SeaLights are proprietary. **ReportPortal** provides ML-based classification but not autonomous RCA. **TeamCity QA Intelligence** is CI-specific and newer. For production-grade autonomous RCA, commercial platforms are required.

**Frameworks for building custom systems**: **ReportPortal** provides the ML classification foundation; **Testkube** provides one-click AI analysis for Kubernetes test runs; **TeamCity QA Intelligence** provides MCP-based diagnosis for TeamCity. **None match BrowserStack's one-click agent with full context or Datadog's test-to-APM correlation.**

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Test failure RCA platforms handling test data and application telemetry must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.
- **The "one-click RCA agent" vs. "failure analytics platform" vs. "predictive test selection" vs. "test impact analysis" vs. "MCP diagnosis" distinction is critical.** **BrowserStack Test Failure Analysis Agent** is a **one-click RCA agent**—it analyzes failed tests, categorizes failures, and recommends fixes with full test-context access . **Datadog Test Optimization** is a **failure analytics platform**—flaky detection, retries, and TIA within observability . **Sauce Labs Failure Analytics** is **enterprise test analytics**—cross-build flakiness identification . **Launchable and Develocity** are **predictive test selection**—they optimize what to run, not diagnose failures . **SeaLights** is **test impact analysis**—it analyzes code changes to determine impacted tests . **Testkube** is **orchestration with AI analysis**—one-click reports for Kubernetes test runs . **TeamCity QA Intelligence** is **MCP diagnosis**—it classifies failure cause into three categories . **Sentry Seer** is **runtime error debugging**—not test failures . **Choose based on whether you need autonomous RCA, analytics, test selection, TIA, or CI-specific diagnosis.**
- **BrowserStack's agent is the most complete one-click RCA**—full access to test context inside Test Reporting & Analytics, automatic categorization, and actionable fixes . Competitors acknowledge it as a "real time-saver during triage" .
- **Datadog's unique advantage is test-to-APM correlation**—Playwright test results link to the browser sessions they generated, something only Datadog can do . **The trade-off**: $20/committer/month scales with headcount; less useful if not already on Datadog.
- **Launchable and Develocity are not RCA tools**—they predict which tests to run, not why a failure occurred . **Do not confuse test selection with root cause analysis.**
- **Testkube brought AI analysis to its open-source edition in June 2026**—one-click report covering pass/fail trends, resource usage, outliers, and optimization recommendations . **The trade-off**: requires Testkube for test orchestration; AI analysis is a feature, not standalone.
- **ReportPortal is the most mature open-source test analytics platform**—Apache 2.0, ML Auto-Analyzer with XGBoost and per-project model retraining . **The trade-off**: report-first with ML labels; not an autonomous agent; requires test result ingestion.
- **TeamCity QA Intelligence is the most focused open-source RCA tool**—19 read-only MCP tools, three-category classification (code change, test instability, infrastructure), and Claude plugin . **The trade-off**: TeamCity-specific; newer project with limited validation. **For TeamCity users with Claude access, it fills a real gap.**
- Self-hosted open-source solutions require proper infrastructure (Java/Docker for ReportPortal, Kubernetes for Testkube, TeamCity for QA Intelligence), security hardening, and ongoing maintenance. **Test failure data includes application logs and stack traces**—ensure your deployment meets your organization's security and compliance requirements before ingesting production test results.

---

**Made for QA engineers, test automation leads, and organizations building transparent test intelligence solutions.**
Let's make AI Test Failure Root Cause Analysis more open, data-driven, and debugging-friendly.
