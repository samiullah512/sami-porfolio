# 🎨 Portfolio Customization Guide

## 1. Adding Your Real Images

### Profile Photo
Replace this line in `index.html` (around line 380):
```html
<img src="assets/images/profile.jpg" alt="Sami Ullah">
```
**Tips:**
- Use a professional headshot (400x500px minimum)
- Save as JPG or WebP for smaller file size
- Keep under 200KB for fast loading

### Project Screenshots
Replace these lines:
```html
<!-- Healthcare Project -->
<img src="assets/images/healthcare-dashboard.png" alt="Healthcare Dashboard">

<!-- Customer Behavior Project -->
<img src="assets/images/customer-behavior-dashboard.png" alt="Customer Behavior Dashboard">
```
**Tips:**
- Capture screenshots at 1200x750px
- Use PNG for crisp text/charts
- Compress with [TinyPNG](https://tinypng.com/)

---

## 2. SEO Optimization

### Update Meta Tags
In the `<head>` section of `index.html`:

```html
<!-- Title & Description -->
<title>Sami Ullah | Data Analyst & BI Developer</title>
<meta name="description" content="Portfolio of Sami Ullah...">

<!-- Open Graph (for LinkedIn, Twitter, Facebook) -->
<meta property="og:title" content="Sami Ullah | Data Analyst Portfolio">
<meta property="og:description" content="3+ years experience in Python, SQL, Power BI...">
<meta property="og:image" content="https://YOUR_USERNAME.github.io/samiullah-portfolio/assets/images/preview.png">
<meta property="og:url" content="https://YOUR_USERNAME.github.io/samiullah-portfolio/">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Sami Ullah | Data Analyst">
<meta name="twitter:image" content="https://YOUR_USERNAME.github.io/samiullah-portfolio/assets/images/preview.png">
```

### Create a preview.png
- Size: 1200x630px (optimal for social sharing)
- Include your name, title, and a visual element
- Save to `assets/images/preview.png`

---

## 3. Adding Google Analytics (Optional)

Add this before `</head>` in `index.html`:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-YOUR_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-YOUR_TRACKING_ID');
</script>
```

Get your Tracking ID from [Google Analytics](https://analytics.google.com/).

---

## 4. Adding a Favicon

1. Create a favicon (32x32px or 180x180px PNG)
2. Save as `assets/favicon.ico` or `assets/favicon.png`
3. Add to `<head>`:
```html
<link rel="icon" type="image/png" href="assets/favicon.png">
<link rel="apple-touch-icon" href="assets/favicon.png">
```

---

## 5. Adding More Projects

Copy this template and paste after the last `.project-card`:

```html
<div class="project-card fade-in">
    <div class="project-image">
        <img src="assets/images/YOUR_PROJECT.png" alt="Project Name">
        <div class="project-overlay">
            <span class="project-category">Category Name</span>
        </div>
    </div>
    <div class="project-body">
        <h3>Project Title</h3>
        <p>Project description...</p>
        <div class="project-metrics">
            <div class="project-metric">
                <div class="project-metric-value">VALUE</div>
                <div class="project-metric-label">Label</div>
            </div>
            <!-- Add more metrics -->
        </div>
        <div class="project-tags">
            <span class="project-tag">Python</span>
            <span class="project-tag">SQL</span>
        </div>
        <div class="project-links">
            <a href="LIVE_DEMO_URL" class="project-link project-link-primary">
                <i class="fas fa-external-link-alt"></i> Live Demo
            </a>
            <a href="GITHUB_URL" class="project-link project-link-secondary">
                <i class="fab fa-github"></i> GitHub
            </a>
        </div>
    </div>
</div>
```

---

## 6. Customizing the Color Scheme

### Option A: Blue Theme (Default)
```css
--accent: #3b82f6;
--accent-light: #60a5fa;
--accent-dark: #1d4ed8;
--gradient-2: #8b5cf6;
```

### Option B: Green Theme
```css
--accent: #10b981;
--accent-light: #34d399;
--accent-dark: #059669;
--gradient-2: #06b6d4;
```

### Option C: Orange Theme
```css
--accent: #f97316;
--accent-light: #fb923c;
--accent-dark: #ea580c;
--gradient-2: #eab308;
```

Replace these values in the `:root` CSS variables.

---

## 7. Pre-Launch Checklist

- [ ] Replace all placeholder images
- [ ] Update all social/profile links
- [ ] Configure Formspree contact form
- [ ] Add Google Analytics (optional)
- [ ] Add favicon
- [ ] Test on mobile device
- [ ] Test all navigation links
- [ ] Verify contact form works
- [ ] Update GitHub repository description
- [ ] Add topics/tags to GitHub repo (data-analytics, portfolio, etc.)
- [ ] Share on LinkedIn with portfolio link
