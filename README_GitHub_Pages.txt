
Orbis Curriculum Mapper — GitHub Pages build (V1)
=================================================

This is a **GitHub-optimized** static site. It runs entirely in the browser (no backend).

Files
-----
- index.html (entry point required by GitHub Pages)
- assets/styles.css (styles)
- assets/app.js (logic + demo data)

How to publish on GitHub Pages
------------------------------
1) Create a new public repo (e.g., `curriculum-mapper`).
2) Upload **all files/folders** from this ZIP to the repo root.
3) Go to **Settings → Pages**.
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/root**
4) Visit: `https://<your-username>.github.io/<repo>/` — it will load `index.html` by default.

Local testing (optional)
------------------------
If you open `index.html` by double-clicking, it should work in most cases. If your browser blocks scripts via file://, run a local server:

```bash
python -m http.server 8080
# then open http://localhost:8080/
```

Resetting demo
--------------
If you previously saved data in the browser, the demo may not appear. Clear it in the Console:

```js
localStorage.removeItem('orbis_mapper_state_v1');
```

Built: 2026-02-18 21:02:51
