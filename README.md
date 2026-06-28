# Nihed Harbi — Portfolio

Personal portfolio site for **Nihed Harbi**, Control & Automation Engineer.

Live sections: Hero (animated control-loop diagram), About, Experience, Projects, Skills, Education/Certifications, Contact.

## Structure
```
.
├── index.html        # all content
├── style.css         # all styling

```

No build step, no dependencies — just static HTML/CSS. Fonts are loaded from Google Fonts via CDN link.

## Run locally
Open `index.html` directly in a browser, or serve it:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. **Create a new repository** on GitHub — for a personal/profile site, name it exactly:
   ```
   nihed-harbi.github.io
   ```
   (replace `nihed-harbi` with your actual GitHub username). If you'd rather use a normal project repo name (e.g. `portfolio`), that also works — see step 5.

2. **Push this folder to the repo:**
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repo on GitHub → **Settings** → **Pages**
   - Under "Build and deployment" → Source: **Deploy from a branch**
   - Branch: `main`, folder: `/ (root)` → **Save**

4. **Wait ~1 minute**, then your site is live at:
   - `https://<your-username>.github.io/` (if repo is named `<username>.github.io`), or
   - `https://<your-username>.github.io/<repo-name>/` (for any other repo name)

5. **Custom domain (optional):** add a `CNAME` file containing your domain, and configure DNS per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Updating content
- Edit the relevant section in `index.html` directly (Experience, Projects, Skills are plain HTML blocks).
- To swap the resume file, replace `assets/Nihed_Harbi_Resume.pdf` and keep the same filename, or update the `href` in the nav's "Resume" link in `index.html`.
- Colors, fonts, and spacing are controlled by CSS variables at the top of `style.css` (`:root`) if you want to retheme.
