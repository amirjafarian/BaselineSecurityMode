# Baseline Security Mode technical guide

An independent, community-authored technical guide to **Baseline Security Mode (BSM)** in the
Microsoft 365 admin center and the related identity, device, email and audit protections.
It summarizes public Microsoft Learn documentation and links to the original pages.

> 📖 **Read it online:** <https://amirjafarian.github.io/BaselineSecurityMode/>
>
> 📄 **Standalone file:** [`guide/bsm-technical-guide.html`](guide/bsm-technical-guide.html) is a
> single self-contained page. Download it and open it offline, or share it on its own.

## What it covers

27 settings in five groups, with search and filters in a settings explorer:

| Group | Settings |
|---|---|
| Phase 1 - Start here | 7 |
| Phase 2 - Expand protection | 7 |
| Phase 3 - Broader security | 7 |
| Other identity controls | 3 |
| Teams Rooms guidance | 3 |

For each setting the guide gives what it does, the likely user impact, how to check impact first,
how to configure and reverse it (including the Microsoft 365 admin center, Office Cloud Policy for
specific groups of users, and PowerShell where the public documentation describes them), who can
change it, and links to the Microsoft Learn pages.

Other sections cover impact and reversal (reversible, permanent and service-managed settings),
products and admin surfaces, and a copyable deployment plan.

## Please note

- The phases and the **Low / Medium / High / N/A** impact labels are planning aids. They are not
  Microsoft requirements, a mandated order or a guarantee of no impact.
- **N/A** means Microsoft already enforces or has retired the behavior, so there is nothing to
  configure.
- Some changes are permanent or service-managed and cannot be reversed. The guide marks these.
- Always review the current Microsoft documentation, your licensing and your change process, and
  pilot with representative users before you configure a production environment.

## Disclaimer

This is an independent, personal community project. It is **not an official Microsoft publication**
and is not endorsed or supported by Microsoft. The content is provided **AS IS** without warranty
of any kind, and you use it at your own risk. Information changes; the linked Microsoft Learn
pages are the authoritative source.

Microsoft, Microsoft 365, Microsoft Entra, Microsoft Defender, Microsoft Purview, Microsoft Teams
and other product names are trademarks of the Microsoft group of companies.

## Contributing and corrections

Open an issue for a correction. Please include the public Microsoft Learn page that supports it.
Content in this repository is limited to public Microsoft documentation and your own public
observations.

## License

Released under the [MIT License](LICENSE).
