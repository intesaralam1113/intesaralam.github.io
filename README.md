# Intesar Alam — Portfolio Website

A professional mechanical engineering portfolio built with plain HTML, CSS, and JavaScript. No build tools, no frameworks — deploy anywhere in seconds.

---

## Folder Structure

```
portfolio/
├── index.html              ← Main portfolio page
├── assets/
│   ├── css/
│   │   └── style.css       ← All styling
│   ├── js/
│   │   └── main.js         ← Interactions & animations
│   └── images/             ← Add your images here
│       ├── photo.jpg       ← YOUR PROFILE PHOTO (replace placeholder)
│       ├── project-*.jpg   ← Project images
│       └── ...
├── assets/
│   └── Intesar_Alam_CV.pdf ← ADD YOUR CV HERE
└── README.md
```

---

## Running Locally

### Option 1: VS Code Live Server (Recommended)
1. Install the **Live Server** extension in VS Code
2. Right-click `index.html` → **Open with Live Server**
3. Your browser opens at `http://127.0.0.1:5500`

### Option 2: Python HTTP Server
```bash
cd portfolio/
python -m http.server 8080
# Open: http://localhost:8080
```

### Option 3: Node.js
```bash
cd portfolio/
npx serve .
# Open the URL shown in the terminal
```

---

## Deploying to GitHub Pages

### Step 1 — Create a GitHub Repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon → **New repository**
3. Name it: `intesar-alam` (or `portfolio`, or `your-github-username.github.io`)
4. Set it to **Public**
5. Click **Create repository**

### Step 2 — Upload Files
**Option A: GitHub Web UI (no git required)**
1. Click **Add file** → **Upload files**
2. Drag the entire `portfolio/` folder contents into the upload area
3. Make sure `index.html` is at the root level (not inside a subfolder)
4. Click **Commit changes**

**Option B: Git Command Line**
```bash
cd portfolio/
git init
git add .
git commit -m "Initial portfolio deployment"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** tab
3. In the left sidebar, click **Pages**
4. Under **Source**, select **Deploy from a branch**
5. Set **Branch** to `main`, folder to `/ (root)`
6. Click **Save**
7. Wait 1–2 minutes, then visit: `https://YOUR-USERNAME.github.io/YOUR-REPO/`

---

## Content to Replace (Placeholder Checklist)

### HIGH PRIORITY — Do these first:
- [ ] **Profile photo**: Replace `profile-photo-placeholder` div in `index.html` with:
  ```html
  <img src="assets/images/photo.jpg" alt="Intesar Alam" style="width:100%; display:block;" />
  ```
  Add your actual photo as `assets/images/photo.jpg` (400×500px or similar portrait)

- [ ] **Resume PDF**: Add your CV as `assets/Intesar_Alam_CV.pdf`. The download button links to this file.

- [ ] **Project images**: Replace each `proj-img-placeholder` div with real images:
  ```html
  <img src="assets/images/project-turbine.jpg" alt="Hybrid turbine simulation" />
  ```
  Good sources: ANSYS/COMSOL screenshots, SolidWorks renders, lab photos, CAD views

### MEDIUM PRIORITY — Improve credibility:
- [ ] **GPA / academic standing**: Add to the education section if strong
- [ ] **AIAA DBFC competition rank/result**: Add specific placement if available
- [ ] **Project measurement results**: Add numerical outcomes to any project that has them
- [ ] **LinkedIn URL check**: Verify your LinkedIn profile URL matches what's in the code

### LOW PRIORITY — Polish:
- [ ] **Favicon**: Add a `favicon.ico` at the root, or a simple SVG favicon
- [ ] **OG image**: Add a preview image for social sharing (1200×630px)
- [ ] Add any new projects, publications, or awards as they happen

---

## Final Polish Checklist (After replacing placeholders)

**Content:**
- [ ] Read every section aloud — does it sound confident and natural?
- [ ] All project descriptions have measurable outcomes where possible
- [ ] No placeholder text remains visible
- [ ] LinkedIn profile is complete and matches CV

**Visual:**
- [ ] Profile photo is well-lit, professional, and crops cleanly
- [ ] All project image placeholders are replaced with actual screenshots/renders
- [ ] Test on mobile — does everything reflow correctly?

**Technical:**
- [ ] CV PDF downloads correctly from the button
- [ ] All external links open in a new tab and work
- [ ] Page loads fast (images should be compressed, under 300KB each)
- [ ] Test in Chrome, Firefox, and Safari

**SEO:**
- [ ] Update the `<meta name="description">` tag with 1–2 strong sentences
- [ ] Add a `<link rel="canonical" href="https://your-actual-url.com" />` once live

---

## Customization Tips

**Changing accent color** — Edit this line in `style.css`:
```css
--accent: #c8a96e;  /* Change this hex value */
```

**Adding a new project card** — Copy an existing `.project-card` block in `index.html` and edit the content.

**Adding a new publication** — Copy a `.pub-item` block and fill in the details.

**Changing fonts** — Update the Google Fonts link in `<head>` and the CSS variables:
```css
--font-display: 'YourFont', sans-serif;
--font-body:    'YourBodyFont', serif;
```

---

## Credits
Built for Intesar Alam — GIKI Mechanical Engineering '26.
Design: Engineering precision aesthetic with Syne + DM Mono + Lora type stack.
