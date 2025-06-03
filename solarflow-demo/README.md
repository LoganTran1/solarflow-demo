# SolarFlow - Solar Marketing Flow Demo

A professional solar marketing website with hero landing page and multi-step qualification flow.

🌐 **Live Demo**: [https://logantran1.github.io/solarflow-demo](https://logantran1.github.io/solarflow-demo)

## 🚀 Features

### 🏠 **Hero Landing Page** (`landing.html`)
- Beautiful solar panel background with gradient overlay 
- Professional hero section with benefits
- ZIP code collection form
- Trusted user avatars with emoji people
- Redirects to qualification flow

### 📋 **6-Step Qualification Flow** (`index.html`)
1. **Homeowner/Renter** - Immediate engagement question
2. **Home Type** - Single family, townhome, condo, apartment
3. **Monthly Electric Bill** - Cost ranges for savings calculation
4. **Roof Sunlight** - Solar potential assessment
5. **Contact Information** - Compact form with satellite imagery
6. **Thank You** - with "You may also like" section + auto-redirect

### ✨ **Professional Design**
- Modern, clean interface
- Progress bar with percentage tracking
- Responsive design (mobile-friendly)
- Smooth animations and transitions
- Compact vertical spacing for better UX

## 🛠️ Setup for GitHub Pages

### Quick Deploy
1. **Fork/Clone** this repository
2. **Go to Settings** → Pages in your GitHub repo
3. **Select Source**: Deploy from a branch → `main` 
4. **Your site will be live** at: `https://[username].github.io/[repo-name]`

### Local Development
```bash
# Serve locally (Python)
python -m http.server 8000

# Or with Node.js
npx serve -s . -p 8000

# Then visit:
# http://localhost:8000/landing.html (Hero page)
# http://localhost:8000/index.html (Flow page)
```

## 📁 File Structure

```
solarflow-demo/
├── landing.html          # Hero landing page (default homepage)
├── index.html           # 6-step qualification flow
├── satellite-image-flow.png  # Satellite imagery for address step
├── README.md            # This file
├── DEPLOY.md           # Deployment instructions
└── server.js           # Local development server (optional)
```

## 🎯 User Journey

1. **Landing Page** → Users enter ZIP code and click "Check My Zip Code"
2. **Flow Begins** → Homeowner/Renter selection with back button to hero
3. **Qualification Steps** → Home type, electricity bill, roof sunlight
4. **Lead Capture** → Contact form with side-by-side name fields
5. **Thank You** → "You may also like" section + auto-redirect after 3 seconds

## 🎨 Customization

### Branding
```css
/* Update company name */
.logo { /* Change "SolarFlow" */ }

/* Update colors */
:root {
  --primary-green: #4CAF50;
  --hero-gradient: linear-gradient(135deg, rgba(70, 130, 180, 0.9), rgba(25, 25, 112, 0.9));
}
```

### Content
- **Pre-filled data**: Update form values in HTML
- **Final redirect URL**: Update `openLearnMore()` function in JavaScript
- **Satellite image**: Replace `satellite-image-flow.png`

### Flow Modifications
- **Steps**: Modify `totalSteps` variable (currently 6)
- **Validation**: Update `nextStep()` function
- **Progress**: Automatic calculation based on step count

## 📱 Mobile Responsive

- **Adaptive grid layouts** (4-column → 2-column on mobile)
- **Flexible form styling** 
- **Touch-friendly buttons**
- **Optimized spacing** for mobile screens

## 🔧 GitHub Pages Configuration

The site is configured to work perfectly with GitHub Pages:
- **No build process required** - pure HTML/CSS/JS
- **Relative paths** for all assets
- **Landing page** served as default homepage
- **Custom 404 handling** (optional)

## 📊 Analytics Integration

To add Google Analytics, insert before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🚀 Deployment Options

### GitHub Pages (Recommended)
- **Free hosting** with custom domain support
- **Automatic SSL** certificate
- **Global CDN** for fast loading

### Alternative Hosting
- **Netlify**: Drag & drop deployment
- **Vercel**: Git integration with preview deployments  
- **Surge.sh**: Simple command-line deployment

## 📈 Performance

- **Lightweight**: No external dependencies
- **Fast loading**: Optimized images and CSS
- **SEO friendly**: Semantic HTML structure
- **Accessible**: Proper contrast ratios and navigation

---

**Built for effective solar lead generation** 🌟

For questions or customization requests, please open an issue in this repository.
