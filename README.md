# Alejandro Morgante - Morgan

<p align="center">
  <img width="350" alt="Little Morgan" src="assets/little-morgan.jpeg" />
</p>

<p align="center"><sub><em>
Only those crazy enough to believe they can change the world are the ones who do.<br />
I want to contribute to the world beyond my day-to-day work by leaving a trace of my nerdiness in public, so it can be useful to others.<br />
May what I learn become a path others can walk to get further, faster, just as I once stood on the shoulders of giants.<br />
I try to be a little better every day, treating setbacks as part of the process.
</em></sub></p>

<p align="center">
  <a href="https://almorgan.dev"><strong>almorgan.dev</strong></a>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/AlejandroMorgante/">
    <img src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://medium.com/@AlejandroMorgante">
    <img src="https://img.shields.io/badge/medium-000000.svg?style=for-the-badge&logo=medium&logoColor=white" alt="Medium" />
  </a>
</p>

---

## Now

**Principal Data & AI Architect @ Mendel** — building data and AI platforms.

Writing about agentic data systems on **[Medium](https://medium.com/@AlejandroMorgante)** — agents that debug their own pipelines, multi-agent architectures on AWS, modern data platform design.

Background in database systems through **Universidad Tecnológica Nacional**. Recognized at **Hackathon 2025 - Harvard Health Systems Innovation Lab** for building high-value health systems through AI.

---

### Certified across cloud, data engineering, and AI

<div style="margin-bottom: 4px;">
  <a href="https://www.credly.com/badges/d60e0d36-37b6-409d-8466-c3f46e9e0694/public_url">
    <img src="https://img.shields.io/badge/AWS-Certified%20Data%20Engineer-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" />
  </a>
</div>
<div style="margin-bottom: 4px;">
  <a href="https://www.credly.com/badges/3d402f99-190e-4d53-9fab-4dd024e8cc7a/public_url">
    <img src="https://img.shields.io/badge/AWS-Certified%20AI%20Practitioner-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" />
  </a>
</div>
<div style="margin-bottom: 4px;">
  <a href="https://www.credly.com/badges/3c1f4223-347e-4b6a-835e-cfeec7660937/public_url">
    <img src="https://img.shields.io/badge/AWS-Certified%20Cloud%20Practitioner-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" />
  </a>
</div>
<div style="margin-bottom: 4px;">
  <a href="https://www.credly.com/badges/f1c7621f-4993-4a0a-bb7f-12f560f9f705/public_url">
    <img src="https://img.shields.io/badge/Google%20Cloud-Cloud%20Engineer-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  </a>
</div>
<div style="margin-bottom: 4px;">
  <a href="https://credentials.databricks.com/68d24fc6-e5dd-4b55-9c31-be438a42d0c3">
    <img src="https://img.shields.io/badge/Databricks-Data%20Engineer%20Professional-FF3621?style=flat-square&logo=databricks&logoColor=white" />
  </a>
</div>
<div>
  <a href="https://credentials.databricks.com/8038de4d-8068-4da1-98a5-826a1c276056#acc.IVRYhcs7">
    <img src="https://img.shields.io/badge/Databricks-Data%20Engineer%20Associate-FF3621?style=flat-square&logo=databricks&logoColor=white" />
  </a>
</div>

---

## Writing

- **[Agentic Airflow: Using AI Agents to Troubleshoot DAG Failures](https://medium.com/@AlejandroMorgante/agentic-airflow-using-ai-agents-to-troubleshoot-dag-failures-37ccfeb4aa25)** — Airflow failure context sent to an AI agent that reads code, proposes fixes, opens draft PRs, and notifies the team.
- **[Multi-Agents with Bedrock and Claude: One Supervisor and Three Specialists](https://medium.com/@AlejandroMorgante/multi-agents-with-bedrock-and-claude-one-supervisor-and-three-specialists-be7483287f92)** — a routed multi-agent architecture using AWS Bedrock and Claude models.
- **[Designing a Modern Data & AI Platform on AWS: From CDC to AI-Powered Analytics](https://medium.com/@AlejandroMorgante/designing-a-modern-data-ai-platform-on-aws-from-cdc-to-ai-powered-analytics-5d9fb0466bf3)** — an end-to-end AWS data platform design, from ingestion and transformation to observability, RAG, and AI-powered analytics.
- **[POC; Amazon Bedrock + S3 Vector](https://medium.com/@AlejandroMorgante/poc-amazon-bedrock-s3-vector-0dbd72273887)** — a practical Bedrock agent proof of concept grounded on documents through S3 Vectors.

---

## Projects

### Bringing AI agent lifecycle orchestration to Apache Airflow

I am contributing a cross-cloud set of Airflow integrations that turns a Dag into a control plane for managed AI agent runtimes. These operators bring the deployment lifecycle into the workflow itself: create an agent runtime, wait for it without occupying a worker, invoke or query the agent, publish updates, and clean up the infrastructure when the workflow is done.

- **[Amazon Bedrock AgentCore Runtime](https://github.com/apache/airflow/pull/67984)** — create, wait for readiness, invoke, and delete an AgentCore Runtime.
- **[Vertex AI Agent Engine](https://github.com/apache/airflow/pull/68479)** — create, retrieve, query, update, and delete an Agent Engine, with deferrable query jobs.
- **[Microsoft Foundry Hosted Agents](https://github.com/apache/airflow/pull/68799)** — create and version, wait for activation, invoke through Responses or Invocations, and delete a Hosted agent.

The larger idea is **bring your own agent**: the agent keeps its framework, reasoning loop, models, and tool integrations, while the cloud service operates the managed runtime around it. Airflow does not replace either layer; it orchestrates the agent's operational lifecycle as part of a larger data or AI workflow. Each contribution includes hooks, operators, deferrable triggers, documentation, unit tests, and end-to-end validation against the real cloud service.

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/apache/airflow"><b>apache/airflow</b></a> <sub>contributor</sub><br />
      <sub>Cross-cloud AI agent lifecycle integrations for AWS, Google Cloud, and Azure, plus data engineering operators</sub>
      <p></p>
      <img src="https://img.shields.io/github/stars/apache/airflow?style=flat-square&label=stars&color=f59e0b" />&nbsp;
      <img src="https://img.shields.io/github/forks/apache/airflow?style=flat-square&label=forks&color=60a5fa" />
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/AlejandroMorgante/agentic-airflow-demo"><b>agentic-airflow-demo</b></a><br />
      <sub>Practical examples for integrating AI agents with Airflow — AWS Bedrock AgentCore and GCP Gemini Agent Platform</sub>
      <p></p>
      <img src="https://img.shields.io/github/stars/AlejandroMorgante/agentic-airflow-demo?style=flat-square&label=stars&color=f59e0b" />&nbsp;
      <img src="https://img.shields.io/github/forks/AlejandroMorgante/agentic-airflow-demo?style=flat-square&label=forks&color=60a5fa" />
    </td>
  </tr>
</table>
