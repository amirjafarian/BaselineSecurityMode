---
title: Home
layout: home
nav_order: 1
description: "Independent community guide to Baseline Security Mode and related Microsoft 365 security settings."
permalink: /
---

# Baseline Security Mode technical guide

An independent, community-authored technical guide to **Baseline Security Mode (BSM)** in the
Microsoft 365 admin center and the related identity, device, email and audit protections. It
summarizes public Microsoft Learn documentation and links to the original pages.

> ⚠️ **Review first, then deploy.** The phases and the Low / Medium / High / Nothing to do impact
> labels are planning aids, not Microsoft requirements or guarantees. Some changes are permanent or
> service-managed and cannot be reversed. Pilot with representative users before you change a
> production environment.

[Open the guide full-screen ↗]({{ '/guide/bsm-technical-guide.html' | relative_url }}){: .btn .btn-primary target="_blank" }
[Download the standalone file ↗]({{ '/guide/bsm-technical-guide.html' | relative_url }}){: .btn target="_blank" download }

The guide is a **single self-contained HTML file**
(`guide/bsm-technical-guide.html`). It has its own theme and needs no server, so you can share it
on its own, or open it offline, and it still works.

---

<iframe
  src="{{ '/guide/bsm-technical-guide.html' | relative_url }}"
  title="Baseline Security Mode technical guide"
  loading="lazy"
  style="width:100%;height:85vh;min-height:640px;border:1px solid #d0d7de;border-radius:6px;background:#fff"></iframe>

---

## What it covers

27 settings in five groups, with a searchable settings explorer:

| Group | Settings |
|---|---|
| Phase 1 - Start here | 7 |
| Phase 2 - Expand protection | 7 |
| Phase 3 - Broader security | 7 |
| Other identity controls | 3 |
| Teams Rooms guidance | 3 |

For each setting: what it does, the likely user impact, how to check impact first, how to configure
and reverse it, who can change it, and links to the Microsoft Learn pages. See the
[Changelog]({{ '/changelog/' | relative_url }}) for what changed in each release.

## Disclaimer

This is an independent, personal community project. It is **not an official Microsoft publication**
and is not endorsed or supported by Microsoft. The content is provided **AS IS** without warranty of
any kind, and you use it at your own risk. Information changes; the linked Microsoft Learn pages are
the authoritative source. See the [LICENSE](https://github.com/amirjafarian/BaselineSecurityMode/blob/main/LICENSE).

Microsoft, Microsoft 365, Microsoft Entra, Microsoft Defender, Microsoft Purview, Microsoft Teams
and other product names are trademarks of the Microsoft group of companies.
