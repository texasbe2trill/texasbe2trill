<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&height=210&text=Chris%20Campbell&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Senior%20Security%20and%20Software%20Engineer&descSize=19&descAlignY=58&animation=fadeIn&section=header&color=0:0d1117%2C55:1f3a68%2C100:1f6feb" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&height=210&text=Chris%20Campbell&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Senior%20Security%20and%20Software%20Engineer&descSize=19&descAlignY=58&animation=fadeIn&section=header&color=0:0a3d91%2C100:1f6feb" />
  <img src="https://capsule-render.vercel.app/api?type=waving&height=210&text=Chris%20Campbell&fontSize=54&fontColor=ffffff&fontAlignY=36&desc=Senior%20Security%20and%20Software%20Engineer&descSize=19&descAlignY=58&animation=fadeIn&section=header&color=0:0a3d91%2C100:1f6feb" width="100%" alt="Chris Campbell, Senior Security and Software Engineer" />
</picture>

<a href="https://github.com/texasbe2trill">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2800&pause=1000&color=58A6FF&center=true&vCenter=true&width=720&lines=Security+engineer+who+ships+software;Detection+%C2%B7+Forensics+%C2%B7+Automation;Wearables+%C2%B7+Applied+LLMs+%C2%B7+Tooling;Python+%C2%B7+Monkey+C+%C2%B7+KQL+%C2%B7+SQL" alt="Security engineer who ships software" />
</a>

<a href="mailto:chris@texasbe2trill.com"><img src="https://img.shields.io/badge/Email-chris%40texasbe2trill.com-0a66c2?style=for-the-badge&logo=maildotru&logoColor=white" alt="Email" /></a>
<a href="https://bsky.app/profile/texasbe2trill.bsky.social"><img src="https://img.shields.io/badge/BlueSky-@texasbe2trill-0285FF?style=for-the-badge&logo=bluesky&logoColor=white" alt="BlueSky" /></a>

</div>

<br>

<table>
<tr>
<td align="center" width="25%">
<h2>5</h2>
<sub>shipped projects<br><b>live or installable</b></sub>
</td>
<td align="center" width="25%">
<h2>22</h2>
<sub>Garmin watch models<br><b>run SolarHarvest</b></sub>
</td>
<td align="center" width="25%">
<h2>700+</h2>
<sub>automated tests<br><b>across my projects</b></sub>
</td>
<td align="center" width="25%">
<h2>13</h2>
<sub>MITRE ATT&amp;CK tactics<br><b>mapped by AlertSage</b></sub>
</td>
</tr>
</table>

## 👋 About Me

I'm a senior security engineer with 8+ years in the field, and I build the software around the security work: automation, detection logic kept in version control, and tools that ship with tests and live deployments. Outside of work I publish open-source projects, from a macOS security scanner and an LLM-assisted alert triage console to a Garmin watch app now live on the Connect IQ Store.

<table>
<tr>
<td align="center" width="33%">
<h3>🛡️ Security Depth</h3>
<b>Detection · Forensics · IR</b><br>
<sub>CVE triage · KQL · detection-as-code</sub>
</td>
<td align="center" width="34%">
<h3>⚙️ Software That Ships</h3>
<b>Tested · Deployed · Maintained</b><br>
<sub>Python · Monkey C · CLIs · Streamlit</sub>
</td>
<td align="center" width="33%">
<h3>🤖 Applied AI</h3>
<b>4 pluggable LLM backends</b><br>
<sub>OpenAI · Anthropic · llama.cpp</sub>
</td>
</tr>
</table>

---

## ☀️ Spotlight: SolarHarvest

<a href="https://github.com/texasbe2trill/SolarHarvest"><img src="https://raw.githubusercontent.com/texasbe2trill/SolarHarvest/main/docs/hero-1440x720.png" width="100%" alt="SolarHarvest pages on Garmin watches" /></a>

**A data field for solar Garmin watches that measures what the sun is actually doing for your battery.** Written in Monkey C, live on the Connect IQ Store, and built for watches that give a data field just 128 KB of memory.

- **Measured, not marketed:** battery drain and gain come from the watch's own 1% steps, and the solar benefit is fitted across activities with a fixed-effects regression.
- **Built for tight hardware:** fits that memory limit with room to spare, computes the sun's position on the watch, and makes no network calls.
- **Shows up in Garmin Connect:** 14 developer FIT fields, checked against real recorded activities.

<p align="center">
  <b>22 watch models · 7 pages · 104 unit tests · 3 screen sizes</b><br><br>
  <a href="https://apps.garmin.com/en-US/apps/b0d0fd86-bc11-4d9a-9f78-40db5c7b7fa0"><img src="https://img.shields.io/badge/Get_it_on-Connect_IQ_Store-1f6feb?style=for-the-badge" alt="Get it on the Connect IQ Store" /></a>
  <a href="https://github.com/texasbe2trill/SolarHarvest"><img src="https://img.shields.io/badge/View_Code-181717?style=for-the-badge&logo=github&logoColor=white" alt="View code" /></a>
</p>

---

## 🚀 More Things I've Built

<table>
<tr>
<td width="50%" align="center" valign="middle">
<a href="https://alertsage.streamlit.app"><img src="https://raw.githubusercontent.com/texasbe2trill/AlertSage/main/docs/images/mitre-ui-dashboard.png" width="100%" alt="AlertSage dashboard" /></a>
</td>
<td width="50%" align="center" valign="middle">
<a href="https://github.com/texasbe2trill/macos-trust"><img src="https://raw.githubusercontent.com/texasbe2trill/macos-trust/main/docs/demo.gif" width="100%" alt="macos-trust scan in a terminal" /></a>
</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛡️ [AlertSage](https://github.com/texasbe2trill/AlertSage)
<sub>**Python · scikit-learn · sentence-transformers · Streamlit · LLMs**</sub>

Free-text security incident in, MITRE ATT&CK triage card out. A fast classifier makes the first pass, then an LLM writes the rationale, with guardrails that fall back to deterministic output when the model drifts from the source text.

***8-class taxonomy · 13 ATT&CK tactics · batch up to 500 rows***

<a href="https://alertsage.streamlit.app"><img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Live app" /></a>
<a href="https://github.com/texasbe2trill/AlertSage"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
<td width="50%" valign="top">

### 🍎 [macos-trust](https://github.com/texasbe2trill/macos-trust)
<sub>**Python · Typer CLI · SARIF 2.1.0 · Homebrew tap**</sub>

A read-only macOS security scanner for unsigned apps, Gatekeeper violations, and suspicious persistence, with vendor-aware risk scoring, entitlements auditing, and SARIF output for GitHub Advanced Security.

***59 passing tests · baseline/diff mode · no network calls***

<a href="https://texasbe2trill.github.io/macos-trust/example-report.html"><img src="https://img.shields.io/badge/Live_Report-0a66c2?style=flat-square&logo=github&logoColor=white" alt="Live report" /></a>
<a href="https://github.com/texasbe2trill/macos-trust"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
</tr>
<tr>
<td width="50%" align="center" valign="middle">
<a href="https://hooplytics.streamlit.app"><img src="https://raw.githubusercontent.com/texasbe2trill/hooplytics/main/docs/assets/player-radar.png" width="100%" alt="Hooplytics player radar chart" /></a>
</td>
<td width="50%" align="center" valign="middle">
<a href="https://konotes.streamlit.app"><img src="https://raw.githubusercontent.com/texasbe2trill/KoNotes/main/docs/screenshots/overview.png" width="100%" alt="KoNotes overview dashboard" /></a>
</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏀 [Hooplytics](https://github.com/texasbe2trill/hooplytics)
<sub>**Python · scikit-learn · pandas · Streamlit**</sub>

NBA player outcome models built on 60+ leakage-safe features covering rolling form, matchup context, and rest, evaluated on a chronological split with an automated promotion gate.

***PRA R² 0.615 · 172K train / 43K test rows***

<a href="https://hooplytics.streamlit.app"><img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Live app" /></a>
<a href="https://github.com/texasbe2trill/hooplytics"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
<td width="50%" valign="top">

### 📚 [KoNotes](https://github.com/texasbe2trill/KoNotes)
<sub>**Python · Streamlit · LLMs · NLP**</sub>

A local-first reading tool that turns Kobo and Kindle highlights into searchable notes, with theme clustering, similarity search, LLM chat, and recommendations.

***571 tests · 20+ modules · 7-subcommand CLI***

<a href="https://konotes.streamlit.app"><img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Live app" /></a>
<a href="https://github.com/texasbe2trill/KoNotes"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" alt="Code" /></a>

</td>
</tr>
</table>

---

## 🛠️ Toolbox

<div align="center">

<img src="https://skillicons.dev/icons?i=python,bash,sklearn,linux,kubernetes,git,github,githubactions,vscode" alt="Python, Bash, scikit-learn, Linux, Kubernetes, Git, GitHub, GitHub Actions, VS Code" />

</div>

| | |
|---|---|
| **Security** | detection-as-code (Panther), forensic automation, KQL, Snowflake SQL, CVE triage, macOS trust assessment |
| **Software** | Python, Monkey C (Garmin Connect IQ), Typer CLIs, unit testing, memory- and CPU-constrained devices |
| **Applied&nbsp;AI** | LLM IOC extraction, incident classification, hallucination guardrails, multi-provider routing |
| **Data&nbsp;&amp;&nbsp;ML** | scikit-learn, pandas, SQL, classification, regression, calibration, time-aware validation |
| **Delivery** | Streamlit dashboards, SARIF 2.1.0, JSON pipelines, REST APIs, Garmin FIT developer fields |

<sub>**Currently exploring:** on-device statistics for wearables, context-aware security scanning, and LLM grounding for structured extraction.</sub>

---

<div align="center">

## 📫 Let's Talk

Always happy to talk security engineering, tooling, or the projects above.

<a href="mailto:chris@texasbe2trill.com"><img src="https://img.shields.io/badge/Email_Me-0a66c2?style=for-the-badge&logo=maildotru&logoColor=white" alt="Email me" /></a>
<a href="https://bsky.app/profile/texasbe2trill.bsky.social"><img src="https://img.shields.io/badge/Follow_on_BlueSky-0285FF?style=for-the-badge&logo=bluesky&logoColor=white" alt="Follow on BlueSky" /></a>

<img src="https://komarev.com/ghpvc/?username=texasbe2trill&style=flat-square&color=0a66c2&label=profile+views" alt="Profile views" />

</div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:1f6feb%2C45:1f3a68%2C100:0d1117" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:1f6feb%2C100:0a3d91" />
  <img src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:1f6feb%2C100:0a3d91" width="100%" alt="" />
</picture>
