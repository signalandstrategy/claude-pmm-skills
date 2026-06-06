# Claude PMM Skills

A collection of Claude skills built for Product Marketing Managers. Each skill encodes a specific PMM workflow — the research process, the output structure, and the quality standards — so Claude produces briefs and analyses that are immediately useful, not just informative.

---

## What Are Claude Skills?

Claude skills are instruction sets you install into Claude to make it consistently better at specific tasks. Instead of re-explaining your workflow every time, a skill bakes in the process, the output format, and the standards once. Claude then follows them automatically whenever the task matches.

Think of them as reusable playbooks. You write the playbook once; Claude runs it reliably every time.

**How to install a skill:**
1. Open Claude (claude.ai)
2. Go to Settings → Skills
3. Upload the `SKILL.md` file from the skill folder you want

---

## Skills in This Repository

### [PMM Research](./skills/pmm-research/)

**What it does:** Generates a full competitive and GTM research brief for any product or company.

**Trigger:** Give Claude a product name or URL with research intent.

**Output:** An 8-section structured brief covering product positioning, pricing analysis, ICP definition, competitive landscape, GTM motion recommendation, marketing risks, discovery questions, and 30-day quick wins. Every section ends with a PMM action.

**Best for:** New client onboarding, interview prep, consulting engagements, pre-launch competitive research.

---

*More skills coming. See the [Contributing](#contributing) section if you want to add one.*

---

## Repository Structure

```
claude-pmm-skills/
├── README.md                          # This file
└── skills/
    └── pmm-research/
        ├── SKILL.md                   # The skill instruction file (install this)
        ├── README.md                  # How to use this skill
        └── examples/
            ├── retell-ai-brief.md     # Example: Voice AI platform
            ├── leadsquared-brief.md   # Example: CRM, interview prep context
            └── whatfix-brief.md       # Example: DAP platform, name-only input
```

---

## Principles Behind These Skills

Skills in this repository follow a few consistent standards:

**Insight over information.** The output should tell you something you couldn't get by reading the website yourself. If the brief is just a summary of the homepage, it failed.

**Every section ends with an action.** Analysis without a recommendation is noise. Every section ends with a direct PMM action — not a hedge, not a "consider exploring."

**Name what's missing.** If data isn't publicly available, say so and explain what that absence signals. A Research Confidence Note at the end of every brief tells you where to trust the output and where to verify.

**State a view and own it.** No "could potentially" or "may want to consider." A senior PMM makes a call. The skill does the same.

---

## Contributing

If you're a PMM who has built a Claude skill for a specific workflow — competitive battlecards, persona development, launch planning, sales enablement, analyst briefings — contributions are welcome.

**To add a skill:**

1. Fork this repository
2. Create a folder under `skills/` named after your skill (e.g., `skills/battlecard-builder/`)
3. Add a `SKILL.md` with YAML frontmatter (name, description) and the full instruction set
4. Add a `README.md` explaining what the skill does, how to trigger it, and what it outputs
5. Optionally add an `examples/` folder with one or two sample outputs
6. Open a pull request with a short description of what the skill does and why it's useful

**Quality bar:** The skill should encode a real PMM workflow — something you've actually used in client work, job prep, or day-to-day PMM tasks. Generic "help me with marketing" prompts don't qualify as skills.

---

## About

Built by [Rohit Rangnekar](https://www.linkedin.com/in/rohitrangnekar/) — PMM with 10 years in B2B SaaS across Whatfix, Leap, and DoSelect (acquired by Info Edge). Currently doing PMM consulting and advisory work across AI and SaaS companies.

The workflows encoded in these skills come from real engagements: competitive research for voice AI platforms, PMM strategy for CRM and DAP companies, GTM planning for early-stage AI products.

If you use these skills and build something useful, share it. The goal is a PMM skill library that actually reflects how good PMMs work.

---

## License

MIT. Use freely, adapt as needed, share improvements.
