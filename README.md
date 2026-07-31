<div align="center">

# Giusippi Apa

### The harness is the job now

<img src="https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />

<a href="https://apa-dev.netlify.app/"><img src="https://img.shields.io/badge/Portfolio-apa--dev.netlify.app-14B8A6?style=flat-square&logo=netlify&logoColor=white" alt="Portfolio" /></a>
<a href="mailto:giusippi.apaii@gmail.com"><img src="https://img.shields.io/badge/Email-0f766e?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
<img src="https://img.shields.io/badge/Manila,%20PH-1f2937?style=flat-square&logo=googlemaps&logoColor=14B8A6" alt="Manila, Philippines" />

</div>

---

**Models will keep getting better.** That is the safest assumption in this field - and it is also the one thing you have no control over and gain no advantage from, because everyone gets the same upgrade on the same day.

What does not arrive with the next release is the scaffolding around it: the specification precise enough to act on, the isolation that makes a wrong attempt cheap, the verification that catches a confident wrong answer, and the judgement about what "wrong" even means here.

**A stronger model does not rescue a missing harness. It makes the wrong answers more convincing.**

So I don't type most of the code I ship any more. I specify it, supervise it, and reject it when it's wrong - and that is a different skill from writing it, with its own failure modes.

## What working this way actually takes

**A specification an agent cannot misread.** Vague instructions do not produce vague code - they produce confident, plausible, wrong code, which is far more expensive. Most of my thinking time now goes into the brief, not the implementation.

**Isolation, so a bad run costs nothing.** I run **ten parallel worktrees** on my main project. Each task is quarantined; a wrong turn is deleted rather than untangled. Cheap disposal is what makes ambitious attempts affordable.

**Review that starts from "this is wrong".** The failure mode of generated code is that it looks finished. It compiles, it reads well, the tests pass - and it solved a slightly different problem. Reading it as an adversary is the only thing that catches that.

**Tests as the contract, written first.** Not for orthodoxy. When an agent writes the implementation, the test is the only artifact that encodes what you actually asked for, and the only thing that survives the next rewrite.

## Where the same thinking shows up in what I build

The systems worth building have the same shape as the workflow: **assume the model will be wrong, and design for the moment it is.**

**UpRank** &nbsp;`current work` &nbsp;`private` — local-SEO and lead-management platform, **~2,280 commits over six months**, ~30 scheduled jobs in production. The generated-content pipeline validates before publishing, feeds the rejection reason back into the retry, holds anything still failing for a person instead of shipping it, and reconciles daily against what actually happened.

**[rag-coach](https://github.com/kyokosawada/rag-coach)** — retrieval-grounded assistant that **refuses questions outside its corpus** rather than guessing. The refusal is the feature: an assistant that answers everything is indistinguishable from one that answers nothing correctly, and that failure is silent.

**[gemini-slack-assistant](https://github.com/kyokosawada/gemini-slack-assistant)** — an agent that reasons over a request and then *acts*, against Gmail and Calendar from Slack, over a live connection rather than polling.

**[lead-approval-bot](https://github.com/kyokosawada/lead-approval-bot)** — an inbound lead becomes an Approve / Deny card in Slack; the decision sends the reply email. One tap, because the person deciding is on their phone.

## What I don't think

That this makes engineers unnecessary, or that any of it is close to unattended. Everything above exists because the output cannot be trusted by default. The judgement about *what to build*, *what counts as wrong*, and *what to do when it is* has not moved anywhere - it has just become the whole job.

---

<div align="center">

**Also shipped** &nbsp;
<img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
<img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" />
<img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go" />
<img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular" />

<br />

<sub>Claude Code as a daily driver since January 2026 · BS Computer Science, De La Salle University</sub>

</div>
