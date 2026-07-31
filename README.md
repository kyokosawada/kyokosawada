<div align="center">

# Giusippi Apa

**AI-forward engineer** · Manila, Philippines

Retrieval, agent workflows, and the reliability work that makes them trustworthy

<a href="https://portfolio-apa.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-14B8A6?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
<a href="mailto:giusippi.apaii@gmail.com"><img src="https://img.shields.io/badge/Email-0f766e?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

---

Rather than list everything I have touched, here is one system in the detail an interview would actually go into.

## A content pipeline that fails safely

**The problem.** Weekly posts had to go out for a fleet of client sites. A model can write them. A model cannot be trusted to write them *unattended*, because the failure is silent - nobody notices a wrong opening hours line or an invented service until a customer does.

**What it does now, in order:**

1. **Generate** the draft.
2. **Validate** it against rules that can actually be checked - the claims, the formatting, the things that have a right answer.
3. **Retry on rejection, carrying the reason.** The next attempt is told exactly why the last one failed rather than rolling the dice again.
4. **Hold, don't publish.** Anything still failing is parked as `needs_review` for a person. It never goes out on a hope.
5. **Reconcile daily** against what the platform actually recorded, so the system's belief about what published is checked against reality rather than assumed.

**What it proves.** The model is one component. Everything interesting is the scaffolding around it: what counts as wrong, what happens next, who finds out, and how you know afterwards that it worked.

**What I would change.** The validators encode what we knew to check for at the time. There is no measurement of what they *miss* - the false-negative rate is unknown, and I would want an error budget and a sampled human review before trusting it further.

---

## The rest, briefly

| | |
|:--|:--|
| **UpRank** · *current, private* | Local-SEO and lead-management platform. ~30 scheduled jobs in production across operations, marketing and reporting. The pipeline above lives here. |
| **[rag-coach](https://github.com/kyokosawada/rag-coach)** | Retrieval-grounded assistant that **refuses** questions outside its corpus rather than guessing. The refusal is the feature. |
| **[gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant)** | An agent that reasons over a request and then *acts* - Gmail and Calendar, from Slack, over a live connection. |
| **[lead-approval-bot](https://github.com/kyokosawada/lead-approval-bot)** | Inbound lead becomes an Approve / Deny card in Slack; the decision sends the reply email. One tap, because the decider is on their phone. |

---

<div align="center">

**Working in** TypeScript · Python · Next.js · FastAPI · Postgres / Supabase
**Models and tooling** Claude · Gemini · retrieval pipelines · scheduled workers
**Also shipped** Java / Spring Boot · Kotlin · Go · Angular

<br />

<sub>Claude Code as a daily driver since January 2026 · BS Computer Science, De La Salle University</sub>

</div>
