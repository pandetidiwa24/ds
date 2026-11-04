# DS Digital Lab

Personal Data Science lab portal for **Pandeti Diwakar** (24102A030066, DS-2), Mohan Babu University.

The whole site is a single, dependency-free `index.html` with hash-based routing, so it can be hosted directly on GitHub Pages.

## Live site

After GitHub Pages is enabled: <https://pandetidiwa24.github.io/ds/>

## Enable GitHub Pages

1. Open the repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch **main** and folder **/ (root)**, then **Save**.
4. Wait for the deployment to finish and open the live URL above.

The `.nojekyll` file tells GitHub Pages to serve the files as-is.

## Local preview

```bash
python -m http.server 8000
```

Then open <http://localhost:8000/>.

## Customising

All personal details live in the `CONFIG` block near the top of the `<script>` in `index.html`:

- `portal` – site name, university and year
- `student` – name, roll number, section, subject, faculty and social links
- `sandbox.backendUrl` – optional Python runner endpoint (leave empty for demo mode using saved notebook outputs)

Experiments, modules and tools are defined below `CONFIG`. Progress and edits are stored in the browser's `localStorage`; use **Export JSON** / **Import JSON** on the Experiments page to back them up.
