# Niko Kavakiotis - Anthropic Application Portfolio Website

A professional portfolio website built for the Anthropic GTM Strategy & Operations (Industries), EMEA application. The site demonstrates industry GTM expertise through comprehensive Healthcare and Manufacturing playbooks built collaboratively with Claude.

## Quick Start: Deploy to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create an account)
2. Click the **+** icon in the top right, then **New repository**
3. Name it: `nikokavakiotis.github.io` (this exact name enables GitHub Pages at the root)
   - Or use any name like `portfolio` (will be available at `nikokavakiotis.github.io/portfolio`)
4. Set to **Public**
5. Click **Create repository**

### Step 2: Upload Files

**Option A: Via GitHub Web Interface (Easiest)**

1. In your new repository, click **uploading an existing file**
2. Drag and drop ALL files from this `website` folder:
   - `index.html`
   - `style.css`
   - `case-studies.html`
   - `why-anthropic.html`
   - `thought-leadership.html`
   - `playbooks/` folder (with `healthcare.html` and `manufacturing.html`)
3. Click **Commit changes**

**Option B: Via Git Command Line**

```bash
# Navigate to the website folder
cd "C:\users\NikoKavakiotis\Claude\CILS\Job_Search\Anthropic\website"

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial portfolio website for Anthropic application"

# Add remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, go to **Settings** (top tab)
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes for deployment
6. Your site will be live at: `https://YOUR_USERNAME.github.io/` or `https://YOUR_USERNAME.github.io/REPO_NAME/`

### Step 4: Verify and Test

1. Visit your live URL
2. Test all navigation links
3. Check mobile responsiveness (resize browser or use phone)
4. Verify all pages load correctly

---

## File Structure

```
website/
├── index.html                 # Homepage with profile and key stats
├── style.css                  # All styles (single CSS file)
├── case-studies.html          # Detailed Siemens case studies
├── why-anthropic.html         # Extended "Why Anthropic" essay
├── thought-leadership.html    # TedX, publications, certifications
├── playbooks/
│   ├── healthcare.html        # Healthcare AI GTM Framework
│   └── manufacturing.html     # Manufacturing AI GTM Framework
└── README.md                  # This file
```

## Customization Checklist

Before submitting your application, consider these customizations:

### Required

- [ ] Add your actual profile photo (replace the "NK" placeholder in `index.html`)
- [ ] Verify your LinkedIn URL is correct
- [ ] Verify your email address is correct
- [ ] Update the TedX talk link when available

### Optional Enhancements

- [ ] Add actual TedX video embed (replace placeholder in `thought-leadership.html`)
- [ ] Add links to specific published articles
- [ ] Add a favicon (currently uses text-based SVG)
- [ ] Purchase custom domain (e.g., nikokavakiotis.com) and point to GitHub Pages

---

## Adding Your Profile Photo

1. Add your photo to the website folder (e.g., `photo.jpg`)
2. In `index.html`, find this line:
   ```html
   <div class="profile-placeholder">NK</div>
   ```
3. Replace with:
   ```html
   <img src="photo.jpg" alt="Niko Kavakiotis" class="profile-image">
   ```
4. Commit and push the changes

---

## Connecting a Custom Domain (Optional)

If you purchase a domain like `nikokavakiotis.com`:

1. In your repository, go to **Settings** > **Pages**
2. Under **Custom domain**, enter your domain
3. At your domain registrar, add these DNS records:
   - A record: `185.199.108.153`
   - A record: `185.199.109.153`
   - A record: `185.199.110.153`
   - A record: `185.199.111.153`
   - CNAME record: `www` pointing to `YOUR_USERNAME.github.io`
4. Wait for DNS propagation (up to 24 hours)
5. Enable **Enforce HTTPS** in GitHub Pages settings

---

## Using the Website URL in Your Application

In the Anthropic application form, there's an optional **Website** field. Enter:

```
https://YOUR_USERNAME.github.io/
```

Or if using a custom domain:
```
https://nikokavakiotis.com
```

This will stand out because:
- 99% of applicants leave this field blank
- It demonstrates Claude expertise (the playbooks were built with Claude)
- It shows the exact deliverables you'd create in the role
- It proves you understand Anthropic's product and mission

---

## Technical Notes

- **No build process required** - pure HTML/CSS, deploys instantly
- **No dependencies** - no npm, no frameworks, no JavaScript libraries
- **Mobile responsive** - works on all device sizes
- **Print-friendly** - CSS includes print styles for case studies
- **Fast loading** - single CSS file, no external resources

---

## Support

If you encounter issues:
1. GitHub Pages troubleshooting: [docs.github.com/pages](https://docs.github.com/en/pages)
2. Check browser console for errors (F12 > Console)
3. Verify all file paths are correct (case-sensitive on some systems)

---

*This website was built collaboratively with Claude as a demonstration of AI-assisted GTM strategy development.*
