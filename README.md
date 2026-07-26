# advisories

Coordinated disclosures in open-source software, and the CVEs that come out of them.

Different discipline from bug bounty work, and a different disclosure path — vendor coordination
rather than programme policy — so it gets its own repository rather than living alongside the
[write-ups](https://github.com/pablodlz/writeups).

## Published

| ID | project | class | severity | fixed in |
| --- | --- | --- | --- | --- |
| | | | | |

Entries appear here only after the fix ships, or after the disclosure deadline passes with the
vendor informed. Anything currently in coordination is deliberately absent — an advisory under
embargo is not a portfolio item, and publishing one early is the fastest way to lose a
maintainer's trust.

## Structure

One directory per advisory:

```
CVE-YYYY-NNNNN-<project>/
  README.md      affected versions, root cause, impact, fixed-in, credit
  timeline.md    reported, acknowledged, patched, published
  poc/           minimal reproducer, pinned to the vulnerable version
```

The reproducer is pinned so the advisory stays verifiable after the project moves on. An
advisory you can no longer reproduce is a claim, not a record.

## Process

1. **Find it in something real.** A dependency of a dependency in an actual engagement beats
   grepping GitHub for `eval(`. Bugs that matter live on paths people execute.
2. **Report to the vendor first** — their `SECURITY.md` if they have one, a GitHub private
   security advisory if they use those, a maintainer email otherwise. Never a public issue.
3. **Wait.** 90 days is the norm. Longer if the maintainer is engaging in good faith; shorter only
   if it is already being exploited in the wild.
4. **Request the CVE** through the vendor's CNA where one exists, MITRE otherwise. The CVE is
   bookkeeping — the fix is the outcome.
5. **Publish here** once the fix ships, with the timeline intact including the parts that went
   slowly.

## The bar

A CVE for a self-XSS in an abandoned repository with four stars is easy to obtain and worth
nothing. People in this field can tell the difference at a glance, and a padded advisory list
reads worse than a short one.

So: real software, real users, real impact, fix shipped. Anything that doesn't clear that bar
doesn't get an entry, no matter how easy the ID would be to claim.

## Related

- [**writeups**](https://github.com/pablodlz/writeups) — bug bounty findings, which follow
  programme policy rather than vendor coordination
- [**pocs**](https://github.com/pablodlz/pocs) — reusable proof-of-concept artefacts
- [**labs**](https://github.com/pablodlz/labs) — deliberately vulnerable reproductions

## Licence

[CC BY 4.0](LICENSE) for the writing. Reproducers are MIT. Neither is authorization to test
anything.
