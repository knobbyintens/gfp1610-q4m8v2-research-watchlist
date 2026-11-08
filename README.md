# Third-Party Implementation Watchlist

This repository records the best third-party implementation for papers in our
reading queue that have no official code release.

## Entry format

Create one entry per paper at `entries/<preprint-id>.json`:

```json
{
  "paper_id": "2601.01234",
  "paper_title": "Sparse-Gated Recurrent Kernels for Long-Horizon Sequence Modeling",
  "chosen_url": "https://github.com/<owner>/<repo>",
  "repo_full_name": "<owner>/<repo>",
  "verified": true,
  "verification_note": "README cites the exact paper title and preprint identifier"
}
```

## Selection policy

* Only genuine implementations of the paper qualify. A repository qualifies
  only when its README explicitly cites the paper's exact title and preprint
  identifier and the repository actually contains implementation code.
* Implementations of later or different works, general-purpose libraries that
  merely share the paper's keywords, official implementations of unrelated
  papers, and notes-only repositories do not qualify, no matter how popular
  they are in the index.
* Among qualifying repositories, pick the one with the strongest community
  traction, i.e. the highest `adoption_score` in the latest snapshot under
  `metrics/`.
