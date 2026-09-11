# Cardinal public documentation

This repository is the canonical Mintlify source for [docs.cardinalweb3.com](https://docs.cardinalweb3.com).

## Deployment

- **Source:** `CardinalKennyS/PublicDocs`
- **Production branch:** `main`
- **Preview:** Mintlify creates a preview deployment for pull-request branches.
- **Release:** The Mintlify GitHub app deploys the merged `main` branch to `https://cardinal-web3.mintlify.app`, which serves the public custom domain.
- **Owner:** Kenneth Scally approves public product wording and production publication.

The `Cardinal-Web3/cardinal-docs` repository is an internal documentation and drafting workspace. A merge there does not update the live Mintlify site.

## Reviewed publishing workflow

1. Create a focused branch from `main`.
2. Open a draft pull request and link the relevant Cardinal roadmap issue.
3. Check the Mintlify preview for navigation, links, code examples, mobile layout, and status labels.
4. Obtain technical review for product, API, data, smart-contract, security, or compliance claims.
5. Obtain Kenneth's approval for investor-facing and public wording.
6. Mark the pull request ready and merge it into `main`.
7. Verify the Mintlify deployment and the affected pages on the public domain.

Do not commit provider credentials, restricted data, partner payloads, production secrets, or unapproved contract addresses.

## Rollback

If a published change is inaccurate or breaks the site:

1. Revert the merge commit through a reviewed pull request.
2. Merge the revert into `main`.
3. Confirm that Mintlify redeploys the last approved content.
4. Record the incident and corrective action on the linked GitHub issue.

Avoid rewriting `main` history or force-pushing a rollback.

## Local preview

Run the Mintlify development server from the repository root:

```bash
mint dev
```

See the [Mintlify documentation](https://mintlify.com/docs) for supported installation and preview options.
