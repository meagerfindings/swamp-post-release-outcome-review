# Post-Release Outcome Review

A standalone Swamp extension that validates and records deterministic,
evidence-bound post-release recommendations. It neither collects data nor
executes recommendations.

The packaged extension is in [`extensions/`](extensions/). It is licensed under
the MIT License; see [LICENSE](LICENSE).

## Verify

```sh
deno fmt --check
deno lint
deno check extensions/models/post_release_outcome_review.ts
deno test
swamp extension fmt extensions/manifest.yaml --check --json
swamp extension quality extensions/manifest.yaml --json
swamp extension push extensions/manifest.yaml --dry-run --json
```
