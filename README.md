# Resume Evaluation — Evidence-Based Hiring Decision Skill

A practical **resume screening / CV evaluation / candidate assessment** Agent Skill for recruiters, HR professionals, and hiring managers.

Evaluate a candidate **CV or resume against a target job description** and get a structured, evidence-based recommendation: **Strong Advance / Advance / Hold / Reject**.

> Built for the employer side of hiring — not resume rewriting.

## What it does

- Builds a role scorecard from a JD or role title
- Checks **Hard Gates / must-have requirements** first
- Separates explicit resume evidence from inference
- Scores overall **job fit / candidate-role match**
- Identifies strengths, confirmed gaps, evidence gaps, and verification points
- Grades evidence quality instead of relying on keywords alone
- Generates targeted behavioral interview questions
- Produces a clear **Strong Advance / Advance / Hold / Reject** recommendation
- Supports side-by-side ranking of multiple candidates

## Best for

- Resume screening
- CV evaluation
- Candidate assessment
- Job-fit analysis
- Recruiter shortlisting
- Hiring-manager review
- Interview preparation
- Candidate comparison
- HR / Talent Acquisition workflows

## Why this skill is different

Many resume tools focus on rewriting a candidate's resume or matching keywords. This skill is designed for **recruiters and hiring managers making a selection decision**.

It focuses on three things:

1. **Hard Gates** — does the candidate meet the truly critical requirements?
2. **Evidence Level** — is the claimed experience actually supported by scope, ownership, duration, metrics, geography, or outcomes?
3. **Hiring Decision** — what should the recruiter do next, and what must be verified in interview?

## Minimum input

1. Candidate CV / resume
2. Target role or job description

Optional context can include hiring country, seniority, industry, language requirements, compensation range, must-have constraints, LinkedIn profile, or recruiter notes.

**LinkedIn is optional.**

## Example prompts

```text
Evaluate this CV for a Country HR Manager role. Focus on local HR experience,
employee relations, payroll, recruiting, team leadership, and stakeholder management.
```

```text
Compare these three candidates against the same Operations Manager JD and rank them.
Show Hard Gates, fit score, main risks, and recommended interview focus.
```

```text
Quick resume screening: give me fit score, decision, top 3 strengths,
top 3 risks, and 5 interview questions.
```

## Public use cases

See how the skill behaves in realistic fictional hiring scenarios:

- [Country HR Manager](examples/use-case-country-hr-manager.md) — local HR, employee relations, payroll, compliance, team leadership
- [Operations Manager](examples/use-case-operations-manager.md) — frontline scale, KPIs, labor planning, quality, safety, productivity
- [Country Manager](examples/use-case-country-manager.md) — P&L, growth, multi-function leadership, organization scale, commercial execution

These examples are synthetic and contain no real candidate data.

See `examples/` for additional fictional sample inputs and `references/output-example.md` for an example assessment.

## Output structure

Typical output includes:

- Overall fit score
- Hiring recommendation
- Hard Gate check
- Candidate snapshot
- Core experience relevance
- Evidence-backed strengths
- Confirmed gaps vs. not-evidenced items
- Interview verification points
- Targeted interview questions
- Final hiring view

## Install from GitHub

```bash
npx skills add https://github.com/shileidzr-gif/resume-evaluation-skill --skill resume-evaluation
```

Review third-party installation commands before running them in your environment.

## SkillsMP discovery

This repository is designed to be indexed by public Agent Skill marketplaces such as SkillsMP.

Recommended repository topics:

`claude-skills` · `claude-code-skill` · `agent-skills` · `resume-screening` · `candidate-assessment` · `recruiting` · `human-resources`

## Responsible hiring and privacy

This skill is **decision support**, not autonomous hiring authority.

- Do not use protected characteristics as positive or negative hiring signals
- Do not infer sensitive traits from names, photos, schools, locations, or affiliations
- Avoid reproducing unnecessary personal data from resumes
- Treat `Not Evidenced` differently from `Not Met`
- Keep a qualified human reviewer accountable for material hiring decisions
- Follow applicable employment, anti-discrimination, privacy, and AI-governance requirements

See `references/fair-hiring-and-privacy.md`.

## Skill files

```text
resume-evaluation-skill/
├── SKILL.md
├── README.md
├── LICENSE
├── CHANGELOG.md
├── references/
│   ├── scoring-rubric.md
│   ├── output-example.md
│   └── fair-hiring-and-privacy.md
└── examples/
    ├── sample-jd.md
    ├── sample-candidate.md
    ├── use-case-country-hr-manager.md
    ├── use-case-operations-manager.md
    └── use-case-country-manager.md
```

## License

MIT License. See `LICENSE`.

## Version

**2.2.0 — Growth Edition**

### Search keywords

resume evaluation, CV evaluation, resume screening, candidate screening, candidate assessment, job fit analysis, hiring decision, recruiter assistant, talent acquisition, HR recruitment, interview questions, candidate ranking, evidence-based hiring
