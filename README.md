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

Three small tools that teach one project from start to finish — decide, ship, learn:

**[decision-matrix](https://github.com/MarwanMaher0/decision-matrix)** — a guided decision matrix for
build-versus-buy and tool choices ([try it](https://marwanmaher0.github.io/decision-matrix/)). It keeps
must-haves apart from weighted criteria, shows how far a weight has to move before a different option
wins, and writes a decision record you can commit. Runs entirely in the browser. Vue 3, 63 tests.

**[phasegate](https://github.com/MarwanMaher0/phasegate)** — a CLI and GitHub Action that walks a project
from discover to operate. It writes short guided documents for each phase and fails CI when a phase the
team has moved past is not actually done: requirements without acceptance criteria, decisions still
"proposed", a release checklist with no rollback plan. It checks its own repository. TypeScript, 86 tests.

**[django-postmortem](https://github.com/MarwanMaher0/django-postmortem)** — blameless incident reviews
for Django. It flags blame-shaped phrasing, and every action item has to name the guard that stops the
failure coming back: a regression test, a constraint, an alert. A review cannot close until each fix is
verified. 133 tests.

**[vue-rtl-kit](https://github.com/MarwanMaher0/vue-rtl-kit)** — a Vue 3 and Nuxt toolkit for
right-to-left that actually holds up. The piece I care about is bidirectional text: in an Arabic
sentence, a date, a phone number, an order reference or a version string silently reverses, and
users report it as "the number is wrong" rather than as a rendering bug. The kit isolates those
runs, plus direction state that survives SSR, logical-property utilities, and locale-aware
formatting across numbering systems. MIT, 106 tests, CI on Node 20 and 22.

**[django-rtl-admin](https://github.com/MarwanMaher0/django-rtl-admin)** — the same problem on the
server side. The Django admin in an RTL locale is mirrored, not translated: the add-button icon
sits on the wrong edge, object tools float the wrong way, the sidebar chevron never swaps, and
table cells reverse identifiers. This fixes the styling with logical properties, isolates cell
contents, formats numbers and dates for the active locale's numbering system, and adds a language
switcher. MIT, 192 tests, CI across Django 4.2 to 6.1 on Python 3.10 to 3.13.

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
