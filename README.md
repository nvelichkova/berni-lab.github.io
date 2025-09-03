# Neuroscience Lab Website Template

A clean, professional Jekyll website template for neuroscience research labs, inspired by the ALPN Lab design. Perfect for GitHub Pages hosting.

## Features

✅ **Responsive Design** - Looks great on desktop and mobile  
✅ **Clean Layout** - Professional, academic appearance  
✅ **Easy Content Management** - Simple markdown files  
✅ **Team Profiles** - Organized by lab roles  
✅ **Publications Page** - Formatted academic citations  
✅ **News/Updates** - Lab announcements and highlights  
✅ **Research Areas** - Showcase your lab's work  
✅ **SEO Optimized** - Better search engine visibility  
✅ **Social Media Integration** - Link to lab profiles  

## Quick Start

### 1. Create Your Repository
- Create a new repository named `yourusername.github.io` (or `your-lab-name.github.io`)
- Make it public for free GitHub Pages hosting

### 2. Upload Files
Copy all these files into your repository:
```
├── _config.yml
├── _layouts/
│   └── default.html
├── assets/css/
│   └── style.css
├── index.md
├── research.md
├── people.md
├── publications.md
├── news.md
├── contact.md
└── README.md
```

### 3. Enable GitHub Pages
- Go to your repository Settings → Pages
- Set Source to "Deploy from a branch"
- Select "main" branch and "/ (root)" folder
- Your site will be live at `https://yourusername.github.io`

## Customization Guide

### Essential Changes

**1. Edit `_config.yml`**
Replace all placeholder text:
```yaml
title: "Your Lab Name - Neuroscience Lab"
lab_name: "Your Neuroscience Lab"
pi_name: "Dr. Your Name"
institution: "Your University"
email: "lab@university.edu"
# ... etc
```

**2. Update Homepage (`index.md`)**
- Replace research description
- Add your lab members
- Update recent news items

**3. Customize People Page (`people.md`)**
- Add real team member information
- Include photos (upload to `images/people/` folder)
- Update roles and bios

**4. Add Publications (`publications.md`)**
- Replace with your actual papers
- Update author names (bold for lab members)
- Include DOI links and PDFs

**5. Update Research Page (`research.md`)**
- Describe your specific research areas
- Add current projects and methods
- Include funding information

**6. Modify Contact Page (`contact.md`)**
- Add real contact information
- Update directions and parking info
- Include specific application requirements

### Adding Content

**Add Team Member Photos:**
1. Create `images/people/` folder
2. Upload photos (recommended: 300x300px, jpg/png)
3. Update person cards in `people.md`:
```html
<div class="person-photo">
  <img src="{{ '/images/people/john-doe.jpg' | relative_url }}" alt="John Doe">
</div>
```

**Add Research Images:**
1. Create `images/research/` folder
2. Upload figures/diagrams
3. Include in markdown:
```markdown
![Research Figure]({{ '/images/research/figure1.png' | relative_url }})
```

**Update Colors and Fonts:**
Edit `assets/css/style.css` to match your university branding:
```css
/* Change primary colors */
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
}
```

### Advanced Features

**Add Google Analytics:**
Add to `_config.yml`:
```yaml
google_analytics: your-tracking-id
```

**Custom Domain:**
1. Add `CNAME` file with your domain
2. Update DNS settings
3. Enable HTTPS in repository settings

**Blog Posts:**
Create `_posts/` folder and add files like:
```
2024-01-15-welcome-new-member.md
```

## File Structure

```
├── _config.yml          # Site configuration
├── _layouts/            # Page templates
│   └── default.html
├── assets/css/          # Stylesheets
│   └── style.css
├── images/              # All images
│   ├── people/         # Team photos
│   ├── research/       # Research figures
│   └── news/           # News images
├── index.md             # Homepage
├── research.md          # Research areas
├── people.md            # Team members
├── publications.md      # Publications list
├── news.md             # Lab news
├── contact.md          # Contact info
└── README.md           # This file
```

## Maintenance Tips

### Regular Updates
- Add new publications as they're published
- Update team member information
- Post lab news and achievements
- Keep contact information current

### SEO Best Practices
- Use descriptive page titles
- Add meta descriptions
- Include alt text for images
- Link to external profiles (ORCID, Google Scholar)

### Performance
- Compress images before uploading
- Keep CSS and HTML clean
- Test on mobile devices regularly

## Support

### Common Issues

**Site not loading?**
- Check that repository is public
- Verify GitHub Pages is enabled
- Ensure `index.md` exists

**Styling looks broken?**
- Check that `assets/css/style.css` is in the right location
- Verify no syntax errors in CSS

**Navigation not working?**
- Check that all page files exist
- Verify navigation links in `_config.yml`

### Getting Help

1. **Jekyll Documentation**: https://jekyllrb.com/docs/
2. **GitHub Pages**: https://docs.github.com/en/pages
3. **Markdown Guide**: https://www.markdownguide.org/

## License

This template is free to use and modify for academic purposes. If you use this template, a link back to the original would be appreciated but is not required.

## Credits

Inspired by the clean design of the ALPN Lab website and built with Jekyll and GitHub Pages.

---

**Questions?** Open an issue in this repository or contact [your-email].

*Last updated: [Date]*
