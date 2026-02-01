# Personal Website

A clean, minimal academic-style personal website for showcasing research, publications, and writing.

## Features

- Clean, readable design optimized for academic/professional content
- Responsive layout that works on all devices
- Five main sections: About, Publications, CV, Writing, Contact
- Blog post template for easy content creation
- No build process required - pure HTML/CSS
- Optimized for GitHub Pages hosting

## Setup Instructions

### 1. Initialize Git Repository

```bash
git init
git add .
git commit -m "Initial commit: Personal website"
```

### 2. Create GitHub Repository

1. Go to GitHub and create a new repository
2. Name it `yourusername.github.io` (replace `yourusername` with your GitHub username)
3. Don't initialize with README (you already have files)

### 3. Push to GitHub

```bash
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git branch -M main
git push -u origin main
```

### 4. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click Settings → Pages
3. Under "Source", select "main" branch
4. Click Save
5. Your site will be live at `https://yourusername.github.io` in a few minutes

## Customization Guide

### Update Your Information

1. **Replace "Your Name"** throughout all files with your actual name
2. **Update contact information** in `contact.html`
3. **Add your bio** in `index.html` (the hero section)
4. **List your research interests** in `index.html`

### Add Publications

Edit `publications.html`:
- Duplicate the `publication-item` div
- Update title, authors, venue, and links
- Add actual PDF links when available

### Update CV

Edit `cv.html`:
- Fill in your education details
- Add your professional experience
- Update skills section
- Add awards and service roles

### Create Blog Posts

1. Copy `posts/template.html` to a new file (e.g., `posts/my-first-post.html`)
2. Update the title, date, and content
3. Add a link to the new post in `writing.html`

Example:
```html
<li class="blog-item">
    <div class="blog-date">February 2026</div>
    <h2 class="blog-title">
        <a href="posts/my-first-post.html">My First Post</a>
    </h2>
    <p class="blog-excerpt">
        A brief description of the post...
    </p>
</li>
```

### Styling Customization

All styles are in `styles.css`. Key variables are at the top:

```css
:root {
    --text-primary: #1a1a1a;      /* Main text color */
    --accent: #2c5f7c;             /* Links and highlights */
    --serif: 'Crimson Pro', serif; /* Heading font */
    --sans: 'IBM Plex Sans', sans-serif; /* Body font */
}
```

Change these to customize the color scheme and typography.

## File Structure

```
.
├── index.html          # About page (home)
├── publications.html   # Research publications
├── cv.html            # Curriculum Vitae
├── writing.html       # Blog/writing index
├── contact.html       # Contact information
├── styles.css         # All styles
├── posts/             # Blog posts directory
│   └── template.html  # Blog post template
└── README.md          # This file
```

## Adding a Custom Domain (Optional)

1. Buy a domain name
2. In your GitHub repository, create a file named `CNAME` with your domain:
   ```
   yourdomain.com
   ```
3. Configure your domain's DNS settings to point to GitHub Pages
4. See [GitHub's custom domain documentation](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Maintenance Tips

- **Regular updates**: Keep your publications and CV current
- **Blog consistently**: If you're using the blog, aim for regular posts
- **Check links**: Periodically verify all external links work
- **Backup**: Keep local copies of your content
- **Analytics**: Consider adding Google Analytics to track visitors

## Technology Stack

- Pure HTML5 and CSS3
- Google Fonts (Crimson Pro, IBM Plex Sans)
- No JavaScript framework required
- No build process needed
- Works with any static hosting service

## License

This template is free to use and modify for your personal website.

## Support

For issues with GitHub Pages, see [GitHub Pages documentation](https://docs.github.com/en/pages).
