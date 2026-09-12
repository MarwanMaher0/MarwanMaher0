# Marwan Maher

**Digital Transformation · IP & Trademarks · Riyadh, Saudi Arabia**

I lead digital transformation for an intellectual-property practice — turning trademark filing,
watching and enforcement from spreadsheet-and-inbox work into systems that run on their own and
tell people what needs doing.

Most of what I ship is internal, so this profile is the part that generalises: how I think about
building software for a domain where being wrong has legal consequences.

---

## What I work on

**Trademark watch, at registry scale.**
Monitoring national registries and official gazettes for marks that conflict with a client's
portfolio, across multiple countries and two scripts. The hard part is not fetching the data — it
is deciding which of hundreds of thousands of new marks actually threaten yours, and being able to
defend that judgement to a lawyer.

**Matching that survives Arabic and English in the same pipeline.**
A staged funnel rather than one clever score: filter by Nice classification, retrieve nearest
neighbours by vector similarity, rank on a composite of phonetic, visual and semantic distance,
then put the survivors in front of a language model for a reasoned verdict. Each stage exists
because the stage before it produced a specific kind of false positive.

**AI where it is accountable, not decorative.**
Model output that drives a legal recommendation gets judged against real historical cases before
anyone trusts it. I care far more about the false-positive rate an operator actually sees than
about a benchmark number.

**The platform underneath.**
Django and Vue, bilingual Arabic/English with genuine RTL rather than a mirrored afterthought,
role-scoped operations tooling, and a cloud migration done without an outage. Unglamorous work
that decides whether any of the above reaches a user.

**Deciding what not to build.**
I spend as much time cutting scope as adding it. Most operational pain turns out to be a workflow
problem wearing a feature request as a disguise.

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
macOS, no network calls, 109 tests that consume no API quota.

The interesting part was the constraint: an account is bound at process start, so nothing can
switch one mid-session. Everything else follows from accepting that.

---

## Tools

`Python` · `Django` · `Vue` · `PostgreSQL` · `Playwright` · `Docker` · `OCI` / `AWS` ·
`vector search` · `LLM pipelines` · `Arabic/English RTL`

---

📫 **marwanmaher635@gmail.com** · 💼 **[LinkedIn](https://www.linkedin.com/in/marwan-maher-b11628227/)**
