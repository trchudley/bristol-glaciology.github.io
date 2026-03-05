# Bristol Glaciology Centre Website

A Jekyll website powered by Minimal Mistakes theme, hosted on GitHub Pages.

Repo and tutorial website for Minimal Mistakes theme:

 - https://github.com/mmistakes/minimal-mistakes/
 - https://mmistakes.github.io/minimal-mistakes/

## Test website locally

1. **Install Ruby** (if not already installed)

2. **Install dependencies:**
   ```bash
   bundle install
   ```

3. **Run the site locally:**
   ```bash
   bundle exec jekyll serve
   ```

   Visit the indicated address (normally `http://localhost:4000`) in your browser.

## Adding Content

### New Pages
Create a new markdown file in the `_pages/` directory with frontmatter:
```markdown
---
title: Page Title
permalink: /page-url/
layout: single
---

Your content here.
```

### New News Posts
Create a new markdown file in the `_posts/` directory with the naming convention `YYYY-MM-DD-title.md`:
```markdown
---
title: "Post Title"
date: 2026-03-03
categories:
  - category-name
---

Your content here.
```

## Site Structure

- `_config.yml` - Site configuration
- `_pages/` - Main pages (Research, People, Publications, Join Us, News)
  - `resources/` - Resource sub-pages (Datasets, Software, Hardware, Group Notes)
- `_posts/` - News/blog posts
- `_people/` - Individual person files (faculty, postdocs, PhD students, MScR students)
- `_resources/` - Resource collection entries for grid display
- `_includes/` - Custom template includes (person-grid.html, resource-grid.html, footer.html)
- `index.md` - Homepage
- `assets/` - Images, CSS, and other assets

## Managing People

To add or remove people, create or delete files in `_people/`:
```markdown
---
title: "First Last"
last_name: "Last"
type: "faculty"  # or "postdoc", "phd", "mscr"
excerpt: "Job Title"
image: /assets/images/people/first-last.jpg
profile_url: "https://bristol.ac.uk/profile"
---
```

People are automatically sorted alphabetically by last name and grouped by type on the People page.

## Managing Resources

Resource pages are in `_pages/resources/` and displayed as a grid via the `_resources/` collection.

## Customization

To customize the site further:
- Edit `_config.yml` for site-wide settings
- Modify page frontmatter for individual page settings
- Add custom CSS in `assets/css/main.scss`

## More Information

- [Minimal Mistakes Documentation](https://mmistakes.github.io/minimal-mistakes/)
- [Jekyll Documentation](https://jekyllrb.com/)
