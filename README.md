# Ebenezer Dream Studio — Portfolio Website

A minimal, elegant portfolio website for showcasing apps, projects, and services.

## 🚀 Quick Start

### Run Locally
```bash
npm run dev
```
This starts a local server at `http://localhost:3000`

### Alternative
```bash
npm run serve
```

## 📁 Project Structure

```
├── index.html               — Homepage
├── projects.html             — All projects listing
├── products.html             — All apps/products listing
├── privacy-policy.html       — Privacy Policy
├── terms-and-conditions.html — Terms & Conditions
├── projects/
│   ├── qr-for-dom.html       — QR for Dom Project Detail
│   └── *.html                — Individual project pages
├── products/
│   ├── qr-for-dom/
│   │   ├── index.html           — QR for Dom App Marketing
│   │   ├── privacy-policy.html  — App-specific Privacy Policy
│   │   └── terms-and-conditions.html — App-specific Terms
│   └── sample-app/           — Sample App directory
├── css/
│   └── style.css             — Design system & all styles
├── js/
│   └── main.js               — Navigation, theme, animations
├── assets/
│   └── images/               — All images
└── .github/
    └── workflows/
        └── deploy.yml        — Auto-deploy to GitHub Pages
```

## 📝 How to Add a New Project

1. **Duplicate** `projects/sample-project.html`
2. **Rename** to your project name (e.g., `projects/my-new-app.html`)
3. **Update** the title, description, images, and content
4. **Add a card** for it on `projects.html` and `index.html` (copy an existing card block)
5. **Commit & push** — the site will auto-deploy

## 📱 How to Add a New App/Product Marketing Page

1. **Duplicate** the `products/sample-app/` folder.
2. **Rename** the folder to your app name (e.g., `products/my-cool-app/`).
3. **Update** `index.html` inside the folder with your title, description, screenshots, and download links.
4. **Update** `privacy-policy.html`, `terms-and-conditions.html`, and `support.html` inside the folder with your app-specific legal and support info.
5. **Add a card** for it on `products.html` and `index.html` linking to `products/my-cool-app/index.html`.
6. **Commit & push** — the site will auto-deploy.

## 🎨 How to Customize

### Change Brand Name
Search and replace "Ebenezer Dream Studio" and "EDS" across all HTML files.

### Change Colors
Edit the CSS custom properties in `css/style.css`:
```css
:root {
  --accent: #4f46e5;        /* Change primary accent color */
  --accent-hover: #4338ca;   /* Darker version for hover */
}
```

### Change Fonts
Update the Google Fonts import at the top of `css/style.css`.

### Dark/Light Mode
The site automatically respects system preferences and also has a manual toggle.

## 🌐 Deployment

### GitHub Pages (Recommended)
1. Push this code to a GitHub repository
2. Go to **Settings → Pages**
3. Source: **GitHub Actions**
4. The workflow at `.github/workflows/deploy.yml` handles the rest

### Custom Domain
1. Buy a domain (Namecheap, Google Domains, etc.)
2. In GitHub repo settings → Pages → Custom domain → Enter your domain
3. Add these DNS records at your domain registrar:
   - `A` record → `185.199.108.153`
   - `A` record → `185.199.109.153`
   - `A` record → `185.199.110.153`
   - `A` record → `185.199.111.153`
   - `CNAME` record → `your-username.github.io`
4. Check "Enforce HTTPS"

### Update Your Site
Just edit files and push to `main`. The site auto-deploys in about 1 minute.

## 📄 Legal Pages

Every app you publish needs a Privacy Policy and Terms & Conditions. The templates are already included:
- `privacy-policy.html` — Update with your specific data practices
- `terms-and-conditions.html` — Update with your specific terms

Link to these from your app store listings.

## 📧 Contact

Update the email address `hello@dreamstudio.dev` in all files to your real email.

---

Built with ❤️ by Ebenezer Dream Studio
