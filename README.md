# Design Atlas: 9-week Interaction Design prep

Responsive, dark-mode, self-contained static site. No build step.

## Publish to GitHub Pages
1. Create a new repository (public if using GitHub Pages on a free personal account).
2. Upload `index.html`, `content.json`, `papers/`, and `.nojekyll` to the repository root.
3. Under **Settings → Pages**, set **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Open the Pages URL after the deployment succeeds.

## How progress is stored
Writing, scores and reading statuses autosave in browser localStorage.
Use **Your data → Download backup** regularly.

## Optional cross-device sync
1. Create a **separate private GitHub repository** for data; do not place `progress.json` in the public Pages repository.
2. Create a fine-grained personal access token for the private data repository, with **Contents: Read and write**.
3. Open **Your data** on your trusted device, supply owner, repo, `progress.json`, token, then choose Save to GitHub or Restore from GitHub.
4. The token is not saved by Design Atlas. Re-enter it in a new tab/session. Keep it private.
5. GitHub sync is manual and does NOT merge concurrent edits. Make a backup before restoring.

Avoid storing personal or confidential material in public repositories. Hosting does not require a GitHub token.
