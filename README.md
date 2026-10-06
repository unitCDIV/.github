# unitCDIV/.github

The public home of **Unit 404 — Cyber Division (CDIV)** on GitHub. This repository holds:

| Path | Purpose |
|:--|:--|
| `index.html`, `assets/` | Landing page for CDIV's open-source activity, served at **https://unitcdiv.github.io/.github/** |
| `profile/README.md` | The profile shown on the [unitCDIV organisation page](https://github.com/unitCDIV) |
| `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md` | Community health files, used as defaults by every repository in the organisation |
| `.github/ISSUE_TEMPLATE/` | Issue forms for content errors, broken links and lesson proposals, also organisation-wide defaults |
| `LICENSE`, `LICENSE-CONTENT` | MIT for this page's code, CC BY-NC 4.0 for written content |

The curriculum itself is at **https://unitcdiv.fairytale.ai/**. Its source is private and deployed separately; public feedback on it comes in through this repository's issues.

## Landing page

Plain HTML, one stylesheet and one small ES module. There is no build step and no third-party code. The module adds the theme toggle and lists public repositories and recent activity from the GitHub API, and the page works without it. A Content Security Policy allows only same-origin assets, the hashed inline theme script, and `connect-src https://api.github.com`.

Preview locally:

```bash
python -m http.server 8000
```

Then open http://localhost:8000/.

### Deploy

**Settings → Pages → Source:** *Deploy from a branch*, branch `main`, folder `/ (root)`. Leave **Custom domain** empty. The page is served at `https://unitcdiv.github.io/.github/`.

`.nojekyll` makes GitHub Pages serve the files as they are, rather than rendering the Markdown files as extra pages.

## Licence

Page code: [MIT](LICENSE). Written content: [CC BY-NC 4.0](LICENSE-CONTENT), the same licence as the CDIV lessons. The curriculum site's own code is proprietary; see its [licensing page](https://unitcdiv.fairytale.ai/attribution/).
