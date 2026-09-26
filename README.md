<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&height=210&text=Chris%20Campbell&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Blue%20Team%20%C2%B7%20Forensics%20%C2%B7%20Incident%20Command&descSize=24&descAlignY=58&animation=fadeIn&section=header&color=0:0d1117%2C55:1f3a68%2C100:1f6feb" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&height=210&text=Chris%20Campbell&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Blue%20Team%20%C2%B7%20Forensics%20%C2%B7%20Incident%20Command&descSize=24&descAlignY=58&animation=fadeIn&section=header&color=0:0a3d91%2C100:1f6feb" />
  <img src="https://capsule-render.vercel.app/api?type=waving&height=210&text=Chris%20Campbell&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Blue%20Team%20%C2%B7%20Forensics%20%C2%B7%20Incident%20Command&descSize=24&descAlignY=58&animation=fadeIn&section=header&color=0:0a3d91%2C100:1f6feb" width="100%" alt="Chris Campbell: Blue Team · Forensics · Incident Command" />
</picture>

<a href="https://github.com/texasbe2trill">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2800&pause=1000&color=58A6FF&center=true&vCenter=true&width=720&lines=Blue+team%3A+I+investigate%2C+hunt%2C+and+respond;Forensics+%C2%B7+Incident+command+%C2%B7+Threat+hunting;Endpoint%2C+network%2C+and+identity+correlation;LLM-assisted+triage+%C2%B7+Sigma+%C2%B7+KQL+%C2%B7+SPL" alt="Blue team: I investigate, hunt, and respond" />
</a>

<a href="mailto:chris@texasbe2trill.com"><img src="https://img.shields.io/badge/Email-chris%40texasbe2trill.com-0a66c2?style=for-the-badge&logo=maildotru&logoColor=white" alt="Email" /></a>
<a href="https://texasbe2trill.github.io/AlertSage/"><img src="https://img.shields.io/badge/Start_with-AlertSage_docs-1f6feb?style=for-the-badge&logo=materialformkdocs&logoColor=white" alt="Start with the AlertSage docs" /></a>

</div>

<br>

I've spent 8+ years in security, most of it in detection and response: writing detections, hunting threats, running forensics, and serving as incident commander on high-impact incidents. I also build the security tools I want on hand during an investigation. The four security tools on this page are open source, tested, and green in CI, so you can read the code before you take my word for it.

<div align="center">
<table>
<tr>
<td align="center" valign="top" width="50%">
<h2>35%</h2>
<sub>lower average time to mitigate<br><b>KQL over Sentinel and Defender</b></sub>
</td>
<td align="center" valign="top" width="50%">
<h2>&lt;3 min</h2>
<sub>time to acknowledge<br><b>for the response rotation</b></sub>
</td>
</tr>
<tr>
<td align="center" valign="top" width="50%">
<h2>~42%</h2>
<sub>shorter median forensic case time<br><b>about 6h to 3.5h with Python automation</b></sub>
</td>
<td align="center" valign="top" width="50%">
<h2>20</h2>
<sub>open-source Sigma rules<br><b>34 ATT&amp;CK techniques and sub-techniques</b></sub>
</td>
</tr>
</table>
</div>

---

## 🛡️ Spotlight: AlertSage

**AI in the SOC, with a confidence gate.** Paste a free-text incident into this open-source Python console and get a triage card back: incident class, severity, ATT&CK techniques, a playbook hint, and a case record. Its classifier is trained on 500,000 synthetic incidents, and it shows where an LLM helps triage and where it should stay out of the way. An analyst still moves every case from New to Closed.

<p align="center"><a href="https://texasbe2trill.github.io/AlertSage/"><img src="https://raw.githubusercontent.com/texasbe2trill/AlertSage/main/docs/images/bookmarks.png" width="80%" alt="AlertSage Bookmarks page with demo cases and the New, Triaging, Contained, Closed case status stepper" /></a></p>

- **Classifier first.** TF-IDF (5,000 features) plus 384-dimension sentence embeddings feed a logistic regression across 10 incident classes, from phishing and malware to insider threat and data exfiltration.
- **LLM when unsure, by default.** In Fallback mode, the default, the LLM runs only when classifier confidence is low. Off never calls it, and Override sends every event to the LLM. In the demo, a 45%-confidence call took about 1.4 s in the classifier and about 5.8 s in the LLM, and came back as Phishing (ATT&CK T1566 and T1598).
- **Only known labels.** The LLM can override the classifier only with schema-validated JSON and a known label, with synonyms normalized first. If it hedges, a forced second pass runs.
- **Your model, your keys.** Anthropic, OpenAI, Hugging Face, or local llama.cpp, swappable per session, with a fallback when a key is missing.
- **Built for the analyst.** Regex IOC extraction for 10 indicator types, VirusTotal enrichment with your own key, and one-click pivots to AbuseIPDB, Shodan, and GreyNoise.
- **Hunt and track.** A hunt page with Lucene-style queries such as `mitre:T1566 AND last:24h`, case timelines with notes and tags, and CSV batch triage up to 500 rows.

<p align="center">
  <b>Kill-chain view across 13 of 14 ATT&amp;CK Enterprise tactics · 78 tests, CI green</b><br><br>
  <a href="https://texasbe2trill.github.io/AlertSage/"><img src="https://img.shields.io/badge/Docs-1f6feb?style=for-the-badge&logo=materialformkdocs&logoColor=white" alt="Docs" /></a>
  <a href="https://alertsage.streamlit.app"><img src="https://img.shields.io/badge/Live_App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Live app" /></a>
  <a href="https://github.com/texasbe2trill/AlertSage"><img src="https://img.shields.io/badge/View_Code-181717?style=for-the-badge&logo=github&logoColor=white" alt="View code" /></a><br>
  <sub>The live app sleeps when idle: click wake and give it a moment. The docs site is always up.</sub>
</p>

---

## 🚨 Incident Command

I have served as senior incident commander for high-impact security incidents and run every stage of the response:

<p align="center"><b>Triage</b> → <b>Containment</b> → <b>Eradication</b> → <b>Recovery</b> → <b>Root cause</b></p>

- **Malware, ransomware, and data protection incidents:** recognized as incident commander for all three, and led ransomware eradication and recovery.
- **Briefings people can act on:** delivered risk assessments and remediation guidance to engineers and leadership.
- **Identity-aware investigations:** correlated endpoint, network, identity, and behavioral sources to rebuild multi-stage activity.
- **Threat hunting:** led enterprise threat hunting and network forensic analysis, and built the Splunk dashboards and Python automation behind it.
- **For the next responder:** wrote the investigation playbooks and response baselines they start from.
- **AI in my own casework:** used LLMs in production to summarize unstructured case data, triage events, draft investigation notes, and pull IOCs, timestamps, and actor patterns out of free text.

---

## 🧰 More Security Tools

<table>
<tr>
<td width="50%" align="center" valign="top">
<a href="https://github.com/texasbe2trill/ScenarioKit"><img src="https://raw.githubusercontent.com/texasbe2trill/ScenarioKit/main/scenarioKit_storyboard_example.png" width="100%" alt="ScenarioKit storyboard listing matched Sigma rules and ATT&amp;CK techniques" /></a>
</td>
<td width="50%" align="center" valign="top">
<a href="https://github.com/texasbe2trill/macos-trust"><img src="https://raw.githubusercontent.com/texasbe2trill/macos-trust/main/docs/screenshot.png" width="100%" alt="macos-trust scan in baseline mode flagging an invalid code signature" /></a>
</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔎 [ScenarioKit](https://github.com/texasbe2trill/ScenarioKit)
<sub>**Swift CLI · Sigma · Homebrew tap**</sub>

Turns macOS Unified Log JSON into one offline HTML storyboard: a timeline with ATT&CK techniques attached. Its detections live as code: 20 Sigma rules for persistence, TCC, sudo, SSH, keychain access, process injection, and more, run by its own Sigma matcher.

***20 Sigma rules · 34 ATT&CK techniques and sub-techniques · no network calls***

<a href="https://github.com/texasbe2trill/ScenarioKit/blob/main/Sources/ScenarioKit/Resources/Sigma/macos/sigma-macos-rules.yml"><img src="https://img.shields.io/badge/Read_the_rules-6e40c9?style=flat-square&logo=github&logoColor=white" alt="Read the Sigma rules" /></a>
<a href="https://github.com/texasbe2trill/ScenarioKit"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
<td width="50%" valign="top">

### 🍎 [macos-trust](https://github.com/texasbe2trill/macos-trust)
<sub>**Python CLI · SARIF 2.1.0 · Homebrew tap**</sub>

A read-only posture and persistence audit for Macs: unsigned apps, Gatekeeper violations, LaunchAgents and LaunchDaemons, plus kernel and browser extensions. It audits entitlements for 24 sensitive permissions, and baseline mode shows only what changed since your saved baseline. SARIF output drops findings straight into GitHub code scanning.

***59 tests · CodeQL and pip-audit on every push · no network calls or telemetry***

<a href="https://texasbe2trill.github.io/macos-trust/example-report.html"><img src="https://img.shields.io/badge/Live_Report-0a66c2?style=flat-square&logo=github&logoColor=white" alt="Live report" /></a>
<a href="https://github.com/texasbe2trill/macos-trust"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
</tr>
<tr>
<td width="50%" align="center" valign="top">
<a href="https://github.com/texasbe2trill/policyforge"><img src="https://raw.githubusercontent.com/texasbe2trill/policyforge/main/demo-approvals.gif" width="100%" alt="policyforge sending a require_approval decision to the approval queue, a human approving it, then a drift check" /></a>
</td>
<td width="50%" valign="top">

### 🚦 [policyforge](https://github.com/texasbe2trill/policyforge)
<sub>**Go · policy as code · CLI and REST API**</sub>

Guardrails for AI agents and automation that act on production. A YAML policy answers allow, deny, or require_approval after 9 ordered checks. Bots, CI jobs, and AI agents get time-limited policy envelopes, so an expired session is denied. A require_approval decision goes to an approval queue, where a human can approve or reject it. Every decision lands in a SHA-256 hash-linked audit log, and drift detection re-checks past decisions against today's policy.

***61 tests · 3 safety tiers · 4 policy packs · approval workflow***

<a href="https://github.com/texasbe2trill/policyforge"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
</tr>
</table>

<p align="center"><sub><b>205 tests across the four security tools, CI green on all four.</b></sub></p>

---

## 🛠️ Toolbox

<div align="center">

<img src="https://skillicons.dev/icons?i=python,go,swift,bash,linux,kubernetes,git,githubactions" alt="Python, Go, Swift, Bash, Linux, Kubernetes, Git, GitHub Actions" />

</div>

| Function | At work, and in public code you can read |
|---|---|
| **Detection as code** | Python detections in Panther, version controlled and peer reviewed, over high-scale fintech telemetry · **public:** 20 Sigma rules in [ScenarioKit](https://github.com/texasbe2trill/ScenarioKit) |
| **SIEM and query** | Microsoft Sentinel, Splunk, Panther, KQL, SPL, and SQL. Made Snowflake monitoring queries about 20% faster for the on-call rotation. |
| **Endpoint** | Microsoft Defender telemetry · **public:** macOS persistence and code-signing audit in [macos-trust](https://github.com/texasbe2trill/macos-trust) |
| **Cloud and containers** | Daily CVE triage for Kubernetes containers and images; better SQL joins and filters saved about 2 hours per investigation · **public:** guardrails for bots and AI agents acting on infrastructure in [policyforge](https://github.com/texasbe2trill/policyforge) |
| **Hunting and forensics** | Enterprise threat hunting · network forensics · Splunk dashboards · Python artifact collection, log parsing, and enrichment · **public:** Lucene-style search over triaged cases in [AlertSage](https://github.com/texasbe2trill/AlertSage) |
| **AI in the SOC** | LLMs in production for case summaries, IOC extraction, and event triage · **public:** confidence-gated LLM escalation in [AlertSage](https://github.com/texasbe2trill/AlertSage) |
| **Reporting** | Findings turned into clear next steps for engineering and security leaders · **public:** SARIF 2.1.0 for GitHub code scanning, plus JSON and HTML reports, in [macos-trust](https://github.com/texasbe2trill/macos-trust) |
| **Languages** | Python · Go · Swift · KQL · SPL · SQL · Monkey C |

<sub>**Work versus public code:** the Panther, Sentinel, Defender, Splunk, Snowflake, and Kubernetes work above comes from my day jobs and isn't public. The repos on this page are the part you can inspect today. Also: two years managing an enterprise information security governance and risk program.</sub>

---

## 🧭 Beyond Security

Side projects built with the same habits: measure it, test it, ship it.

<table>
<tr>
<td width="42%" align="center" valign="top">
<a href="https://github.com/texasbe2trill/SolarHarvest"><img src="https://raw.githubusercontent.com/texasbe2trill/SolarHarvest/main/docs/hero-1440x720.png" width="100%" alt="SolarHarvest pages on Garmin watches" /></a>
</td>
<td width="58%" valign="top">

### ☀️ [SolarHarvest](https://github.com/texasbe2trill/SolarHarvest)
<sub>**Monkey C · Garmin Connect IQ · live on the Connect IQ Store**</sub>

Connected-device engineering on tight hardware. One codebase runs on 17 Garmin device targets (22 solar watch models), 3 Connect IQ API generations, and 3 screen sizes. It fits the 128 KB data-field limit on the tightest devices. It measures battery drain and solar gain from the watch's own 1% battery steps and records 19 developer FIT fields to every activity.

***112 unit tests across device tiers · 7 pages · no network calls***

<a href="https://apps.garmin.com/en-US/apps/b0d0fd86-bc11-4d9a-9f78-40db5c7b7fa0"><img src="https://img.shields.io/badge/Connect_IQ_Store-1f6feb?style=flat-square" alt="Get it on the Connect IQ Store" /></a>
<a href="https://github.com/texasbe2trill/SolarHarvest"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
</tr>
</table>

- 📚 **[KoNotes](https://github.com/texasbe2trill/KoNotes):** local-first reading analytics with local embeddings, clustering, and LLM chat, plus a 7-subcommand CLI. 645 tests.
- 🏀 **[Hooplytics](https://github.com/texasbe2trill/hooplytics):** NBA player models tested on later games they never saw (R² 0.615 for combined points, rebounds, and assists). A model is saved only if it passes an R² check. 30 tests.

---

<div align="center">

## 📫 Let's Talk

Happy to compare notes on detection engineering, incident response, or putting LLMs to work in triage.

<a href="mailto:chris@texasbe2trill.com"><img src="https://img.shields.io/badge/Email_Me-0a66c2?style=for-the-badge&logo=maildotru&logoColor=white" alt="Email me" /></a>
<a href="https://bsky.app/profile/texasbe2trill.com"><img src="https://img.shields.io/badge/Bluesky-@texasbe2trill.com-0285FF?style=flat-square&logo=bluesky&logoColor=white" alt="Bluesky" /></a>

</div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:1f6feb%2C45:1f3a68%2C100:0d1117" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:1f6feb%2C100:0a3d91" />
  <img src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:1f6feb%2C100:0a3d91" width="100%" alt="" />
</picture>
