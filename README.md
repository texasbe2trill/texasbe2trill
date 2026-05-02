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
<h3>215K</h3>
<sub>row chronological train/test split across 8 NBA targets</sub>
</td>
<td align="center" width="34%">
<h3>R² 0.615</h3>
<sub>PRA holdout, chronological split (n_test = 43K)</sub>
</td>
<td align="center" width="33%">
<h3>4</h3>
<sub>shipped open-source projects, 3 with live apps</sub>
</td>
</tr>
</table>

---

## 🚀 Featured Project: Hooplytics

<table>
<tr>
<td width="62%" valign="top">

### NBA Player Analytics & Decision-Support Platform
<sub>**Python · scikit-learn · pandas · Streamlit · Typer · joblib**</sub>

End-to-end ML platform: ingest game logs, engineer 60+ leakage-safe features, train and calibrate 8 regressors, swap in a regime-aware playoff bundle when the post-season hits, and ship the result through a Streamlit app, a CLI, and printable PDFs.

**Held-out R² (chronological split, n_test = 43,000):**

| Target | R² | MAE | | Target | R² | MAE |
|:--|--:|--:|:--|:--|--:|--:|
| **PRA** | **0.615** | 6.03 | | Rebounds | 0.499 | 1.89 |
| Fantasy | 0.571 | 7.81 | | Turnovers | 0.336 | 0.87 |
| Points | 0.540 | 4.59 | | 3PM | 0.305 | 0.89 |
| Assists | 0.530 | 1.39 | | STL+BLK | 0.193 | 0.95 |

</td>
<td width="38%" valign="top" align="center">

<a href="https://hooplytics.streamlit.app">
  <img src="https://img.shields.io/badge/▶_Live_App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
</a>
<br><br>
<a href="https://github.com/texasbe2trill/hooplytics">
  <img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>
<br><br>
<a href="https://github.com/texasbe2trill/hooplytics">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=texasbe2trill&repo=hooplytics&theme=github_dark&hide_border=true" />
</a>

</td>
</tr>
</table>

---

## 📦 More Projects

<table>
<tr>
<td width="33%" valign="top">

### 🚨 [AlertSage](https://github.com/texasbe2trill/AlertSage)
<sub>**Python · Jupyter · scikit-learn**</sub>

Reusable workflow for security alert classification: TF-IDF and lexical features, calibrated thresholds, and a structured evaluation harness for repeatable model comparison.

<a href="https://alertsage.streamlit.app"><img src="https://img.shields.io/badge/Live-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" /></a>
<a href="https://github.com/texasbe2trill/AlertSage"><img src="https://img.shields.io/badge/Code-181717?style=flat-square&logo=github&logoColor=white" /></a>

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
