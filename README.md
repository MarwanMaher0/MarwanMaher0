# Marwan Maher

**Technical PM & Engineer · IP & Legal-tech · Egypt (working with a Riyadh IP-services firm) · Open to remote & relocation (KSA/UAE)**

I am the Project Manager for IT projects at an IP-services firm in Riyadh — turning trademark
filing, watching and enforcement from spreadsheet-and-inbox work into systems that run on their
own and tell people what needs doing.

The products themselves are my employer's and stay internal, so this profile is the part that
generalises: how I think about building software for a domain where being wrong has legal
consequences.

---

## What I work on

**Owning a portfolio, not a ticket queue.**
Five production systems, from requirements and procurement through release and maintenance. That
includes writing the requirements a vendor is judged against, running the evaluation, and being
the one accountable when the decision is to build instead of buy.

**AI where it is accountable, not decorative.**
Model output that drives a legal recommendation gets validated against real historical outcomes
before anyone trusts it. I care far more about the false-positive rate an operator actually sees
than about a benchmark number.

**The platform underneath.**
Django and Vue, bilingual Arabic/English with genuine RTL rather than a mirrored afterthought,
role-scoped operations tooling, and a cloud migration done without an outage. Unglamorous work
that decides whether any of the above reaches a user.

**Deciding what not to build.**
I spend as much time cutting scope as adding it. Most operational pain turns out to be a workflow
problem wearing a feature request as a disguise. One finished reporting build was rejected because
it missed what the business actually needed; re-scoping it was the right call, not a setback.

---

## Selected work

- **IP management platform** — sole architect and builder, from an empty repo to production; now
  the daily system of record for operations. Django + Vue, bilingual Arabic/English with genuine
  RTL, role-scoped access.
- **Trademark monitoring** — as PM: wrote the requirements, ran a four-vendor evaluation, then led
  the in-house build. In production.
- **[Cepro.ai](https://cepro.ai)** — Next.js 15 + React 19 rebuild with in-browser Arabic OCR
  (Tesseract.js), delivered two weeks early. Live at https://cepro.ai.

Internal products are described at the level of my role only; implementation details belong to my
employer.

Portfolio & CV: https://marwanmaher.vercel.app

---

## How I work

- **Look at the real data before writing the parser.** Formats you assume are formats you get
  wrong. More than once a field I "knew" the shape of turned out to have two shapes, and the
  difference mattered.
- **Test in the real thing.** Scripted probes report success on broken paths. If it is a user
  interface, it is not done until it has been driven in a browser.
- **Make the failure mode expensive to reintroduce.** A bug that caused real damage earns a test,
  a comment explaining *why*, and a line in the README — not just a fix.
- **Say plainly what broke.** Post-mortems that hedge teach nobody anything.

---

## Open source

**[claude-account-switcher](https://github.com/MarwanMaher0/claude-account-switcher)** — run
several Claude Code accounts and fail over when one hits its rate limit, carrying the conversation
across. Built because I kept stalling on one subscription while a second sat idle. MIT, Linux and
macOS, no network calls, 218 assertions that consume no API quota.

The interesting part was the constraint: an account is bound at process start, so nothing can
switch one mid-session. Everything else follows from accepting that.

**[vue-intent](https://github.com/MarwanMaher0/vue-intent)** — Vue 3 adapter for intent-first,
state-driven UIs: permission guards, navigation protection, a composable API. TypeScript.

---

## Tools

`Python` · `Django` · `Vue` · `PostgreSQL` · `Playwright` · `Docker` · `OCI` / `AWS` ·
`LLM pipelines` · `Arabic/English RTL`

---

📫 **marwanmaher635@gmail.com** · 💼 **[LinkedIn](https://www.linkedin.com/in/marwan-maher-b11628227/)**
