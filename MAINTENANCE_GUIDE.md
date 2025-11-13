# Website Maintenance Guide

This guide explains how to update different parts of your academic website.

## Quick Reference

| What to Update | File to Edit | Type |
|---------------|--------------|------|
| Homepage bio | `_pages/about.md` | Markdown |
| Contact info | `_config.yml` | YAML |
| Add new publication | `_publications/YYYY-MM-title.md` | Markdown |
| Add teaching experience | `_teaching/YYYY-semester-course.md` | Markdown |
| Update CV page | `_pages/cv.md` | Markdown |
| Navigation menu | `_data/navigation.yml` | YAML |
| Upload files (PDFs) | `files/` | Directory |

## Common Tasks

### 1. Add a New Publication

Create a new file in `_publications/` folder:

**File name format**: `YYYY-MM-DD-short-title.md`

**Template**:
```markdown
---
title: "Your Paper Title"
collection: publications
category: conferences  # or "manuscripts" for journals
permalink: /publication/YYYY-MM-short-title
excerpt: 'Brief description of the paper'
date: YYYY-MM-DD
venue: 'Conference/Journal Name'
paperurl: 'https://link-to-paper.com'
citation: 'Authors. (Year). "Title." <i>Venue</i>.'
---

Full abstract and details here...
```

### 2. Update Your Bio

Edit `_pages/about.md`:
- Write in Markdown
- Use `##` for section headers
- Use `**bold**` for emphasis
- Add links with `[text](url)`

### 3. Add a New Teaching Experience

Create a new file in `_teaching/` folder:

**Template**:
```markdown
---
title: "Course Number: Course Name"
collection: teaching
type: "Undergraduate course"  # or "Graduate course"
permalink: /teaching/YYYY-semester-course
venue: "University, Department"
date: YYYY-MM-DD
location: "City, State"
---

Course description and your responsibilities...
```

### 4. Update Profile Information

Edit `_config.yml`:
```yaml
author:
  name: "Your Name"
  bio: "Your title/position"
  location: "City, State"
  email: "your@email.com"
  googlescholar: "https://scholar.google.com/..."
  github: "username"
```

### 5. Upload a New PDF

1. Add the PDF to the `files/` directory
2. Reference it in your pages: `/files/filename.pdf`
3. Example in CV: `[Download PDF](/files/your-cv.pdf)`

### 6. Update Navigation Menu

Edit `_data/navigation.yml`:
```yaml
main:
  - title: "Publications"
    url: /publications/
  - title: "CV"
    url: /cv/
```

## Markdown Basics

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*

[Link text](https://url.com)

- Bullet point
- Another bullet

1. Numbered list
2. Second item

> Blockquote
```

## Publication Categories

In `_config.yml`, publication categories are defined:
- `books`: For books
- `manuscripts`: For journal articles
- `conferences`: For conference papers

Use the category key in your publication front matter.

## Deploying Updates

### Method 1: Git Command Line
```bash
git add .
git commit -m "Description of changes"
git push origin master
```

### Method 2: GitHub Web Interface
1. Navigate to your repository on GitHub
2. Click on the file you want to edit
3. Click the pencil icon to edit
4. Make changes
5. Commit changes at the bottom

### After Pushing
- GitHub Pages automatically rebuilds (1-2 minutes)
- Check your site: https://flagzhao.github.io/FlagZhao

## Testing Locally (Optional)

If you want to preview changes before pushing:

```bash
# Install dependencies (first time only)
bundle install

# Serve the site locally
bundle exec jekyll serve

# View at: http://localhost:4000
```

**Note**: Changes to `_config.yml` require restarting the server.

## File Organization

```
FlagZhao/
├── _config.yml           # Main configuration
├── _data/
│   └── navigation.yml    # Menu items
├── _pages/
│   ├── about.md         # Homepage
│   ├── cv.md            # CV page
│   └── publications.html # Publications page
├── _publications/        # Individual publication files
├── _teaching/           # Individual teaching files
├── files/               # PDFs and downloads
└── images/              # Images (including profile photo)
```

## Tips

1. **Always test locally** before pushing major changes (optional but recommended)
2. **Commit frequently** with descriptive messages
3. **Keep markdown files** well-formatted for readability
4. **Use consistent naming** for files (YYYY-MM-DD-title.md)
5. **Update the CV PDF** in `files/` when you update `_pages/cv.md`
6. **Check for typos** - the site is public!

## Common Issues

### Site not updating after push?
- Wait 2-5 minutes for GitHub Pages to rebuild
- Check GitHub Actions tab for build errors
- Clear your browser cache

### Changes to _config.yml not showing?
- Restart local server if testing locally
- GitHub Pages needs full rebuild (may take longer)

### Images not showing?
- Check file path: `/images/filename.png`
- Ensure image is committed and pushed
- Check file name case-sensitivity

### Publication not appearing?
- Check front matter YAML syntax
- Ensure `collection: publications` is set
- Check date format: YYYY-MM-DD
- Verify file is in `_publications/` directory

## Resources

- [Academic Pages Documentation](https://github.com/academicpages/academicpages.github.io)
- [Markdown Guide](https://www.markdownguide.org/)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [YAML Syntax](https://yaml.org/spec/1.2/spec.html)

## Getting Help

1. Check the [Academic Pages Wiki](https://github.com/academicpages/academicpages.github.io/wiki)
2. Search [existing issues](https://github.com/academicpages/academicpages.github.io/issues)
3. Ask in [discussions](https://github.com/academicpages/academicpages.github.io/discussions)

---

**Last Updated**: November 13, 2025

