# Skill Registry

Project: Portafolio
Generated: 2026-05-04

## Sources Scanned
- User-level: `~/.config/opencode/skills/*/SKILL.md`
- Project-level: `.claude/skills/`, `.gemini/skills/`, `.agent/skills/`, `skills/` (none found)
- Project conventions: `agents.md`, `AGENTS.md`, `CLAUDE.md`, `.cursorrules`, `GEMINI.md`, `copilot-instructions.md` (none found)

## User Skills (deduplicated)
Excluded from trigger table: `sdd-*`, `_shared`, `skill-registry`.

| Skill | Trigger |
|---|---|
| branch-pr | Creating/opening pull requests or preparing changes for review |
| issue-creation | Creating GitHub issues, reporting bugs, or requesting features |
| go-testing | Writing Go tests, teatest/Bubbletea testing, adding test coverage |
| skill-creator | Creating new AI skills or documenting reusable AI patterns |
| comment-writer | Drafting PR/review/issue/chat comments for humans |
| cognitive-doc-design | Writing docs: guides, READMEs, RFCs, onboarding, architecture docs |
| gentle-ai-chained-pr | Planning/splitting large PRs into chained/stacked review slices |
| work-unit-commits | Structuring commits by deliverable work units |
| judgment-day | User asks for dual/adversarial review ("judgment day", "doble review", etc.) |

## Compact Rules

### branch-pr
- Every PR must link an approved issue.
- Use one and only one `type:*` label.
- Use conventional commits and valid branch naming.

### issue-creation
- Use issue templates, not blank issues.
- New issues start as needs-review.
- PR starts only after maintainer approval.

### go-testing
- Prefer table-driven tests in Go.
- Include deterministic assertions and failure clarity.
- Add coverage when behavior changes.

### skill-creator
- Create skills only for repeated, non-trivial patterns.
- Keep SKILL.md structured and actionable.

### comment-writer
- Be warm, direct, and short.
- Start with actionable feedback and explain why.

### cognitive-doc-design
- Lead with outcome, then details.
- Use chunking, signposting, checklists/tables over dense prose.

### gentle-ai-chained-pr
- Split PRs when review size risk is high (>400 changed lines).
- Ensure each slice is autonomous, verifiable, and rollback-safe.

### work-unit-commits
- Commit by deliverable behavior, not by file type.
- Keep tests/docs with the behavior they verify.

### judgment-day
- Run two blind parallel reviews, then synthesize findings.
- Apply fixes and re-judge up to escalation threshold.
