# Masaru Ogasawara

Freelance Infrastructure/Cloud Engineer based in Japan, working across AWS, GCP, Databricks,
and Kubernetes — building data platforms and the governance layers around them.
Looking to work outside Japan, alongside engineers I can learn from.

---

## Projects

| Project | Problem | Stack | Differentiator |
|---|---|---|---|
| [dbt-pii-compliance-pipeline](https://github.com/Karasu1t/dbt-pii-compliance-pipeline) | GDPR PII governance drifts out of sync as schemas change | Databricks, dbt, Unity Catalog, Terraform | AI judgment only at dev-time; CI stays fully deterministic |
| [claude-driven-schema-evolution](https://github.com/Karasu1t/claude-driven-schema-evolution) | Schema changes touch many files silently | AWS Glue, Iceberg, Athena, Terraform | Same human-in-the-loop pattern, applied to ETL |
| [internal-log-troubleshooting-with-cortex](https://github.com/Karasu1t/internal-log-troubleshooting-with-cortex) | Cross-cloud IAM trust wiring for incident logs | AWS, Snowflake, Iceberg, Terraform | NL→SQL without exporting raw logs to external LLMs |
| [enterprise-sales-forecast-dashboard](https://github.com/Karasu1t/enterprise-sales-forecast-dashboard) | ML metrics that lie due to data leakage | GCP, Vertex AI, BigQuery, Terraform | Leakage-aware time-series validation, honest metrics |
| [azure-realtime-lakehouse](https://github.com/Karasu1t/azure-realtime-lakehouse) *(in progress)* | Batch inventory checks detect stockouts a day late | Azure Event Hubs, Flink on AKS, Iceberg, ADLS2, Apache Polaris | Stateful (not windowed) detection; checkpoint-synced exactly-once into a vendor-neutral catalog |

---

## How I use AI in engineering

AI judgment belongs at development time, reviewed by a human — never running unattended in CI.
Two of these projects (schema-evolution, pii-compliance) share the same pattern: an interactive
Claude Code command proposes changes step by step with explicit confirmation, while CI/CD stays
100% deterministic — no LLM calls, no API key, anywhere in the pipeline.

---

## How I think about engineering

- What drives my effort isn't a revenue number — it's leveling up. Revenue matters (it's
  literally why I keep getting picked), but it's the result of doing good work, not the reason
  I do it. Give me something that grows my skills and I'll absorb it without being asked.
- I have opinions about the "ideal" architecture, but I'll pick the realistic one. I like new
  tech, but operability wins most arguments.
- I trust what I've actually run and broken over what a blog post says should work.
- I write code heavily, and I want to be in the room from requirements and spec — not just
  execution. Coming up with "this could be better" ideas comes naturally, but it's on top of
  building, not instead of it.
- On a team, I tend to own my own area rather than pair — but I make a habit of feeding
  teammates information they wouldn't otherwise run into: how other companies actually
  structure branch strategy or regression prevention, what a Snowflake seminar or AWS Summit
  was actually worth once you get past the marketing, and what a CEO panel on "how we use AI"
  revealed once you got past the slide deck — including the times the honest answer was "not much."
- Whatever I don't know yet, I've consistently figured out on my own.

---

## Certifications
- AWS Certified Solutions Architect – Professional
- AWS Certified Cloud Practitioner
- Google Cloud Certified – Associate Cloud Engineer
- Certified Kubernetes Administrator (CKA)
- Microsoft Certified: Azure Administrator Associate (AZ-104)
- SnowPro Associate

[View badges on Credly →](https://www.credly.com/users/username.4ad73995)

---

## Currently building

Production-style Azure streaming portfolio (Event Hubs + Flink on AKS + ADLS2 + Apache Polaris) —
architecture and design decisions are documented, implementation is in progress.

Based in Japan.
