# ABX Capital Partners Asset Management

Static microsite for ABX Capital Partners Asset Management division.

## Structure

```
abxcapitalpartnersam/
├── index.html              # Home page
├── strategy.html           # Strategy & approach
├── research.html           # Research & insights
├── about.html              # About & philosophy
├── contact.html            # Contact information
├── sitemap.xml             # SEO sitemap
├── robots.txt              # Search engine directives
└── assets/
    ├── css/
    │   └── styles.css      # Main stylesheet
    ├── js/
    │   └── main.js         # Minimal JS (year display)
    └── img/
        ├── hero-placeholder.jpg
        ├── data-visualization.jpg
        └── team-collaboration.jpg
```

## Deployment to Cloudflare Pages

### Option 1: Git Integration (Recommended)

1. Initialize git repo and push to GitHub/GitLab:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: ABX AM microsite"
   git remote add origin <your-repo-url>
   git push -u origin main
   ```

2. In Cloudflare Dashboard:
   - Go to **Pages** > **Create a project**
   - Connect your Git repository
   - Build settings:
     - **Build command:** (leave empty)
     - **Build output directory:** `/`
   - Deploy

3. Configure custom domain:
   - Add `abxcapitalpartnersam.com` in **Custom domains**
   - Update DNS as instructed by Cloudflare

### Option 2: Direct Upload

1. In Cloudflare Dashboard:
   - Go to **Pages** > **Create a project** > **Direct Upload**
   - Upload all files (can drag entire directory)

2. Configure custom domain as above

## SEO Optimization

- All pages include semantic HTML5 elements
- Meta descriptions on every page
- JSON-LD structured data on homepage
- Sitemap.xml for search engines
- Canonical URLs specified
- Mobile-responsive design

## Image Placeholders

The three SVG placeholder images can be replaced with actual photos:
- `hero-placeholder.jpg` - Data/analytics theme
- `data-visualization.jpg` - Charts/quantitative analysis
- `team-collaboration.jpg` - Team/culture imagery

Keep aspect ratios consistent when replacing.

## Customization

- **Colors:** Edit CSS variables in `assets/css/styles.css` (`:root` section)
- **Content:** Update HTML files directly
- **Links:** All external links use `target="_blank" rel="noopener noreferrer"`
- **Footer year:** Automatically updates via `main.js`

## Performance

- No external dependencies
- Minimal CSS (~4KB)
- Minimal JS (~150 bytes)
- Static files only
- Fast load times on Cloudflare's edge network

## Browser Support

Modern browsers (Chrome, Firefox, Safari, Edge). Uses:
- CSS Grid
- CSS Custom Properties
- System font stack
- SVG images

