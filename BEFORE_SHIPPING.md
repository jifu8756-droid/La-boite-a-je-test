# Before shipping on GitHub Pages

This checklist describes the deployment files in this directory. The site is static HTML/CSS and can be published without a build step.

## Remaining legal placeholders

There are **7 `.placeholder` chips** in the five legal pages:

| Page | Placeholder | What closes it |
|---|---|---|
| `mentions-legales.html` | OVH phone number | Replace with the verified host's name, address, and phone after final hosting is chosen. |
| `mediation-consommation.html` | Mediator name | Contract with a consumer mediator and enter its name. |
| `mediation-consommation.html` | Mediator postal address | Enter the contracted mediator's address. |
| `mediation-consommation.html` | Mediator website | Enter the contracted mediator's website. |
| `confidentialite.html` | Reservation tool | Name the appointment provider if/when one is selected and document its data handling. |
| `cookies.html` | Audience-measurement tool | Confirm whether analytics will be used; name it if so. |
| `cookies.html` | Online booking tool | Name the booking provider if/when integrated and describe its trackers. |

## Functional/content checks

- `modalites-rendez-vous.html` has a static appointment request form with `action="#"`; it does not submit to a backend.
- `qui-suis-je.html` has a separate question form with `action="#"`; it does not submit to a backend. All “Me poser une question” links lead to that form.
- `cgv.html` describes an online booking agenda, but this Calendly-free snapshot contains no booking tool. Match the page copy to the actual service before publishing.
- `cookies.html` contains text about cookies and a consent interface. Check that the final wording matches the actual deployed site and any embedded third-party services.
- Two empty image slots remain in `etre-accompagne.html` and `mon-approche.html`.
- Saturday hours are still “Horaires à préciser” in `modalites-rendez-vous.html`.
- The legal notice names OVH as host. Change this to GitHub Pages (or the actual hosting arrangement) before publishing the legal information.
- Configure a custom domain only if desired. Add the final domain to the sitemap if one is created; this copy currently has no `robots.txt` or sitemap.
- `assets/logo.png` is used as a PNG favicon; no `favicon.ico` is included.

## Deploy only this folder

Publish the contents of `github-pages/`, not the project root. This directory contains:

- `index.html` and `index_test2.html`
- `etre-accompagne.html`, `mon-approche.html`, `qui-suis-je.html`, `modalites-rendez-vous.html`, `faq.html`
- `mentions-legales.html`, `confidentialite.html`, `cookies.html`, `cgv.html`, `mediation-consommation.html`
- `assets/` shared CSS and referenced images
- `README.md` and this checklist (remove these two Markdown files from the public branch if you do not want them served)

The project-root archives, `references/`, `version1/`, and `new_legal_pages_tmp/` are excluded from this deploy copy.
