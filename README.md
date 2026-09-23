# Resume Automator

Evidence-first resume tailoring for people who want stronger applications without inventing credentials.

[Live app](https://resume-automator-frontend.vercel.app/) · [Backend API](https://github.com/adity982/ResumeAutomator-Backend) · [Roadmap](https://github.com/adity982/ResumeAutomator-Frontend/blob/main/ROADMAP.md)

## Why this project exists

Most resume tools optimize for keyword stuffing, black-box scoring, or disposable one-off drafts. Resume Automator takes the opposite position:

- analyze the evidence already present in a resume
- show why a recommendation exists
- keep AI-generated edits reviewable
- avoid fabricated ATS dimensions or unsupported claims
- connect tailoring work to the rest of the application workflow

## What it does

- **Evidence workbench** for resume upload, job description input, analysis, and fact-locked tailoring
- **Career evidence vault** for reusable verified achievements, stories, and skill evidence
- **Job library** with normalized saved targets
- **Application board** with stage tracking, reminders, and package readiness
- **Interview coach** with saved sessions, prep briefs, and answer feedback
- **Outreach studio** with role-specific outreach variants
- **Discovery panel** for preference-based role suggestions
- **Analytics dashboard** for stage conversion and analysis history

## Product principles

- **Evidence first:** every recommendation maps back to resume or job-description text
- **Privacy by default:** uploaded PDFs are parsed in memory and not retained
- **Human approval required:** generated edits stay drafts until accepted
- **Reproducibility over hype:** the UI shows backend-provided metrics

## Stack

- React 19
- TypeScript
- Vite
- TanStack Query
- Firebase authentication
- Recharts

## Local setup

1. Run `npm ci`
2. Copy `.env.example` to `.env.local`
3. Start the backend with `APP_ENV=development` and `AUTH_MODE=development`
4. Run `npm run dev`

## Quality checks

```bash
npm run check
```

This runs linting, type-checking, tests, and a production build.

## Repository map

- `src/components/Workbench.tsx`: upload, analysis, tailoring, exports
- `src/components/EvidenceVault.tsx`: verified evidence management
- `src/components/ApplicationBoard.tsx`: application tracking
- `src/components/InterviewCoach.tsx`: interview practice
- `src/components/AnalyticsDashboard.tsx`: funnel metrics

## Related repository

The FastAPI backend lives in [ResumeAutomator-Backend](https://github.com/adityaguptaaaa/ResumeAutomator-Backend/tree/main).
