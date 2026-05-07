# apex-ecco

Source for **etherealconnectionsco.com** — ECCO's main canonical surface. The
apex carries the brand, the service tiers, the Transparency Project Heart Room,
the Sentient Security Checkpoint front door, and the `/why` companion surface.

## Posture

Public repository. Published under CC BY-NC-ND 4.0. The apex is ECCO's
front door — visibility supports discovery and provenance verification.
Licensed for non-commercial reading, citation, and linking; commercial
repackaging requires permission. See `LICENSE` for full terms.

## Doctrine

Every external claim resolves to live content. Every link verifiable.
Live = reachable by a human in a browser. Not "reachable by every bot."

The build pipeline enforces this — `node check-links.mjs index.html` runs
on every deploy, and the build fails on any unrecognized 4xx/5xx response.
The previous good version stays live until the next green build.

> Every claim verifiable. Every link live. Build pipeline enforced.

## Stack

- **Source:** single-file `index.html` (vanilla HTML/CSS/JS, no framework)
- **Build gate:** `check-links.mjs` v4 (Node 20+, zero dependencies, native fetch)
- **Host:** Netlify, Git-driven CI from this repo
- **Config:** `netlify.toml`

## Files

| File | Purpose |
|------|---------|
| `index.html` | Apex source — diamond glass aesthetic, sentient checkpoint, full canonical surface |
| `404_main_site.html` | Custom 404 page |
| `_redirects` | Netlify routing config |
| `privacy-policy.html` | Privacy policy (carrier-compliant, A2P-10DLC vetting) |
| `terms.html` | Terms (carrier-compliant) |
| `why/index.html` | `/why` companion surface (under continued development; published per transparency doctrine) |
| `intro.mp4` | Hero intro video |
| `coin.mp4` | E-Axiom coin animation |
| `etree.mp4` | E-Tree closing animation |
| `etree.jpg` / `etree.png` | E-Tree static variants |
| `tree.jpg` | E-Tree section anchor image |
| `seal.jpg` | ECCO seal asset |
| `arrow-qr.png` | E-Axiom QR arrowhead |
| `OIP.jpg` | Open Graph preview image |
| `check-links.mjs` | Build-time link integrity gate (port from scan-ecco) |
| `netlify.toml` | Netlify build configuration |
| `LICENSE` | CC BY-NC-ND 4.0 |

## License & use

Published under CC BY-NC-ND 4.0. See `LICENSE` for full terms.

**You may:** read, link to, cite, and share for non-commercial purposes with
attribution to Ethereal Connections Co.

**You may not:** repackage, rebrand, fork-and-resell, incorporate into paid
products, paid courses, paid newsletters, or any commercial offering without
prior written permission.

For commercial licensing, partnership, or any use beyond the terms above:

**jeremiah@etherealconnectionsco.com**

## Doctrinal artifacts in play

This repo joins `scan-ecco`, `toolkit-ecco`, `mirror-ecco`, and `master-context`
on the public-surface side, and `commission-ecco` (private, all rights
reserved) on the closed-methodology side. The build pipeline is the same on
every surface; what differs is the visibility posture and the surface-specific
integrity profile.

The `/why` companion surface is published under continued-development
posture — transparency over polish, provenance over performance. The act of
making the work inspectable while it is still being built is itself the
doctrine in operation.

Part of the Track G Phase 2 migration from Netlify Drop to Git-driven CI.

---

*Provenance over performance. Infrastructure over influence. Doctrine over excuse.*
