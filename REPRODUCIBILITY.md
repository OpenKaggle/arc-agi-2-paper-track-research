# Reproducibility guide

## What this snapshot can reproduce

This public snapshot supports inspection and code-level replay of the original
ARC-AGI-2/Paper Track orchestration, validators, negative controls, paper
protocols, and lightweight evaluation records. It is a research snapshot, not
a final-ready submission package.

The archive does not contain competition files, generated submissions, model
weights/checkpoints, compiled caches, or the original virtual environments.
Any neural or competition-data run therefore requires separately acquired,
properly licensed inputs and exact environment reconstruction.

The six historical conservative-agreement V1, stable-V2, and exact-overlay-V3
development/holdout notebooks are also excluded: they were generated from a
third-party public notebook whose redistribution license is not frozen here.
Their contributor-authored builder, private candidate metadata, factual
upstream metadata, preregistrations, and hash-bound receipts remain for audit.
Regenerating a candidate requires separately acquiring that upstream notebook
under its own terms. Historical manifests may name and hash an excluded payload;
that evidence binding is not a redistribution of the payload itself.

## Entry points

- `README.md` records the historical execution state and research gates.
- `paper/06_reproducibility_checklist.md` defines the paper evidence contract.
- `run_exact_rule_heldout_audit.py` is the exact-rule negative-control entry.
- `run_neurogolf_dsl_baseline.py` is the NeuroGolf DSL negative-control entry.
- `validate_candidate_notebook.py` and `validate_submission.py` provide static
  and schema checks.

The retained tests are part of the research record, not a hermetic CI bundle.
Full discovery in this slim public snapshot is expected to report unavailable
optional dependencies (for example `jsonschema`) and missing bindings to
excluded run receipts, competition inputs, public-asset mirrors, or sibling
research modules. Reacquire those artifacts under their original terms before
attempting the complete historical suite.

For a dependency-light syntax and machine-readable-record check from the
repository root, run:

```bash
python3 -c 'import ast, pathlib; [ast.parse(p.read_text(encoding="utf-8")) for p in pathlib.Path(".").rglob("*.py") if ".git" not in p.parts]'
find . -path ./.git -prune -o -name '*.json' -type f -exec python3 -m json.tool {} \; >/dev/null
```

These checks do not recreate excluded datasets, models, Kaggle runs, or a
competition score. When running individual historical tests, read their input
contracts first and treat missing external artifacts as an unmet prerequisite,
not as evidence that the archived claim passed or failed.

## Evidence boundary

Treat hashes and receipts as bindings to the historical artifacts they name.
Do not infer final readiness, hidden-set performance, or generalization from a
passing source/test check. Review `NOTICE.md` before acquiring third-party
notebooks, official code, or model assets.
