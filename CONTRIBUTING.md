# Contributing

Normal pull requests add or update one or more files under
`data/vendors/{shard}/`.

- Describe only public vendor, program, and offer facts supported by the URLs
  in the record.
- Keep stable IDs stable. Correct or end an offer instead of deleting its
  history.
- Do not claim Sourcey verification, vendor signatures, freshness, or
  provenance tiers in YAML. Sourcey's independent evidence and authority
  pipeline derives those properties.
- Do not add executable code, schemas, generated output, evidence objects,
  scanner state, package files, or release controls.
- Sign off commits using `Signed-off-by: Name <email>` to certify the
  [Developer Certificate of Origin](https://developercertificate.org/).

CI validates only the changed dependency closure through the exact
digest-pinned Sourcey Candidate Verifier. A required external admission check
binds evidence to the exact pull-request head. Once an admitted pull request is
merged, publication and live activation are automatic.
