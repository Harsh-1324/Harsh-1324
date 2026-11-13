<div align="center">
  <img src="assets/grid-banner.svg" alt="Harsh Gupta — AI-Native Software Engineer" width="100%" />
  <br />
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=18&duration=3000&pause=1000&color=FF6B00&center=true&vCenter=true&width=850&lines=Building+Deterministic+Systems+Around+Stochastic+AI+Models;Multi-Agent+Orchestration+%7C+Full-Stack+Microservices+%7C+Cloud+Architecture;State-Level+AI+Hackathon+Winner+%7C+Published+Author+%7C+SIH+Team+Lead;Turning+Complex+Data+Schemas+into+Autonomous+Decision+Engines" alt="Engineering Focus" />

  <p align="center">
    <a href="https://www.linkedin.com/in/harsh-gupta" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    <a href="https://leetcode.com/u/harshhgupta13/" target="_blank"><img src="https://img.shields.io/badge/LeetCode-harshhgupta13-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
    <a href="mailto:harshhgupta1324@gmail.com"><img src="https://img.shields.io/badge/Email-Let's_Talk-FF6B00?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
    <img src="https://komarev.com/ghpvc/?username=Harsh-1324&label=PROFILE+VISITS&color=FF6B00&style=for-the-badge" alt="Profile Views" />
  </p>
</div>

---

## ⚡ The Engineering Philosophy

> *"Anyone can wrap an API call around an LLM and call it a demo. Real software engineering begins when you have to make a probabilistic model behave deterministically inside a fault-tolerant production system."*

Hi, I'm **Harsh** — a Computer Engineering undergraduate at **MET's Institute of Engineering** and a **Full-Stack & Agentic AI Engineer**. While most developers treat Backend Systems and Artificial Intelligence as two separate worlds, I build at the exact seam where they meet.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🧠 What Makes My Approach Different</h3>
      <ul>
        <li><b>Guardrails Before Generation:</b> I don't trust raw model outputs near production data. I build Abstract Syntax Tree (<code>SQLGlot</code>) validators, strict JSON-Schema contracts, and Human-in-the-Loop (HITL) gates.</li>
        <li><b>OLTP vs. OLAP Separation:</b> I design systems where AI-driven analytical workloads run in isolated in-memory sandboxes (<code>DuckDB</code>) so they never lock transactional customer databases (<code>PostgreSQL</code>).</li>
        <li><b>Algorithmic Backbone:</b> Daily problem-solver in <b>Java</b> across Dynamic Programming, Graph Theory, and Bit Manipulation—bringing clean time/space complexity discipline to system design.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>🎯 Current Engineering Radar</h3>
      <ul>
        <li><b>Stateful Multi-Agent Topologies:</b> Orchestrating cyclic planner-critic reflection loops using <code>LangGraph</code> and the <code>Model Context Protocol (MCP)</code>.</li>
        <li><b>Schema-Driven Generative UI:</b> Translating unstructured human intent into live, validated <code>React</code> component trees and interactive BI dashboards.</li>
        <li><b>Zero-Day Threat Heuristics:</b> Combining lexical feature extraction with soft-voting gradient boosted ensembles for real-time cybersecurity defense.</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🏛️ Interactive System Blueprints (Live Architecture)

*Unlike static text diagrams, the blueprints below are rendered natively via GitHub Mermaid—you can pan, zoom, and inspect the exact data flow of my flagship systems.*

### 1. `OmniDash` — Autonomous Multi-Agent NL-to-SQL & Decision Intelligence
**The Challenge:** Enterprise teams sit on massive relational databases and unstructured PDFs, but non-technical stakeholders cannot write complex multi-join SQL, and engineering teams cannot risk letting an unguarded LLM touch production databases.

```mermaid
flowchart LR
    A[User NL Query / Docs] --> B(Surya-OCR & Hybrid RAG)
    B --> C{LangGraph Orchestrator}
    C -->|Drafts Query| D[Planner Agent]
    D --> E[Critic & Schema Verifier]
    E -->|Self-Correction Loop| D
    E -->|Verified Candidate| F[[SQLGlot AST Security Gate]]
    F -->|Blocks Destructive Ops| G(DuckDB In-Memory Staging)
    G --> H[Interactive React / Plotly BI]

    style A fill:#161B22,stroke:#8B949E,color:#FFFFFF
    style B fill:#161B22,stroke:#38BDF8,color:#FFFFFF
    style C fill:#161B22,stroke:#FF6B00,color:#FF8C00
    style D fill:#0D1117,stroke:#30363D,color:#C9D1D9
    style E fill:#0D1117,stroke:#30363D,color:#C9D1D9
    style F fill:#2A1205,stroke:#FF6B00,color:#FF6B00
    style G fill:#161B22,stroke:#38BDF8,color:#FFFFFF
    style H fill:#161B22,stroke:#FF9E00,color:#FFFFFF
```

* **How It Works:** Ingests both relational schemas (`PostgreSQL`) and unstructured documents (`Surya-OCR` + `PGVector`/`ChromaDB`). A stateful `LangGraph` workflow plans the query, critiques join paths, passes the SQL through an AST syntax blocker (`SQLGlot`) to guarantee read-only safety, stages aggregations in `DuckDB`, and streams visual insights to a `React` frontend.
* **Why It Matters:** Published as a primary research paper, awarded **1st Runner-Up at Project Poster Presentation 2K26**, and built as our flagship system for **Smart India Hackathon (SIH)**.

---

### 2. `ApexPhishGuard` — Multi-Model Soft-Voting Threat Intelligence Engine
**The Challenge:** Traditional blacklists fail against newly minted, zero-day phishing domains, while heavy deep-learning models introduce too much latency for real-time browser and email inspection.

```mermaid
flowchart LR
    U[Incoming URL / Email Payload] --> P(Lexical & Structural Parser)
    U --> T(TF-IDF N-Gram Vectorizer)
    P --> F[Feature Fusion Matrix]
    T --> F
    F --> M1[Logistic Regression]
    F --> M2[Random Forest]
    F --> M3[LightGBM Classifier]
    M1 & M2 & M3 --> V[[Soft-Voting Probability Aggregator]]
    V --> R([Real-Time Threat Verdict API])

    style U fill:#161B22,stroke:#8B949E,color:#FFFFFF
    style P fill:#0D1117,stroke:#38BDF8,color:#C9D1D9
    style T fill:#0D1117,stroke:#38BDF8,color:#C9D1D9
    style F fill:#161B22,stroke:#FF9E00,color:#FFFFFF
    style V fill:#2A1205,stroke:#FF6B00,color:#FF6B00
    style R fill:#161B22,stroke:#FF6B00,color:#FFFFFF
```

* **How It Works:** Extracts structural URL lexical signatures alongside TF-IDF token vectors, feeding them concurrently into a calibrated ensemble of `Logistic Regression`, `Random Forest`, and `LightGBM` exposed via a low-latency REST microservice.
* **Why It Matters:** Outperformed standalone classifiers in false-positive suppression and clinched **🏆 1st Place at the upXgen State-Level Hackathon (AI Domain)**.

---

### 3. Production Full-Stack & Predictive Engines
| System | Architectural Problem Solved | Core Engineering Stack |
| :--- | :--- | :--- |
| **[Forma-AI](https://github.com/Harsh-1324/Forma-AI-AI-Augmented-Dynamic-Form-Engine)** | Eliminates manual form-builder boilerplate by converting natural language prompts into strict, schema-validated, interactive UI forms with automated database persistence. | `React.js` `Node.js` `LangChain` `PostgreSQL` `JSON-Schema` |
| **[Foresight](https://github.com/Harsh-1324/foresight-demand-inventory)** | Solves retail stockout and overstock risks by benchmarking gradient-boosted weekly SKU demand curves against seasonal-naive baselines. | `Python` `LightGBM` `Pandas` `Scikit-learn` `Time-Series` |
| **[Customer Segmentation](https://github.com/Harsh-1324/Intelligent-Customer-Segmentation-Behavioral-Analytics)** | Transforms raw transactional logs into actionable behavioral clusters for targeted retention strategies. | `Python` `Unsupervised ML` `Clustering` `Data Pipelines` |
| **[Mastek FinTech Tracker](https://github.com/Harsh-1324/mastek-ml_based_expense_tracker)** | Full-stack polyglot architecture pairing an Express/React web portal with an isolated Python ML microservice for automated expense categorization. | `React.js` `Express` `Python` `REST Microservices` |

---

## 🧰 The Technology Matrix

<div align="center">
  <p>
    <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
    <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" />
    <img src="https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white" />
  </p>
  <p>
    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
    <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
    <img src="https://img.shields.io/badge/LangChain_%2F_LangGraph-1C3C3C?style=for-the-badge&logo=chainlink&logoColor=white" />
    <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
    <img src="https://img.shields.io/badge/Scikit_Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  </p>
  <p>
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
    <img src="https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black" />
    <img src="https://img.shields.io/badge/AWS_Cloud-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=FF9900" />
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  </p>
</div>

---

## 💼 Experience, Leadership & Milestones

* ⚡ **Software Developer — Deployra Private Limited:** Engineering scalable backend architectures, asynchronous API orchestration, and production AI workflow integrations.
* 💻 **Web Development Intern — Sunanda Infotech:** Architected reusable `React.js` frontend component systems and AI-augmented dynamic form workflows for client applications.
* 🏛️ **Technical Advisory Head — SACC (MET Institute of Engineering):** Spearheading architectural code reviews, technical workshops, and mentoring student engineering teams across the department.
* 🏆 **Honours & Recognition:**
  * 🥇 **1st Place Winner** — *upXgen State-Level Hackathon (AI Domain)*
  * 📄 **Primary Research Author** — *Autonomous Multi-Agent Text-to-SQL & Dynamic BI Generation*
  * 🥈 **1st Runner-Up (2nd Prize)** — *Institute Project Poster Presentation 2K26*
  * 🚀 **National Semi-Finalist** — *Mastek Project Deep Blue (Season 11)*
  * ☁️ **Certified** — *AWS Academy Cloud Foundations* & *Quantum Computing (IIT Roorkee & C-DAC)*

---

## 🔥 Contribution Velocity & Activity Grid

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=Harsh-1324&theme=dark&hide_border=true&background=0D1117&ring=FF6B00&fire=FF8C00&currStreakLabel=FF8C00&sideNums=FFFFFF&currStreakNum=FFFFFF&dates=8B949E" alt="GitHub Streak" width="82%" />
</div>

<br />

<div align="center">
  <!-- Automated Daily Orange Contribution Snake -->
  <img src="https://raw.githubusercontent.com/Harsh-1324/Harsh-1324/output/github-contribution-grid-snake-dark.svg" alt="Contribution Grid Snake" width="100%" />
</div>

---

<div align="center">
  <samp>
    <b>Designed &amp; Engineered by Harsh Gupta</b> • Always open to discussing Distributed Systems, Agentic AI &amp; SDE Opportunities
  </samp>
</div>
