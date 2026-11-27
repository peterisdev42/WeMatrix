# Contributing to WeMatrix

## Contributor licensing

The planned contribution policy for WeMatrix is a non-exclusive CLA, separate from the public open-source license. The [proposed CLA](CLA.md) is **not yet effective**; do not sign it or merge external copyrightable contributions until the final agreement and checks are active.

The GitHub Actions workflow will direct contributors to the immutable approved agreement and provide the exact signing comment. Before acceptance, clearly explain the broad commercial, proprietary, cross-project and transferable licensing rights, the absence of a perpetual open-source commitment, and the public signature metadata. Implement any separately required privacy consent and preserve evidence of the accepted agreement and declaration. The CLA covers eligible historical, current and future submissions only after actual valid acceptance; ordinary feedback is excluded. Signature metadata is stored publicly on the [cla-signatures branch](https://github.com/peterisdev42/WeMatrix/tree/cla-signatures); do not submit sensitive personal information. Contributors retain their copyright. No DCO or separate service account is required.

### Maintainer activation and verification

1. Privately document the Project Owner's legal identity and its association with GitHub numeric User ID 340498199. Arrange appropriate legal review of CLA v1.0, including governing law, patent terms, electronic acceptance, historical and corporate contributions. Provide a private legal/privacy contact channel and review applicable privacy notice, separate consent, public disclosure and cross-border processing requirements. Approve the final text and remove the draft status and review notices only when these prerequisites are satisfied.
2. Commit the final `CLA.md` to main, then create repository Actions variable `CLA_DOCUMENT_SHA` with that full commit SHA. Every distinct SHA uses an independent signature file; retain all earlier records.
3. Verify the Action on an actual external fork PR, including a failed unsigned check, a successful signed recheck, and a new commit. Do not create fake signatures or treat this draft as accepted. The Action initializes its JSON file automatically.
4. In repository rules, require a PR and the observed CLA check on main; keep existing checks, disable force pushes/deletion on main and cla-signatures, and permit the Action to append to cla-signatures. Do not require a PR for the signatures branch. Do not activate required checks while the CLA variable is unset. Protect changes to the CLA workflow and policy; a skipped check is not proof of a valid signature.
5. Confirm the PR is still open and its current head has been checked. The coverage guard blocks PRs over 100 commits, unlinked authors, unsupported co-authored commits and unaccounted PR authors; resolve authorization independently before permitting a merge. Review third-party and corporate rights separately. The Action does not itself prove legal identity or copyright ownership.
6. Back up signature records and immutable agreement versions. Retain previous authorization evidence on any change; disable any overlapping CLA GitHub App only after preserving existing records, if any.

The workflow uses a pinned StepSecurity Action and the repository GITHUB_TOKEN only. It does not execute or check out external PR code.
