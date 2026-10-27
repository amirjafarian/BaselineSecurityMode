# Copilot instructions for BaselineSecurityMode

An independent, community-authored technical guide to Baseline Security Mode (BSM) and related
Microsoft 365 security settings. The deliverable is one self-contained HTML file,
`guide/bsm-technical-guide.html`, published through GitHub Pages from `main`. The site landing page
is `index.md` and the root `README.md` is GitHub-only.

## Content rules (public source only)

- Use **public Microsoft Learn documentation only** (`https://learn.microsoft.com/en-us/...`, no
  query strings). Every statement about what a setting does, its values, scope, roles, impact or
  reversal must be supported by a linked public page. If a page names a policy but gives no value,
  say "Confirm the value in the Learn page" instead of guessing.
- Never add tenant data, customer names or identifiers, internal tooling or programme labels,
  email addresses, local file paths, non-public documents or screenshots of them.
- Keep wording neutral and independent. Do not imply that Microsoft authored, endorses, supports or
  mandates the guide, its phases or its impact labels. The phases and the Low / Medium / High /
  Nothing to do labels are planning aids.
- Keep **Permanent** (cannot be reversed), **Reversible** and **Service-managed** distinct, and
  keep the red outline on permanent items. Do not present a permanent change as reversible.
- Recheck the linked Learn pages before updating the "public documentation reviewed" date, and
  record that date in `CHANGELOG.md`.

## The guide file

- It is a generated single file with inline CSS and JavaScript. Keep it **self-contained**: no
  external scripts, fonts, images or CDNs, so it works offline and when emailed on its own.
- Do not hand-edit unrelated parts. Replace the whole file with a new build, then check it in a
  browser at narrow (about 390px), desktop and ultrawide widths: header, tabs, settings explorer
  (three columns on wide screens), the setting detail dialog, and the footer (review/generation
  line at the bottom and the independent-community badge at bottom right).

## Docs site

- Jekyll with the just-the-docs remote theme (`_config.yml`). Pages source branch is `main`, path
  `/`. Local preview (needs Ruby): `bundle install` then `bundle exec jekyll serve`, then open
  `http://127.0.0.1:4000/BaselineSecurityMode/`.
- Docs must be audience-neutral. Standalone HTML is embedded in `index.md` through an iframe, with
  full-screen and download links.

## Branches, commits and releases

- Work on a feature branch and open a PR into `main`. Do not push directly to `main`.
- Commit subjects are imperative and at most 72 characters. The body explains why. On
  AI-assisted commits, end with `Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>`.
- Tag releases `vX.Y.Z` and keep `CHANGELOG.md` (Keep a Changelog format) in step.
