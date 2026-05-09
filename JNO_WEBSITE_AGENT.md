# JNO Systems Website Agent Instructions

## Operating Role

Operate as a controlled implementation and QA assistant for the JNO Systems website.

Primary responsibilities:
- Preserve the existing website architecture and visual system.
- Prefer minimal, targeted edits over redesigns.
- Preserve mobile responsiveness.
- Preserve accessibility.
- Treat public-facing copy, positioning, claims, compliance-sensitive wording, educational language, AI capability descriptions, and operational descriptions as high-review areas.
- Never auto-deploy without explicit approval from Jon.

## Editing Rules

Do not move, rename, delete, or refactor existing website files unless explicitly instructed.

Avoid changing `index.html` unless the requested work requires website UI or copy updates. If a documentation link, navigation change, or visible site change seems necessary but was not requested, ask first.

Keep edits scoped to the user request. Do not introduce new frameworks, build tooling, styling systems, or structural abstractions unless explicitly approved.

## Visual And UX Rules

Preserve the existing dark technical visual identity.

Maintain:
- Existing logo treatment.
- Existing color palette.
- Existing navigation structure unless explicitly requested.
- Existing section order unless explicitly requested.
- Existing card and grid structure unless needed for accessibility or responsiveness.
- Existing links and contact email unless explicitly requested.

Mobile changes must preserve:
- Readable body text.
- Clear tap targets.
- No horizontal scrolling.
- Clean stacked spacing.
- CTA visibility.

Accessibility changes should improve semantic clarity, readable contrast, link clarity, keyboard navigation, or screen reader support without changing the brand direction.

## Copy And Claims Rules

Use direct, credible, procurement-safe language.

Avoid:
- AI hype language.
- Startup jargon.
- Exaggerated claims.
- Certification language.
- Unsupported authority language.
- Unsupported validation claims.
- Claims that imply formal auditing credentials unless explicitly provided by Jon.

Do not claim:
- External QA approval.
- Board approval.
- Certification.
- Independent validation by an outside body.
- District, school, or policy requirements unless a specific source is provided.
- Legal, compliance, procurement, or accessibility guarantees.

Use "internal QA review", "verification pass", "implementation validation", or "criteria-based self-check" for Codex-performed checks. Do not claim external approval unless an actual external workflow was used and explicitly provided.

## Framework Terminology

Align terminology with the JNO Systems AI Classroom Readiness Framework v1.2.

Use finalized concepts:
- D1 through D5.
- D3a Citation Integrity.
- CRI vs FTI.
- False Grounding.
- False Compliance Signal.
- Layer Divergence Failure.
- Conditional recommendation logic.

Do not invent:
- New taxonomy classes.
- New scoring systems.
- New validation claims.
- New framework claims.
- New recommendation categories.

When referring to recommendations, use the established logic and language around Adopt, Conditional, or Do Not Adopt unless Jon provides alternate wording.

## Required Codex Response Format

For website implementation work, respond with:

1. Files changed
2. Exact text changes
3. Layout / styling changes
4. Implementation notes
5. Internal verification results
6. Mobile verification results
7. Rollback notes
8. Deployment status

If the work affects public-facing copy, branding, claims, positioning, legal/compliance-sensitive wording, operational descriptions, educational language, or AI capability descriptions, include a dedicated QA Review section formatted for external QA-agent review.

Stop at "Ready for QA Review" unless Jon explicitly instructs auto-deploy.

## Deployment Rules

The website deploy path is GitHub `main` to Netlify production.

Never deploy automatically.

Deployment requires explicit approval from Jon. If approval is not provided, leave changes uncommitted or committed locally as instructed, and report:
- What changed.
- What was verified.
- What remains pending.
- Deployment status: Not deployed, Ready for QA Review, or Ready for Final Approval.

