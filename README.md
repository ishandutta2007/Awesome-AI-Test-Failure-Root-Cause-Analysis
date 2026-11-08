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

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global software testing and test automation market is estimated at **$50B–$60B in 2025–2026** (with AI-driven automation expanding past **$160B+** at >30% CAGR), while specialized AI test failure triage and automated root cause analysis (RCA) represent its fastest-accelerating frontier. The sector is **moderately to highly fragmented** rather than winner-take-all, split across enterprise observability giants (e.g., Datadog), cross-browser cloud ecosystems (e.g., BrowserStack, Sauce Labs), developer observability leaders (e.g., Sentry), and focused test intelligence startups (e.g., Testkube, Launchable).

## SaaS/Hosted Platforms

| Platform | Company Valuation / Scale | Starting Pricing Tier | Free Tier / Trial Limits | Key RCA & Test Intelligence Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[Datadog Test Optimization](https://www.datadoghq.com/)** | **~$48B Market Cap** ($3.43B FY2025 revenue; NASDAQ: DDOG) | **$20/active committer/month** (annual billing; $24/mo monthly, $29/mo on-demand; includes 1M test spans/committer, $3/additional 1M spans; CI Pipeline Visibility add-on at $8/committer/mo) | **14-day free trial** with full platform access (bounded by evaluation span limits and 1-day retention; no permanent free tier for Test Optimization) | Early flake detection before merge, automated test retries, test impact analysis (TIA), and proprietary correlation connecting test failures directly with APM/RUM production traces. |
| **[BrowserStack Test Failure Analysis Agent](https://www.browserstack.com/)** | **~$4.0B Valuation** (~$225M–$230M ARR; profitable private unicorn) | **$59/month** (entry Automate plan with 1 parallel test; bundled with BrowserStack AI features / Test Observability) | **Free trial with 100 minutes** of automated mobile app testing and **60 minutes** of automated browser testing (no permanent free tier for AI Agent) | One-click autonomous root cause analysis agent; parses logs, execution history, and stack traces to categorize failures into product, environment, or test script bugs with fix suggestions. |
| **[Sentry Seer](https://sentry.io/)** | **~$3.0B Valuation** (~$100M–$120M ARR; Functional Software Inc.) | **$26/month** (Team Plan base; Seer AI features billed at **$20/month** add-on including $25/month AI usage credits) | **Free forever plan ("Developer Plan")**: 1 user, 5,000 error events/mo, 10,000 performance units, 50 session replays/mo, 30-day retention; plus 14-day paid trial | AI root cause analysis across stack traces, commits, and spans with 94.5% diagnostic accuracy; suggests code remediations and can open pull requests autonomously. |
| **[Sauce Labs Failure Analytics](https://saucelabs.com/)** | **~$500M Valuation** (~$92M revenue; backed by TPG & Riverwood Capital) | **$39/month** (Live Testing entry tier; automated testing plans start at **$149/month** per concurrent session) | **28-day free trial**: 60 automated/live testing minutes, up to 3 parallel virtual machines, and sample AI insight queries (free tier available for approved open-source projects) | Enterprise failure pattern analytics across historical test suites, systemic flaky test detection, machine learning failure categorization, and Backtrace error monitoring. |
| **[Catchpoint / Thundra Foresight](https://www.catchpoint.com/)** | **~$250M Acquisition Valuation** (Catchpoint acquired Thundra assets; Catchpoint subsequently acquired by LogicMonitor for >$250M; ~$30M–$58M ARR) | **$10,000/year** (Catchpoint Quick Start synthetic/observability tier using token/factor consumption; WebPageTest developer tier from **$75/month**) | **14-day sales-provisioned free trial** (custom-scoped test credits/nodes; WebPageTest public tier offers ~150 free monthly test runs) | Distributed CI/CD tracing, erroneous test execution diagnosis, and performance bottleneck identification across automated pipelines. |
| **[Develocity Predictive Test Selection](https://develocity.ai/)** | **~$160M Valuation** (~$46M ARR; Gradle Inc.) | **$700/developer/year** (commercial starting baseline tier; quote-only annual committer license for enterprise deployment) | **Free forever on public service** (`scans.gradle.com` provides unlimited individual public Build Scans); 30-day enterprise evaluation trial upon request; free enterprise instances for open-source foundations | Machine learning model trained on code change history and test execution outcomes to select only affected tests; Build Scan failure diagnostics and build caching. |
| **[SeaLights](https://www.sealights.io/)** | **~$150M Acquisition Valuation** (Acquired by Tricentis for $150M in July 2024; raised $50M prior) | **Custom Quote** (Enterprise tier calibrated by active committers and lines of code; typically scales from ~$10,000+/year) | **Sales-provisioned enterprise POC / trial** (typically 14–30 days scoped to designated test suites; no public free tier) | Test Impact Analysis (TIA) analyzing PR pull-request code diffs to isolate and execute only impacted tests; quality governance and release risk scoring. |
| **[Launchable](https://www.launchableinc.com/)** | **~$50M–$100M Valuation Range** (Acquired by CloudBees in August 2024; raised $12.7M prior; founded by Kohsuke Kawaguchi) | **$12,000/year** (Mars for Teams tier starting pricing; enterprise usage-based predictive test selection) | **Free forever plan ("Moon for Developers")**: 1 user limit, includes flaky test notifications and test suite health insights; enterprise POC available | ML predictive test selection ordering tests by probability of failure to shorten feedback loops; flaky test scoring and suite entropy tracking. |
| **[Testkube AI](https://testkube.io/)** | **~$35M–$45M Valuation** ($8M Series A in 2025 led by Insight Partners; Kubeshop spin-off) | **$700/agent/year** (Testkube Pro cloud control-plane; AI features currently in preview at no additional charge) | **Free forever plan (OSS Standalone Edition)**: unlimited runs on self-hosted Kubernetes; **30-day free trial** for cloud-hosted Pro control plane | Native Kubernetes test orchestration with one-click AI failure diagnosis; plain-language summaries, root cause correlation with Git commits, and remediation PR creation via MCP agents. |



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
