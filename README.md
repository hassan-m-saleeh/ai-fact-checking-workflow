# AI Fact-Checking Workflow

A structured workflow for recording claims, evidence, sources, verdicts, and uncertainty. Includes a CSV ledger and a validator.

## Quick start
Python 3.10+; no third-party packages.
```bash
python src/validate_claims.py data/claims.csv
python -m unittest discover -s tests -v
```

## Verdict definitions
- `supported`: evidence directly supports the claim as written.
- `contradicted`: reliable evidence directly conflicts with it.
- `mixed`: evidence supports only part of it or credible evidence conflicts.
- `insufficient_evidence`: available evidence does not justify a conclusion.

The included rows are templates and intentionally marked `insufficient_evidence`. They are not completed fact-checks. Replace them only after inspecting sources directly.
