# Vedank Ayurveda Wellness — Website

Static HTML website for Vedank Ayurveda Wellness Clinic, Greater Noida. No build step required — every page is a self-contained HTML file (images are embedded as base64, so there are no separate asset folders to manage).

## Pages

| File | Purpose |
|---|---|
| `index.html` | Home page |
| `liver.html` | Liver Care program (flagship specialty) |
| `chronic-care.html` | Chronic disease hub — joint, neurological, skin, metabolic, digestive, respiratory, women's health, mental wellness |
| `services.html` | Services overview |
| `doctors.html` | Doctor team profiles |
| `contact.html` | Contact / consultation booking |
| `fatty-liver-landing.html` | Standalone ad landing page (e.g. for Google Ads campaigns) |
| `privacy-policy.html` | Privacy policy |
| `terms.html` | Terms & conditions |
| `disclaimer.html` | Medical disclaimer |

## Deploying to GitHub Pages

1. Create a new repository on GitHub (or use an existing one) and upload all files in this folder to the repository root.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`.
4. Choose the branch (usually `main`) and folder `/ (root)`, then click **Save**.
5. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.
6. To use a custom domain, add a `CNAME` file with your domain name and configure your DNS provider's A/CNAME records per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Notes for future edits

- Colour palette is set via CSS custom properties near the top of each file's `<style>` block (e.g. `--green`, `--gold`, `--cream` on most pages; `--forest`, `--green`, `--gold`, `--cream` on the legal pages and Chronic Care). Change the hex values there to re-theme a page without touching the rest of the CSS.
- `chronic-care.html` renders its disease list from a JavaScript data array near the bottom of the file — add a new condition by adding an object to the relevant category's `diseases` array.
- All internal links are relative (`href="liver.html"`, etc.), so the site works identically whether hosted at a domain root or in a GitHub Pages subpath.
