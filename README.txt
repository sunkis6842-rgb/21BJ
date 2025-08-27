
Hank Blackjack 21 — Web-only Deploy Pack
========================================

This pack lets you deploy WITHOUT installing any software.

Option A — GitHub Pages (pure web UI)
-------------------------------------
1) Go to https://github.com/new and create a new public repository (e.g., hanks-bj21).
2) Click "Add file" → "Upload files", upload the two files in this folder:
   - index.html
   - (this) README.txt
   Commit the changes.
3) Go to the repo "Settings" → "Pages" → "Build and deployment":
   - Source: "Deploy from a branch"
   - Branch: "main" / folder: "/ (root)"
   - Save. Wait for it to build.
4) Your site will be at: https://<your-username>.github.io/<repo-name>/

Option B — Any static host that allows file upload (Netlify Drop, etc.)
-----------------------------------------------------------------------
Upload index.html and you are done.

Notes
-----
- Firestore/Firebase config is embedded in index.html and works from any host.
- If Firestore shows "needs composite index", click the console link to auto-create it once.
- Make sure Anonymous Auth is enabled in Firebase Auth console.
