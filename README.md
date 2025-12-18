# Rescue Capital Fund Website

Professional website for Rescue Capital Fund - crisis management and restructuring advisory services.

## Features

- **Multilingual Support**: English, Polish, German (with language switcher)
- **Responsive Design**: Optimized for desktop, tablet, and mobile
- **Modern Aesthetics**: Dark theme with gold accents, elegant typography
- **Smooth Animations**: Scroll-triggered animations, hover effects
- **SEO Ready**: Semantic HTML, meta descriptions

## Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click "New repository"
3. Name it `rescuecapitalfund.github.io` (or any name)
4. Make it **Public**
5. Click "Create repository"

### Step 2: Upload Files

Upload these files to your repository:
- `index.html` - Main website file
- `CNAME` - Custom domain configuration

You can do this via:
- GitHub web interface (drag & drop)
- Git command line
- GitHub Desktop

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll to **Pages** section (left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**

### Step 4: Configure Custom Domain

#### In GitHub:
1. In **Settings > Pages**
2. Under "Custom domain", enter: `rescuecapitalfund.com`
3. Click **Save**
4. Check "Enforce HTTPS" (after DNS propagates)

#### In Your Domain Registrar (DNS Settings):

Add these DNS records:

**For apex domain (rescuecapitalfund.com):**

| Type | Name | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

**For www subdomain:**

| Type | Name | Value |
|------|------|-------|
| CNAME | www | your-username.github.io |

### Step 5: Wait for DNS Propagation

- DNS changes can take up to 48 hours (usually 15-30 minutes)
- GitHub will automatically provision SSL certificate
- Site will be available at: https://rescuecapitalfund.com

## Customization

### Editing Content

All text content is in `index.html`. Search for `data-lang` attributes to find translatable content:

```html
<span data-lang="en" class="active">English text</span>
<span data-lang="pl">Polish text</span>
<span data-lang="de">German text</span>
```

### Changing Colors

Edit CSS variables at the top of `index.html`:

```css
:root {
    --color-bg: #0a0c10;           /* Background */
    --color-accent: #c9a962;        /* Gold accent */
    --color-text: #e8e6e3;          /* Text color */
}
```

### Updating Contact Information

Search for `contact@rescuecapitalfund.com` and replace with your email.

Update location in the contact section:
```html
<p>Gdańsk, Poland</p>
```

### Adding Statistics

Update numbers in the "About" section stats.

## File Structure

```
rescuecapitalfund/
├── index.html      # Main website (HTML + CSS + JS)
├── CNAME           # Custom domain configuration
└── README.md       # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

© 2025 Rescue Capital Fund. All rights reserved.
