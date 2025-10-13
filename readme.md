# Personal Academic Website

This is a GitHub Pages website mimicking the clean, professional style of academic websites. The design is responsive and optimized for showcasing research work, publications, and academic achievements.

## 📁 File Structure

```
/webpage/
├── index.html          # Main webpage file
├── styles.css          # Stylesheet with responsive design
├── avatar.jpg          # Your profile photo (add this)
├── figures/            # Publication figures/images
│   ├── paper1.png      # Figure for first publication
│   ├── paper2.png      # Figure for second publication
│   └── README.md       # Guidelines for publication figures
└── README.md          # This file
```

## 🎨 Customizing Your Website

### 1. Replace Placeholder Content

Edit `index.html` to add your personal information:

- **Profile Section**: Update name, title, and description
- **About**: Replace with your research interests and background
- **Publications**: Add your papers, conferences, and journals
- **Education**: Update with your degrees and institutions
- **Honors & Awards**: List your achievements
- **Contact**: Add your email, office, and social links

### 2. Add Your Profile Photo

- Add an image file named `avatar.jpg` to the folder
- Recommended size: 300x300 pixels or larger (square format works best)
- The CSS will automatically crop it to a circle

### 3. Styling Customizations

The website uses a clean, academic style with:
- **Font**: Inter (professional, readable)
- **Colors**: Neutral grays with blue accent links
- **Layout**: Centered, max-width container for readability
- **Responsive**: Works on desktop, tablet, and mobile

To customize colors, edit the CSS variables in `styles.css`:
```css
/* Main colors */
color: #333;           /* Text color */
background-color: #fff; /* Background */
color: #0066cc;        /* Link color */
```

## 🚀 Publishing to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Name it `[your-username].github.io` (replace with your GitHub username)
4. Make it **public**
5. Check "Add a README file"
6. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Web Interface (Easier)**
1. In your new repository, click "uploading an existing file"
2. Drag and drop all files from your `/webpage/` folder
3. Write a commit message like "Initial website setup"
4. Click "Commit changes"

**Option B: Command Line (Advanced)**
```bash
# Navigate to your webpage folder
cd /Users/fengyz/Documents/webpage

# Initialize git repository
git init

# Add GitHub repository as remote
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git

# Add all files
git add .

# Commit changes
git commit -m "Initial website setup"

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

Your website will be live at `https://[your-username].github.io` within a few minutes!

## 📝 Managing and Updating Content

### Adding Publications

To add a new publication, copy this template in `index.html`:

```html
<div class="publication">
    <div class="pub-figure">
        <img src="figures/your-paper-figure.png" alt="Your Paper Figure" class="pub-image">
    </div>
    <div class="pub-content">
        <div class="pub-title">Your Paper Title</div>
        <div class="pub-authors">
            <strong>Your Name</strong>, Co-author Name, Another Author.
        </div>
        <div class="pub-venue">
            <em>Conference/Journal Name</em>, Year.
        </div>
        <div class="pub-links">
            [<a href="paper-url">Paper</a>] [<a href="code-url">Code</a>] [<a href="slides-url">Slides</a>]
        </div>
    </div>
</div>
```

### Managing Publication Figures

1. **Add figure images** to the `/figures/` folder
2. **Recommended size**: 240x180 pixels (2:3 aspect ratio)
3. **Supported formats**: PNG, JPG, WebP
4. **Update the image path** in your publication's HTML:
   ```html
   <img src="figures/your-figure-name.png" alt="Descriptive Alt Text" class="pub-image">
   ```

**Figure Guidelines:**
- Use your paper's main figure, teaser, or architecture diagram
- Keep file sizes under 200KB for fast loading
- Ensure good contrast and readability at small sizes
- Use descriptive alt text for accessibility

### Making Updates

1. Edit the files locally
2. Upload changed files to GitHub (drag-and-drop or git push)
3. Changes will appear on your website within minutes

### Adding New Sections

You can add new sections like "Teaching", "Service", or "Talks":

```html
<section class="teaching">
    <h3>Teaching</h3>
    <div class="teaching-item">
        <strong>Course Name</strong> - Role, Institution, Year
    </div>
</section>
```

## 🎨 Design Features

Your website includes modern design elements inspired by top academic websites:

### Unified Link Colors
- All links use a consistent blue color (`#0066cc`)
- Smooth hover transitions for better user experience
- Easy to customize via CSS variables in `styles.css`

### Publication Layout with Figures
- Each publication displays with a figure on the left
- Responsive design: stacks vertically on mobile devices
- Automatic image sizing and cropping with rounded corners

### Easy Customization
- **CSS Variables**: Change colors site-wide by modifying variables in `styles.css`
- **Modular Structure**: Clear HTML templates for easy copying
- **Responsive Design**: Automatically adapts to all screen sizes

```css
/* Customize your color scheme */
:root {
    --primary-color: #1a1a1a;     /* Main text color */
    --secondary-color: #666;       /* Secondary text */
    --accent-color: #0066cc;       /* Link color */
    --border-color: #f0f0f0;       /* Border color */
}
```

## 🔧 Advanced Features

### Adding a Custom Domain

1. Buy a domain (e.g., `yourname.com`)
2. In your GitHub repository settings → Pages
3. Add your custom domain
4. Configure DNS with your domain provider

### Analytics

Add Google Analytics by inserting this before `</head>` in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### SEO Optimization

The website includes basic SEO optimization. To improve it further:

1. Add meta descriptions
2. Use semantic HTML
3. Optimize images
4. Add structured data for publications

## 📱 Mobile Responsiveness

The website is fully responsive and includes:
- **Flexible layouts** for different screen sizes
- **Publication layout**: Figures and content stack vertically on mobile
- **Optimized typography** scaling for readability
- **Touch-friendly** navigation and interactions
- **Fast loading** optimized for mobile networks
- **Image optimization**: Figures resize appropriately on all devices

## 🎯 Best Practices

1. **Keep it updated**: Regular updates show you're active
2. **Professional photos**: Use high-quality, professional images
3. **Clear writing**: Write clearly about your research
4. **Working links**: Regularly check that all links work
5. **Backup**: Keep local copies of your files

## 🆘 Troubleshooting

**Website not showing up?**
- Wait 10-15 minutes after initial setup
- Check GitHub Pages settings
- Ensure repository name is exactly `username.github.io`

**Styling looks broken?**
- Check that `styles.css` is in the same folder as `index.html`
- Clear your browser cache

**Images not loading?**
- Check file names match exactly (case-sensitive)
- Ensure images are in the same folder as `index.html`

---

Need help? Feel free to reach out or check GitHub's [Pages documentation](https://docs.github.com/en/pages).