# Repository agent instructions

## Shared startup and integration branches (owner instruction, 2026-11-04)

This repository belongs to COINCUBE. Before substantive work, read the owning
workspace's AGENTS.md and required company context, then this repository's
instructions. Load `tirith-tech/agent-ops` from one verified current reviewed
`main` commit, reading committed AGENTS.md, README.md, contracts/task.md,
docs/task-routing.md, workflows/delivery.md, workflows/pr-review-repair.md and
workflows/batched-ci.md. Read its owning company profile when available; never
substitute another company's brain. Use an existing verified checkout or fetch
the committed files from GitHub without switching another worker's checkout.
Record the full policy SHA and startup receipt in the task's existing issue/PR.
A link alone does not prove the policy was read. If unavailable, report that
before dependent work.

Robert adopted integration-branch batching here. Verify the current primary
branch (currently `master`). Honor an assigned PR target; otherwise reuse a
matching integration branch only after checking scope and integrator ownership,
or create `feature/<topic>` from current primary for multi-slice work. Create
component task branches/worktrees from it and target their PRs there. Choose
automatically; ask only for ambiguous targets, scope or conflicting ownership.
Small standalone fixes may use one draft PR to primary. Never retarget unrelated
active PRs. Record base/head SHAs, chosen targets and one integration owner.

Component PRs use local checks and independent exact-head review. Final PRs to
`master`, `redesign` stay draft while assembling the batch; local validation,
finding dispositions and independent exact-head acceptance allow ready, which
starts applicable hosted CI. Hosted checks must pass before the existing merge
gate. Missing, skipped or unscheduled CI is not passed. Preserve all company
merge/deployment authority, protection and specialist-review requirements.
This adoption changes branch routing and CI scheduling only. For this workflow
it supersedes older instructions that require CI before the ready transition.

PRs targeting the long-standing `redesign` branch also run CI. Do not rename it
or assume unrelated work belongs there.
