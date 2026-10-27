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
  N/A labels are planning aids. **N/A** means Microsoft already enforces or has retired the
  behavior, so the customer has nothing to configure.
- Keep **Permanent** (cannot be reversed), **Reversible** and **Service-managed** distinct, and
  keep the red outline on permanent items. Do not present a permanent change as reversible.
- Recheck the linked Learn pages before updating the "public documentation reviewed" date, and
  record that date in `CHANGELOG.md`.

## The guide file

- It is a generated single file with inline CSS and JavaScript. Keep it **self-contained**: no
  external scripts, fonts, images or CDNs, so it works offline and when emailed on its own. The
  generator is maintained outside this repository. Replace the whole file with a new build for
  structural changes; for a small wording or link fix, edit only the affected text and keep the
  embedded JSON valid.
- Required page elements: the title "Microsoft 365 security configuration guide - Baseline
  Security Mode (BSM)" linked (new tab, `rel="noopener noreferrer"`) to Microsoft's public Baseline
  Security Mode settings page on Microsoft Learn; a footer with the unofficial disclaimer, the
  "public documentation reviewed / generated" line at the bottom, a link to this repository, and the
  "Independent community guide - public Microsoft documentation only" badge at the bottom right.
- Impact labels are **Low / Medium / High / N/A**. N/A is for behavior Microsoft already enforces or
  has retired (nothing for the customer to configure). Do not reintroduce "Nothing to do" or
  internal-style labels.
- Setting links must be direct `https://learn.microsoft.com/en-us/...` pages without query strings.
  The title link is the one deliberate exception and keeps `?view=o365-worldwide`.
- Check the file in a browser at narrow (about 390px), desktop and ultrawide widths: header, tabs,
  settings explorer (three columns on wide screens), the setting detail dialog, and the footer.

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
- Tag releases `vX.Y.Z` and keep `CHANGELOG.md` (Keep a Changelog format) in step. Versions 1.0.0
  to 1.0.3 are recorded in the changelog but have not been tagged yet.
- After a merge to `main`, confirm the GitHub Pages build succeeds and the live guide at
  `https://amirjafarian.github.io/BaselineSecurityMode/guide/bsm-technical-guide.html` shows the
  change. Git normalizes line endings, so compare content, not raw bytes.
