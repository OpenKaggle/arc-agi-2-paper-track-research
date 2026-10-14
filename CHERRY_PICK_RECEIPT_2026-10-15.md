# Cherry-pick publication receipt — 2026-10-15

Project: `arc2_paper` → repository `OpenKaggle/arc-agi-2-paper-track-research`.
This commit publishes files that were present in the local workspace,
listed in the 853-row first-party source manifest, and missing from the
remote repository at the time of the dry-run comparison. Every file was
re-verified before commit: SHA-256 and byte count match the manifest entry
exactly (see `state` column).

## Files added

- `candidate_notebooks/public_qwen_lb3181_anchor_v1/kernel-metadata.json` (748 bytes)
  - sha256 `c09d0506038dbd9a323a8ca92b8b100314b8d9ca1a76bd6c538204b163b31c88`  - class `source-or-derived-text-candidate`
- `paper/results/ablation_table.csv` (3778 bytes)
  - sha256 `fa5b9388fe0533e5795cada9cfeafaa828b297a13dd0dac59d7327ffd54c9952`  - class `source-or-derived-text-candidate`
- `paper/results/dataset_revision_tasks_2026-09-09.csv` (41857 bytes)
  - sha256 `8e0818abc34aa3d745e819133276cb903b71231651254e63bdfdeeb42e5fd01d`  - class `source-or-derived-text-candidate`
- `paper/results/failure_log.csv` (247 bytes)
  - sha256 `2e8f3a32cfb5ff764bd834d958c2723584ebd74077ad40a3f3971fd5fdb3f082`  - class `source-or-derived-text-candidate`
- `paper/results/family_results_template.csv` (49 bytes)
  - sha256 `3cece28567d55b0791e94b5f98e4cbf721022f8a02d58a6b2eb4c538f0cbdda1`  - class `source-or-derived-text-candidate`
- `paper/results/paired_results_template.csv` (141 bytes)
  - sha256 `ab1dc2bf23cb1bea78337ad5db83f60fc1468896e4765046bd1301839799bbb6`  - class `source-or-derived-text-candidate`
- `paper/results/technical_artifact_watch.csv` (15216 bytes)
  - sha256 `7f088b82f472fd798a5c6a23e830fe8ab764e294b2e53d1a47b5aaaa7b26ba0f`  - class `source-or-derived-text-candidate`
- `paper/tests/fixtures/failure_log_valid.csv` (443 bytes)
  - sha256 `02316c01466300a7df45f66fe857bf99d3241c0b1c25f4fdc5d8f1181d829b61`  - class `source-or-derived-text-candidate`
- `paper/tests/fixtures/family_results_small.csv` (281 bytes)
  - sha256 `691f9a4fc26784ca5f9e98c103c1e366014cdbfe9c6fcc3ececbfbf721c86673`  - class `source-or-derived-text-candidate`
- `paper/tests/fixtures/paired_results_small.csv` (225 bytes)
  - sha256 `8ffd5dc157dad80972f780d0bdf1192470d6cd9c02e15432e2a08ca747a48de1`  - class `source-or-derived-text-candidate`

## Review notes

- First-party paper results/templates/fixtures and one public kernel metadata
  record. No credentials, identity fields, or absolute local paths found.
  Fixture CSVs contain placeholder task ids only.
- `technical_artifact_watch.csv` references files by repo-relative paths.
- Not covered here: `paper/evaluator_only/**` (official evaluator payloads)
  remain unpublished per the source-boundary policy.

## Source of truth

- Local workspace: `~/Desktop/kagglepred/arc2_paper/`
- Source manifest: `outputs/kagglepred-release-audit-2026-09-28/first-party-source-manifest.csv` (project rows for `arc2_paper`).
