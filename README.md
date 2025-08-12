# assignment-6
This project demonstrates how to host a *static website* (HTML, CSS, JS) for free using *GitHub Pages*.

---

## 📌 Prerequisites
- A [GitHub](https://github.com/) account
- Git installed on your system (optional if uploading via GitHub's web interface)
- Your website files (index.html is mandatory as the main entry point)

---

## 🚀 Steps to Host Your Website

### 1. Create a GitHub Repository
1. Log in to your GitHub account.
2. Click *New repository*.
3. Name it:
   - For a personal site → <username>.github.io
   - For a project site → Any name is fine.
4. Click *Create repository*.

---

### 2. Add Your Website Files
- Place your index.html, CSS, JS, and any assets into the repository.
- Either:
  - *Upload via GitHub* (web interface → "Add file" → "Upload files"), OR
  - *Push via Git*:
    
    git init
    git add .
    git commit -m "Initial commit"
    git branch -M main
    git remote add origin https://github.com/<username>/<repo-name>.git
    git push -u origin main
    

---

### 3. Enable GitHub Pages
1. Go to *Settings* of your repository.
2. Click *Pages* in the left sidebar (under "Code and automation").
3. Under *Source* or *Branch*, select:
   - Branch: main (or your default branch)
   - Folder: / (root)
4. Click *Save*.
5. GitHub will show you your live site URL.

---

### 4. Optional: Custom Domain
1. In *Settings → Pages, add your domain under **Custom domain*.
2. Update DNS records at your domain registrar:
   - Add a *CNAME record* pointing your domain to <username>.github.io.
   - For apex/root domains, configure *A records* with GitHub Pages IP addresses.
3. Wait for DNS propagation (can take minutes to hours).

---

## 🌐 Live Website
Once published, your site will be live at:
- *Personal Site* → https://<username>.github.io/
- *Project Site* → https://<username>.github.io/<repo-name>/

---

## 🔹 Notes
- GitHub Pages only supports *static content* — no PHP, Python, or server-side processing.
- Every change you push to your chosen branch will auto-update the live site.
- Make sure index.html is present at the root.

---

## 📄 Example index.html
