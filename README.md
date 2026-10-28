# Kavin Prathi Chellamuthu – Portfolio

A responsive, dark-themed developer portfolio built with plain HTML5, CSS3 and JavaScript (no frameworks).

## Files

```
portfolio/
├── index.html   # content and structure
├── style.css    # design, theme colours, responsive layout
├── script.js    # navigation, animations, form, and the CONFIG block
└── images/      # (optional) put profile.jpg here
```

## 1. Create the files
1. Make a folder called `portfolio`.
2. Put `index.html`, `style.css` and `script.js` inside it (same folder).
3. Optional: create an `images` folder for your photo.

## 2. Run it locally
- **Simplest:** double-click `index.html` to open it in your browser.
- **Better (local server):** in the folder run `python -m http.server 8000`, then open <http://localhost:8000>.
- **VS Code:** install the *Live Server* extension, right-click `index.html` → *Open with Live Server*.

Icons and the Inter font load from free CDNs, so you need an internet connection the first time.

## 3. Edit the content
- **GitHub / LinkedIn:** open `script.js`, fill in `PROFILE_LINKS`. Every GitHub and LinkedIn button updates automatically.
- **Project links:** fill in `PROJECT_LINKS` in `script.js`. Buttons appear only for URLs you add.
- **Text, projects, experience:** edit `index.html`. Each section is marked with a comment such as `<!-- ===== EXPERIENCE ===== -->`.
- **Certifications:** replace the `[Add Certifications]` card in the *Certifications & Achievements* section.
- **Phone number:** it's on your CV but not shown publicly. Add a `<li>` in the contact list if you want it displayed.
- **Colours:** change `--accent` and `--accent-2` at the top of `style.css`.
- **Personal projects:** the CV lists none, so the project cards are built from your work experience. Add real personal projects by copying a `<article class="card project reveal" data-project="...">` block.

## 4. Add a profile photo
1. Save a square photo (at least 600×600) as `images/profile.jpg`.
2. In `script.js` set `const PROFILE_PHOTO = "images/profile.jpg";`.

## 5. Make the contact form send real email
The site is static, so the form currently opens the visitor's email app (`mailto:`). For real delivery:
- **Formspree / Netlify Forms / EmailJS** are free options. Replace the `mailto` block in the form's submit handler in `script.js` with a `fetch()` call to the service.

## 6. Deploy for free

### GitHub Pages
1. Create a GitHub repository (e.g. `portfolio`) and upload the three files (and `images/` if used).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
4. After a minute your site is live at `https://<your-username>.github.io/portfolio/`.

### Netlify
1. Sign in at netlify.com.
2. Choose **Add new site → Deploy manually** and drag your `portfolio` folder onto the page.
3. Netlify gives you a live URL immediately; you can rename it under **Site settings**.
