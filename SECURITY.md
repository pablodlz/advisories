# Security

This repository publishes coordinated disclosures **after** they are fixed, or after their
deadline has passed with the vendor informed. The property that matters here is that nothing
appears before it should.

## Embargoed material is never here

If you maintain a project I have contacted: nothing about your issue is in this repository, in its
git history, or in an unpublished branch, until we have agreed it is public. There is no drafts
directory and no private fork feeding this.

If you believe something published here was released early, or carries more detail than we agreed,
**email pablogalerani@gmail.com and I will unpublish first and discuss afterwards.**

## Reporting a vulnerability to me

This repository is documentation plus minimal reproducers. Email **pablogalerani@gmail.com** if
you find that a reproducer does anything beyond demonstrating its advisory — reaching the network,
touching files outside its own directory, or running against something other than the pinned
vulnerable version.

Reproducers are pinned to the affected version deliberately, so an advisory stays verifiable after
the project moves on. Never point one at a system you do not own.

## Reporting a vulnerability in software I use

Different direction, same principle. I report to the vendor first — their `SECURITY.md`, a private
GitHub advisory, or a maintainer address. Never a public issue, and never here before the fix
ships. The full process is in the [README](README.md).

## Scope

Advisories are published so that users of the affected software can assess their own exposure. A
reproducer is not authorization to run it against anyone else's installation.
