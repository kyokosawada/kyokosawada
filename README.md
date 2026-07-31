<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:0f766e,100:14b8a6&height=190&section=header&text=Giusippi%20Apa&fontSize=52&fontColor=e6fffb&fontAlignY=36&desc=AI-forward%20engineer%20%C2%B7%20agents,%20retrieval%20and%20the%20systems%20that%20keep%20them%20honest&descSize=15&descAlignY=57" alt="" width="100%" />

<p align="center">
  <a href="https://portfolio-apa.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-portfolio--apa.vercel.app-14B8A6?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="mailto:giusippi.apaii@gmail.com"><img src="https://img.shields.io/badge/Email-giusippi.apaii%40gmail.com-0f766e?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Manila-Philippines-1f2937?style=flat-square&logo=googlemaps&logoColor=14B8A6" alt="Manila, Philippines" />
</p>

<br />

I build software **with** agents, and I build the systems that keep them honest.

Most of my work now sits in one place: getting language models to do real work reliably, and proving it when they don't. Day to day that means production systems where a model is one component among validators, retries, review queues and reconciliation - not the whole answer. The interesting engineering is almost never the prompt. It is what happens when the output is wrong, stale, or unavailable, and how anyone finds out.

<br />

<table>
<tr>
<td width="50%" valign="top">

### Agents, supervised

Claude Code has been my daily driver since **January 2026** - not a demo, it is how the work gets written, reviewed and shipped.

Isolated worktrees, one task per agent, an explicit review pass, and a human gate before anything lands.

</td>
<td width="50%" valign="top">

### Grounded, or silent

If a system cannot cite the source it answered from, it should decline.

I build the decline path first. An assistant that answers everything is indistinguishable from one that answers nothing correctly - and that failure is silent, which makes it the expensive kind.

</td>
</tr>
</table>

<br />

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0d1117,50:0f766e,100:14b8a6&height=3&section=header" alt="" width="100%" />

## Selected work

<table>
<tr>
<td width="50%" valign="top">

#### [firstmate](https://github.com/kyokosawada/firstmate)
<img src="https://img.shields.io/badge/Shell-89e051?style=flat-square&logo=gnubash&logoColor=black" alt="Shell" />

An agent fleet you talk to through one interface. Spawns coding agents into isolated worktrees, supervises them, and refuses to tear down work that has not landed.

The whole design question is *what an agent is not allowed to do*: it cannot merge without a human word, cannot discard uncommitted work, and cannot report a task complete without evidence.

</td>
<td width="50%" valign="top">

#### [rag-coach](https://github.com/kyokosawada/rag-coach)
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />

Retrieval-grounded assistant that **refuses questions outside its corpus** rather than guessing at them.

The refusal is the feature. Most of the work went into the boundary - deciding when the retrieved context genuinely supports an answer and when it only looks like it does.

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### [orban-labs-challenge](https://github.com/kyokosawada/orban-labs-challenge)
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />

Two services built to a brief in a fixed window: a notes API with search, and a URL shortener with expiry, click analytics and destination validation.

Test-first, incremental commits, with the AI usage disclosed in the repo rather than hidden.

</td>
<td width="50%" valign="top">

#### [gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant)
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />

A chat-driven agent that reasons over a request and then *acts* - reading and sending against Gmail and Calendar, from Slack.

Socket Mode, so it holds a live connection rather than polling for work.

</td>
</tr>
</table>

<br />

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0d1117,50:0f766e,100:14b8a6&height=3&section=header" alt="" width="100%" />

## Stack

**Working in**

<p>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase" />
</p>

**Models and tooling**

<p>
<img src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude" />
<img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini" />
<img src="https://img.shields.io/badge/Retrieval%20pipelines-0f766e?style=flat-square" alt="Retrieval pipelines" />
<img src="https://img.shields.io/badge/Scheduled%20workers-0f766e?style=flat-square" alt="Scheduled workers" />
<img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" alt="Vercel" />
</p>

**Also shipped**

<p>
<img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" />
<img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go" />
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular" />
</p>

<br />

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kyokosawada&show_icons=true&hide_border=true&count_private=true&bg_color=0d1117&title_color=14B8A6&text_color=8b949e&icon_color=14B8A6&hide=issues" alt="" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kyokosawada&layout=compact&hide_border=true&langs_count=6&bg_color=0d1117&title_color=14B8A6&text_color=8b949e" alt="" height="150" />
</div>

<br />

<p align="center">
  <sub>BS Computer Science, De La Salle University · Currently building lead-management and local-SEO automation</sub>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:14b8a6,50:0f766e,100:0d1117&height=110&section=footer" alt="" width="100%" />
