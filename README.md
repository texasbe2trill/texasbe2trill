<div align="center">

<h1>Chris Campbell</h1>

<a href="https://github.com/texasbe2trill">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2600&pause=900&color=58A6FF&center=true&vCenter=true&width=720&lines=Security+engineering+%E2%86%92+Data+Science;End-to-end+ML+on+real+datasets;Calibration+%C2%B7+Validation+%C2%B7+Applied+LLMs" alt="typing header" />
</a>

### Real data. Measured outcomes. Shipped systems.

<p>
  <img src="https://img.shields.io/badge/8%2B_yrs-Security_Engineering-0a66c2?style=flat-square" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <a href="https://bsky.app/profile/texasbe2trill.bsky.social"><img src="https://img.shields.io/badge/BlueSky-@texasbe2trill-0285FF?style=flat-square&logo=bluesky&logoColor=white" /></a>
</p>

</div>

---

## 🎯 What I Do

I build data science and ML systems end to end, then ship them. Feature engineering, calibration, validation, the unglamorous work that decides whether a model is actually useful. By day, I'm a security engineer building Python forensic automation and applied LLM workflows over high-volume operational and behavioral data.

<sub>**Currently exploring:** regime-aware recalibration, LLM grounding, and time-aware validation patterns for production model bundles.</sub>

<table>
<tr>
<td align="center" width="33%">
<h3>🛡️ Security</h3>
<b>MITRE ATT&CK triage</b><br>
<sub>Free-text incidents → calibrated triage cards via hybrid classifier + LLM rationale</sub>
</td>
<td align="center" width="34%">
<h3>📊 Data Science</h3>
<b>R² 0.615 PRA holdout</b><br>
<sub>Calibrated regressors, time-aware validation, regime-aware bundles (n_test 43K)</sub>
</td>
<td align="center" width="33%">
<h3>🤖 Applied LLMs</h3>
<b>4 pluggable backends</b><br>
<sub>OpenAI · Anthropic · Hugging Face · local llama.cpp — structured extraction & rationale</sub>
</td>
</tr>
</table>

---

## 🚀 Featured Project: AlertSage

<table>
<tr>
<td width="62%" valign="top">

### Open-Source SOC Console
<sub>**Python · scikit-learn · sentence-transformers · Streamlit · LLMs · SQLite**</sub>

Free-text security incident in, MITRE ATT&CK triage card out. A TF-IDF + sentence-transformer hybrid handles the fast first pass. An LLM (OpenAI, Anthropic, Hugging Face, or local llama.cpp) commits to the verdict and writes the rationale. SQLite backs case management, bookmarks, timelines, and batch processing up to 500 rows.

<p align="center">
  <img src="https://img.shields.io/badge/Free--Text_Incident-555?style=for-the-badge" />
  <br>↓<br>
  <img src="https://img.shields.io/badge/Hybrid_Classifier-~1.4s-0a66c2?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <br><sub>TF-IDF + sentence-transformer</sub><br>↓<br>
  <img src="https://img.shields.io/badge/LLM_Rationale-~5s-8B5CF6?style=for-the-badge" />
  <br><sub>OpenAI · Anthropic · HF · local llama.cpp</sub><br>↓<br>
  <img src="https://img.shields.io/badge/MITRE_ATT%26CK_Triage_Card-instant-FF4B4B?style=for-the-badge" />
</p>

</td>
<td width="38%" valign="top" align="center">

<a href="https://alertsage.streamlit.app">
  <img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
</a>
<br><br>
<a href="https://github.com/texasbe2trill/AlertSage">
  <img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>
<br><br>
<br>

<sub>🎯 MITRE ATT&CK-mapped output</sub><br>
<sub>🔌 4 pluggable LLM backends</sub><br>
<sub>⚡ Fast classifier + LLM rationale</sub><br>
<sub>💾 SQLite case management</sub><br>
<sub>📊 Batch up to 500 rows</sub>

<br><br>

<a href="https://github.com/texasbe2trill/AlertSage/stargazers">
  <img src="https://img.shields.io/github/stars/texasbe2trill/AlertSage?style=social" />
</a>
&nbsp;
<a href="https://github.com/texasbe2trill/AlertSage/network/members">
  <img src="https://img.shields.io/github/forks/texasbe2trill/AlertSage?style=social" />
</a>

</td>
</tr>
</table>

---

## 📦 More Projects

<table>
<tr>
<td width="33%" valign="top">

### 🏀 [Hooplytics](https://github.com/texasbe2trill/hooplytics)
<sub>**Python · scikit-learn · pandas · Streamlit**</sub>

End-to-end NBA analytics. 60+ leakage-safe features, 8 calibrated regressors, regime-aware playoff bundle swap, live odds, printable PDFs.

***PRA holdout → R² 0.615 · n_test 43K***

<a href="https://hooplytics.streamlit.app"><img src="https://img.shields.io/badge/Live-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/hooplytics"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

</td>
<td width="34%" valign="top">

### 📚 [KoNotes](https://github.com/texasbe2trill/KoNotes)
<sub>**Python · Streamlit · LLMs · NLP**</sub>

Local-first AI-assisted knowledge analytics. Converts Kobo and Kindle annotations into structured, queryable insight with explainable, rule-based recommendations.

<a href="https://konotes.streamlit.app"><img src="https://img.shields.io/badge/Live-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/KoNotes"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

</td>
<td width="33%" valign="top">

### 🍎 [macos-trust](https://github.com/texasbe2trill/macos-trust)
<sub>**Python · CLI**</sub>

Context-aware macOS trust assessment. Fast evaluation of apps, launch items, and system controls with low false-positive design.

<a href="https://github.com/texasbe2trill/macos-trust"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

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
| **Python data stack** | Python, SQL, pandas, NumPy, statistical reasoning, EDA, reproducible Jupyter workflows |
| **Applied AI** | LLM summarization, structured extraction, text classification, AI-assisted triage and case reporting |
| **Query & detection** | SQL (incl. Snowflake), KQL, Splunk SPL, query optimization, detection-as-code (Panther) |
| **Security domain** | telemetry analysis, forensic automation, investigation analytics, control monitoring |
| **Delivery** | Streamlit dashboards, Typer CLIs, joblib model artifacts, ReportLab reports, REST APIs |

---

## 📊 GitHub

<div align="center">

<img height="160" src="https://github-readme-streak-stats.herokuapp.com/?user=texasbe2trill&hide_border=true&theme=github-dark-blue" />

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&height=2&color=gradient&customColorList=2,6,23,30" width="100%" />

<div align="center">
  <sub>
    <img src="https://komarev.com/ghpvc/?username=texasbe2trill&style=flat-square&color=0a66c2&label=profile+views" />
  </sub>
</div>
