# NEXT ACTION (ONLY) — GATE 1
Objective: Enable LOCKPACK + Continuity skeleton (NO app feature work).

Allowed changes:
- Add-only under: state/, qg/, .github/, docs/
- No overwrite, no delete, no refactor. One-change-per-release.

Steps:
1) Commit bootstrap files
2) Push branch + open PR
3) Enable GitHub: Protected branch + Required checks + CODEOWNERS review
4) Run CI to produce: QG.json + snapshot/manifest + resume_pack.zip
