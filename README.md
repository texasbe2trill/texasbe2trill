<div align="center">

<h1>Chris Campbell</h1>

<a href="https://github.com/texasbe2trill">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&width=720&lines=Security+engineering+%C2%B7+Data+Science+%C2%B7+Applied+LLMs;Forensics+%C2%B7+Predictive+models+%C2%B7+Shipped+systems;Python+%C2%B7+KQL+%C2%B7+pandas+%C2%B7+scikit-learn" alt="typing header" />
</a>

### Real data. Measured outcomes. Shipped systems.

<p>
  <img src="https://img.shields.io/badge/8%2B_yrs-Security_Engineering-0a66c2?style=flat-square" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <a href="https://bsky.app/profile/texasbe2trill.bsky.social"><img src="https://img.shields.io/badge/BlueSky-@texasbe2trill-0285FF?style=flat-square&logo=bluesky&logoColor=white" /></a>
  <a href="mailto:chris@texasbe2trill.com"><img src="https://img.shields.io/badge/Email-chris%40texasbe2trill.com-0a66c2?style=flat-square&logo=maildotru&logoColor=white" /></a>
</p>

</div>

---

## 🎯 What I Do

I work at the intersection of security engineering and data science, building forensic automation, predictive models, then shipping them. Eight years of security domain knowledge feeding ML feature sets nobody else thinks to engineer. By day, a senior security engineer building Python automation and applied LLM workflows over high-volume operational data. Outside of work, I ship end-to-end data science and security projects with live deployments, reproducible pipelines, and test suites.

<sub>**Currently exploring:** regime-aware recalibration, context-aware security scanning, and LLM grounding for structured extraction.</sub>

<table>
<tr>
<td align="center" width="33%">
<h3>🛡️ Security Engineering</h3>
<b>Detection · Forensics · IR</b><br>
<sub>Python automation · KQL · forensic analysis · Panther detection-as-code · CVE triage</sub>
</td>
<td align="center" width="34%">
<h3>📊 Data Science</h3>
<b>R² 0.615 PRA holdout</b><br>
<sub>Calibrated regressors · time-aware validation · regime-aware bundles · n_test 43K</sub>
</td>
<td align="center" width="33%">
<h3>🤖 Applied LLMs</h3>
<b>4 pluggable backends</b><br>
<sub>OpenAI · Anthropic · Hugging Face · local llama.cpp · IOC extraction & structured rationale</sub>
</td>
</tr>
</table>

---

## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🛡️ [AlertSage](https://github.com/texasbe2trill/AlertSage): SOC Triage Console
<sub>**Python · scikit-learn · sentence-transformers · Streamlit · LLMs · SQLite**</sub>

Free-text security incident in, MITRE ATT&CK triage card out. A TF-IDF + sentence-transformer hybrid handles the fast first pass. An LLM (OpenAI, Anthropic, Hugging Face, or local llama.cpp) commits to the verdict and writes the rationale, with hallucination guardrails that downgrade to deterministic output when the model diverges from source.

***8-class taxonomy · 13 MITRE ATT&CK tactics · SQLite case management · batch up to 500 rows***

<a href="https://alertsage.streamlit.app"><img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/AlertSage"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

</td>
<td width="50%" valign="top">

### 🏀 [Hooplytics](https://github.com/texasbe2trill/hooplytics): NBA Analytics Platform
<sub>**Python · scikit-learn · pandas · Streamlit · Sports APIs**</sub>

End-to-end analytics platform for NBA player outcomes. 60+ leakage-safe features across rolling windows, role/matchup context, and rest effects. 8 calibrated regressors on a 215K-row chronological holdout. Regime-aware playoff bundle swap lifts PRA R² from 0.615 → 0.695 without retraining.

***PRA R² 0.615 · n_train 172K · n_test 43K · automated promotion gate***

<a href="https://hooplytics.streamlit.app"><img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/hooplytics"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

</td>
</tr>
</table>

---

## 📦 More Projects

<table>
<tr>
<td width="50%" valign="top">

### 🍎 [macos-trust](https://github.com/texasbe2trill/macos-trust)
<sub>**Python · Typer CLI · SARIF 2.1.0 · Homebrew tap**</sub>

Context-aware macOS security scanner. Identifies unsigned apps, Gatekeeper violations, and suspicious persistence mechanisms with smart vendor recognition. Entitlements auditing, browser extension analysis, baseline/diff mode, and SARIF output for GitHub Advanced Security.

***59 passing tests · Homebrew tap · Privacy-first, read-only***

<a href="https://texasbe2trill.github.io/macos-trust/example-report.html"><img src="https://img.shields.io/badge/Live_Report-0a66c2?style=flat-square&logo=github&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/macos-trust"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

</td>
<td width="50%" valign="top">

### 📚 [KoNotes](https://github.com/texasbe2trill/KoNotes)
<sub>**Python · Streamlit · LLMs · NLP**</sub>

Local-first reading intelligence platform. Converts Kobo and Kindle annotations into structured, queryable insight with semantic theme clustering, similarity search, LLM chat integration, and rule-based recommendations.

***571 tests · 20+ modules · 7-subcommand CLI***

<a href="https://konotes.streamlit.app"><img src="https://img.shields.io/badge/Live-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/KoNotes"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

</td>
</tr>
</table>

---

## 🛠️ Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,bash,sklearn,streamlit,linux,git,github,vscode" />

</div>

| | |
|---|---|
| **ML / Modeling** | scikit-learn, classification, regression, calibration, time-aware validation, residual diagnostics, threshold tuning |
| **Security domain** | detection-as-code (Panther), forensic automation, KQL, Snowflake SQL, macOS trust assessment |
| **Applied AI** | LLM IOC extraction, incident classification, hallucination guardrails, multi-provider routing, AI-assisted case reporting |
| **Python data stack** | Python, SQL, pandas, NumPy, statistical reasoning, EDA, reproducible Jupyter workflows |
| **Delivery** | Streamlit dashboards, Typer CLIs, SARIF 2.1.0, JSON pipelines, joblib model artifacts, REST APIs |

---

<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=gradient&customColorList=2,6,23,30" width="100%" />

<div align="center">
  <sub>
    <img src="https://komarev.com/ghpvc/?username=texasbe2trill&style=flat-square&color=0a66c2&label=profile+views" />
  </sub>
</div>
