<div align="center">
<br />

# Giusippi Apa

### AI-forward engineer

**Retrieval · agent workflows · the reliability work that makes them trustworthy**

<br />

<a href="https://apa-dev.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-14B8A6?style=for-the-badge&logo=netlify&logoColor=white" alt="Portfolio" /></a>
<a href="mailto:giusippi.apaii@gmail.com"><img src="https://img.shields.io/badge/Email-0f766e?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<img src="https://img.shields.io/badge/Manila,%20PH-1f2937?style=for-the-badge&logo=googlemaps&logoColor=14B8A6" alt="Manila, Philippines" />

<br />
<br />

</div>

> Most of my work sits in one place: **getting language models to do real work reliably, and proving it when they don't.**
>
> Production systems where a model is one component among validators, retries, review queues and reconciliation - not the whole answer. The interesting engineering is almost never the prompt. It is what happens when the output is wrong, stale, or unavailable, and how anyone finds out.

<br />

<div align="center">

| | |
|:--|:--|
| **Agents, supervised** | Claude Code as a daily driver since January 2026. Isolated branches, one task at a time, an explicit review pass, and my own read before anything lands. |
| **Grounded, or silent** | If a system cannot cite the source it answered from, it should decline. I build the decline path first. |

</div>

<br />

---

<div align="center">

## Selected work

</div>

<br />

<div align="center">
<table>
<tr>
<td width="440" valign="top">

**UpRank** &nbsp; `current work` &nbsp; `private`

Local-SEO and lead-management platform. **~30 scheduled jobs in production** across operations, marketing and reporting.

The generated-content pipeline is the part worth talking about: validators reject a bad draft, the retry carries the rejection reason into the next attempt, anything still failing is held for a human rather than published, and a daily reconcile records what actually happened instead of what we assumed.

`TypeScript` `Next.js` `Supabase` `Vercel`

</td>
<td width="440" valign="top">

**[rag-coach](https://github.com/kyokosawada/rag-coach)**

Retrieval-grounded assistant that **refuses questions outside its corpus** rather than guessing at them.

The refusal is the feature. Most of the work went into the boundary - deciding when the retrieved context genuinely supports an answer and when it only looks like it does.

`TypeScript` `retrieval` `evaluation`

</td>
</tr>
<tr>
<td width="440" valign="top">

**[gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant)**

A chat-driven agent that reasons over a request and then *acts* - reading and sending against Gmail and Calendar, from Slack.

Socket Mode, so it holds a live connection rather than polling for work.

`TypeScript` `Slack Bolt` `Gemini`

</td>
<td width="440" valign="top">

**[lead-approval-bot](https://github.com/kyokosawada/lead-approval-bot)**

An inbound lead becomes an Approve / Deny card in Slack, and the decision sends the reply email.

Built around a real constraint: the person deciding is on their phone, so it has to be one tap and the audit trail has to survive it.

`TypeScript` `Netlify Functions`

</td>
</tr>
</table>
</div>

<br />

---

<div align="center">

## Stack

<br />

**Working in**

<img src="https://skillicons.dev/icons?i=ts,python,nextjs,fastapi,nodejs,postgres,supabase&theme=dark" alt="TypeScript, Python, Next.js, FastAPI, Node, Postgres, Supabase" />

**Also shipped**

<img src="https://skillicons.dev/icons?i=java,spring,kotlin,go,angular&theme=dark" alt="Java, Spring, Kotlin, Go, Angular" />

<br />
<br />

<sub>BS Computer Science, De La Salle University</sub>

</div>
