---
name: resume-evaluation
description: Evidence-based candidate CV/resume evaluation against a target role or job description. Use for resume screening, CV evaluation, candidate assessment, job-fit analysis, hiring recommendations, interview focus, or comparing multiple candidates. Requires a CV/resume plus a target role or JD; LinkedIn is optional.
metadata:
  version: "2.1.0"
  category: recruiting
  tags:
    - recruiting
    - resume-screening
    - candidate-assessment
    - interview
    - hr
license: MIT
---

# Resume Evaluation

## Purpose
Evaluate a candidate CV/resume against a target role or job description and produce a practical, evidence-based hiring recommendation. Optimize for decision quality and interview usefulness rather than CV summarization.

## Inputs

Required:
- Candidate CV/resume
- Target role, role title, or job description

Optional:
- Hiring country or market
- Seniority and team scope
- Industry or business context
- Language requirements
- Compensation range
- Must-have constraints
- LinkedIn profile
- Recruiter or interview notes

Never require LinkedIn when it is not provided.

## Operating Principles

1. **Evidence first.** Separate explicit resume evidence from inference.
2. **Role relevance over keyword count.** Judge actual scope, ownership, outcomes, scale, and context.
3. **Hard Gates first.** A critical missing requirement may outweigh several minor strengths.
4. **Use `Not Evidenced` when proof is missing.** Do not turn missing evidence into a factual absence.
5. **Do not use protected characteristics in hiring judgments.** Ignore age, gender, ethnicity, religion, disability, family status, political affiliation, sexual orientation, and similar protected traits.
6. **Work authorization is logistical, not a competence proxy.** Consider it only when it is explicitly relevant to the hiring process.
7. **Do not invent facts.** Never fabricate employment history, education, language level, team size, achievements, compensation, or reasons for leaving.
8. **Keep output decision-oriented.** Be concise by default; expand only when useful or requested.

## Workflow

### Step 1 — Build the Role Scorecard
Extract 5–10 criteria from the role/JD and classify each as:
- **Hard Gate** — failure may block progression.
- **Core** — materially affects expected performance.
- **Plus** — useful but non-essential.

If only a role title is provided, infer a reasonable scorecard and clearly mark it as inferred.

### Step 2 — Assess Hard Gates
For each Hard Gate, assign:
- **Met**
- **Partial**
- **Not Met**
- **Not Evidenced**

A `Not Evidenced` result means the CV does not establish the point; it does not automatically mean the candidate lacks it.

### Step 3 — Grade Evidence
For every important positive or negative conclusion, label evidence strength:
- **E3 — Strong:** explicit ownership plus scope, quantified result, duration, team size, geography, or concrete outcome.
- **E2 — Moderate:** relevant responsibility is stated but scope or outcome is limited.
- **E1 — Weak:** keyword, skill claim, or vague self-description only.
- **E0 — None:** no relevant evidence.

### Step 4 — Score Fit
Use `references/scoring-rubric.md`.

Default dimensions:
- Relevant experience — 25%
- Functional capability — 20%
- Scope / seniority / ownership — 15%
- Industry or business-context relevance — 10%
- Geography / local-market relevance — 10%
- Language / stakeholder communication — 10%
- Career trajectory / stability / motivation signals — 10%

Adjust weights when the JD clearly requires it. Hard Gates may override the weighted score.

### Step 5 — Identify Strengths and Risks
Strengths must connect directly to role needs.

Separate risks into:
- **Confirmed gap** — explicit evidence shows the requirement is not met.
- **Evidence gap** — the CV does not establish the requirement.
- **Interview verification point** — plausible fit exists but needs proof.

Do not treat normal career moves, career breaks, or non-linear paths as red flags without job-relevant evidence.

### Step 6 — Make the Hiring Recommendation
Use one of four outcomes:
- **Strong Advance** — strong fit; proceed quickly.
- **Advance** — suitable for the next round; some points need verification.
- **Hold** — mixed fit; compare against stronger candidates or verify a material gap first.
- **Reject** — clear mismatch or failed critical Hard Gate.

## Default Output

### 1. Overall Recommendation
- Fit Score: XX/100
- Decision: Strong Advance / Advance / Hold / Reject
- One-sentence rationale

### 2. Hard Gate Check
| Requirement | Result | Evidence |
|---|---|---|
| ... | Met / Partial / Not Met / Not Evidenced | concise evidence |

### 3. Candidate Snapshot
3–5 bullets covering current or most relevant role, relevant experience, geography, functional scope, and standout background.

### 4. Core Experience & Relevance
Review only roles that materially affect the hiring decision. For each:
- Employer / role / dates
- Job relevance
- Evidence level (E3/E2/E1/E0)
- Brief assessment

### 5. Strengths
3–5 evidence-backed strengths.

### 6. Risks / Gaps / Verification Points
Separate into:
- Confirmed gaps
- Not evidenced
- Needs interview verification

### 7. Interview Focus
List the 3–5 areas that most affect the decision.

### 8. Targeted Interview Questions
Provide 6–10 tailored questions. Prefer behavioral and evidence-seeking questions covering scale, ownership, decisions, metrics, conflict, trade-offs, and outcomes.

### 9. Final Hiring View
Give a short closing judgment explaining whether to move forward and what must be validated next.

## Comparison Mode
When multiple CVs are provided for the same role:
- Apply one shared scorecard and weights to all candidates.
- Show a ranked comparison table.
- Explain the top differentiators.
- Do not let resume design or formatting quality influence competence scoring.

## Quick Mode
If the user asks for a short or fast assessment, output only:
- Fit score
- Decision
- Top 3 strengths
- Top 3 risks
- Top 5 interview questions

## Privacy and Fair-Hiring Guardrails
- Do not repeat phone numbers, personal emails, home addresses, identity numbers, tax numbers, or other unnecessary personal data from the CV.
- Do not use protected characteristics as positive or negative hiring signals.
- Do not infer sensitive attributes from names, photos, schools, locations, or affiliations.
- Do not make medical, psychological, personality, or criminal-history inferences from unrelated resume information.
- Evaluate only job-relevant evidence.

## Quality Check
Before answering, verify that:
- Every major conclusion is supported by the CV and/or JD.
- Hard Gates are explicitly addressed.
- `Not Evidenced` is not presented as `Not Met` without justification.
- The final decision is consistent with the evidence and score.
- Interview questions target unresolved hiring risks rather than generic HR questions.
- No unnecessary personal data is reproduced.

## References
- Scoring method: `references/scoring-rubric.md`
- Example assessment: `references/output-example.md`
- Public-use safety notes: `references/fair-hiring-and-privacy.md`
