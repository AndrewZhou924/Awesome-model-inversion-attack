# Contributing

Contributions are welcome through pull requests or issues.

## Entry format

Please provide:

```text
Year | Paper | Domain | Target/observable | Access | Auxiliary data/prior |
Attack or defense | Venue/status | Paper URL | Code URL (optional)
```

Use an official publisher, conference, proceedings, OpenReview, ACL Anthology, PMLR, CVF/ECVA, USENIX, DOI, or arXiv link whenever possible.

## Status labels

- `peer-reviewed`: published in proceedings or a journal.
- `accepted`: officially accepted but proceedings are not yet available.
- `preprint`: arXiv or another non-peer-reviewed manuscript.
- `withdrawn submission`: a submission record that was withdrawn; do not label it as a conference publication.

## Scope

Classical model inversion uses information exposed by a trained model to reconstruct private training information or sensitive characteristics. Please label the following as **adjacent reconstruction** unless the paper explicitly studies the classical MIA threat model:

- gradient inversion from shared training gradients;
- training-data extraction by prompting a generative model;
- model or embedding inversion for interpretation rather than privacy attacks;
- inversion of unlearning or concept-erasure mechanisms;
- attacks on synthetic-data releases.

## Quality checks

Before submitting:

1. Search the repository for duplicate titles and earlier versions.
2. Merge preprint and final versions into one entry when they represent the same work.
3. Verify authors, title, venue, year, pages, DOI, and current publication status.
4. State the exposed interface and recovered target rather than using only “white-box” or “black-box”.
5. Avoid copying abstracts; add at most one original sentence describing the contribution.
