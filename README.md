# Resume Evaluation — Agent Skill

An evidence-based recruiting skill for evaluating a candidate CV/resume against a target role or job description.

## What it does

- Builds a role scorecard from a JD or role title.
- Checks critical Hard Gates first.
- Separates explicit evidence from inference.
- Scores overall job fit.
- Identifies strengths, confirmed gaps, evidence gaps, and interview verification points.
- Generates targeted interview questions.
- Produces a clear **Strong Advance / Advance / Hold / Reject** recommendation.
- Supports side-by-side comparison of multiple candidates.

## Why this skill is different

Many resume tools optimize for rewriting resumes or keyword matching. This skill is designed for the **employer / recruiter / hiring-manager side** of the decision and emphasizes evidence, job relevance, and interview follow-up.

## Requirements

Minimum input:
1. Candidate CV/resume
2. Target role or job description

LinkedIn is optional.

## Example prompt

```text
Evaluate this CV for a Country HR Manager role. Focus on local HR experience,
employee relations, payroll, recruiting, team leadership, and stakeholder management.
```

See `examples/` for fictional sample inputs and `references/output-example.md` for an example assessment.

## Install from GitHub

```bash
npx skills add https://github.com/shileidzr-gif/resume-evaluation-skill --skill resume-evaluation
```

Check the installer you use before running third-party commands.

## SkillsMP discovery

SkillsMP indexes public GitHub repositories containing a `SKILL.md` with valid frontmatter. Add repository topics such as `claude-skills` or `claude-code-skill` to improve discovery.

## Responsible use

This skill is decision support, not autonomous hiring authority. Keep a human reviewer accountable for material decisions and follow applicable employment, anti-discrimination, privacy, and AI-governance requirements.

See `references/fair-hiring-and-privacy.md`.

## License

MIT License. See `LICENSE`.

## Version

2.1.0 — Public Edition
