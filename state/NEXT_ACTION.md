# NEXT ACTION (ONLY) — GATE 2
Objective: Prove "Signed CI Artifact + Provenance" for the LOCKPACK evidence pack (no app feature work).

Allowed changes (Scope Freeze):
- MODIFY ONLY: .github/workflows/lockpack.yml
- No new files, no deletes, no refactors.
- Keep required status check name stable: "lockpack"

Steps:
1) Update workflow permissions to support OIDC + attestations (id-token + attestations).
2) After building the evidence artifact (.zip), generate build provenance attestation for that artifact.
3) CI must upload: QG.json + snapshot/manifest + resume_pack.zip + (attestation/provenance evidence).
4) Re-run CI on PR and on main; capture evidence (screenshots + downloaded artifact bundle).

Exit criteria:
- Required check "lockpack" PASS
- Evidence pack present
- Provenance/attestation generated for the artifact
- Zero YAML errors, zero pending CI steps
