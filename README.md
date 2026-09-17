<h1 align="center">Nandesh Kanagaraju</h1>

<p align="center">
  <b>I build systems that can be <i>checked</i>, not trusted.</b><br>
  LLM tooling on top of production data infrastructure — typed plans, governed semantic layers,<br>
  and an audit trail behind every number.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nandesh-kanagaraju-270a9b276/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:nandeshjeyalakshmi@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/nandeshkanagaraju?tab=repositories"><img src="https://img.shields.io/badge/Projects-181717?style=for-the-badge&logo=github&logoColor=white" alt="Projects"/></a>
</p>

---

### 🧭 Currently

Final-year **B.Tech CS (Computer Science & Business Systems)** at SASTRA University, graduating June 2027.
Most of my time goes into one question: **when an AI system hands you a number, how do you know it's right?**
My answer so far is to take the freedom away from the model — make it emit a typed plan, compile that plan
deterministically, and ship the evidence alongside the answer.

Off-hours I send patches to the data tools I use.

---

### 🚀 What I've shipped

<table>
<tr>
<td width="50%" valign="top">

**[Receipts](https://github.com/nandeshkanagaraju/receipts)** · payments analytics agent<br>
<sub>`Python` `PostgreSQL` `Docker` `GitHub Actions`</sub>

Built for the **Razorpay AI Builders** programme. Ask a question in
**English, Tamil or Hindi** → get a number *plus a receipt*: the plan,
the generated SQL, and the rows it came from.

The model never writes SQL. It emits a typed `QueryPlan` that a
deterministic compiler turns into SQL over a governed semantic layer —
so metric definitions live in one versioned place, not in prompts, and
the same question can't compile two different ways.

Guarded by an integrity charter enforced in CI: an eval suite plus
fault-injection and meta-tests that check the guardrails actually fire.

</td>
<td width="50%" valign="top">

**[Walmart Data Platform](https://github.com/nandeshkanagaraju/walmart-data-project)** · CDC + quality gates<br>
<sub>`Databricks` `dbt` `Airflow` `Delta Lake` `S3` `Postgres`</sub>

Syncs an operational Postgres into a Databricks lakehouse **hourly via
change data capture** — only rows inserted, updated or deleted since the
last run move across six related tables.

Ingestion path chosen per source by how fast it changes: transactional
tables follow the change stream, low-velocity reference data is read in
place from S3 as an external location — no copied duplicate that can drift.

dbt tests at the conformed layer (uniqueness, not-null, referential
integrity, accepted values) fail the run instead of letting bad rows
reach a dashboard. Airflow in Docker owns scheduling, retries and alerts.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[SpecGuard](https://github.com/nandeshkanagaraju/specguard)** · spec-drift detection<br>
<sub>`Python` `LLM evaluation`</sub>

Does the code still do what the spec says? Evidence-cited verdicts, an
adversarial second pass, and **abstention instead of guessing.**

</td>
<td width="50%" valign="top">

**[MCP Server Bridge](https://github.com/nandeshkanagaraju/mcp-server-bridge)** · secure DB access over MCP<br>
<sub>`Python` `MCP` `HTTP+SSE`</sub>

A pure MCP data-access layer: sandboxed SQL execution and schema
introspection, with NL→SQL left to the client.

</td>
</tr>
</table>

---

### 🛠 Open source

| | |
|---|---|
| **[apache/airflow#72625](https://github.com/apache/airflow/pull/72625)** | `region_name` was silently ignored by the Step Functions execution trigger — deferred tasks polled the wrong AWS region. **Merged**, shipped in `apache-airflow-providers-amazon` **9.36.0**. |
| **[PrefectHQ/fastmcp#5030](https://github.com/PrefectHQ/fastmcp/issues/5030)** | A tool with an output schema that returns an unserializable value reports *success* — handing the client a `repr()` string and no structured content. Filed with a reproduction and a fix branch; more findings queued. |

---

### 💼 Experience

**Titan Company Limited** *(A TATA Enterprise)* — Live Project Intern, Systems Dept · Dec 2025
Integrated a hosted image-generation model into a customer-facing **virtual try-on** flow over its
REST API — shipped end to end in three weeks.

🏆 **Meta PyTorch OpenEnv Hackathon × Scaler School of Technology** — final round, **top 100 teams** · Apr 2026

---

### ⚙️ Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,postgres,docker,githubactions,git,github,aws" height="45"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Delta%20Lake-00ADD4?style=flat-square&logo=delta&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
</p>

<p align="center"><sub>
<b>Languages:</b> Python, SQL &nbsp;·&nbsp;
<b>AI &amp; Data:</b> LLM agents, semantic layers, dbt, Airflow, CDC, Delta Lake, data quality testing &nbsp;·&nbsp;
<b>Tools:</b> Databricks, AWS S3, Docker, Git/GitHub, GitHub Actions
</sub></p>

---

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=nandeshkanagaraju&theme=tokyonight" height="150"/>
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=nandeshkanagaraju&theme=tokyonight" height="150"/>
</p>

<p align="center"><sub>📍 Hosur, Tamil Nadu · 📬 <a href="mailto:nandeshjeyalakshmi@gmail.com">nandeshjeyalakshmi@gmail.com</a></sub></p>
