# Bristol Glaciology Centre Website

A Jekyll website powered by Minimal Mistakes theme, hosted on GitHub Pages.

Repo and tutorial website for Minimal Mistakes theme:

 - https://github.com/mmistakes/minimal-mistakes/
 - https://mmistakes.github.io/minimal-mistakes/

## Table of Contents

- [Bristol Glaciology Centre Website](#bristol-glaciology-centre-website)
  - [Table of Contents](#table-of-contents)
  - [Managing Content](#managing-content)
    - [Site Structure](#site-structure)
    - [Managing People](#managing-people)
    - [New Pages](#new-pages)
    - [New News Posts](#new-news-posts)
    - [Managing Resources](#managing-resources)
  - [Test website locally](#test-website-locally)
  - [Customization](#customization)
  - [More Information](#more-information)

## Managing Content

### Site Structure

- `_config.yml` - Site configuration
- `_pages/` - Main pages (Research, People, Publications, Join Us, News)
  - `resources/` - Resource sub-pages (Datasets, Software, Hardware, Group Notes)
- `_posts/` - News/blog posts
- `_people/` - Individual person files (faculty, postdocs, PhD students, MScR students)
- `_resources/` - Resource collection entries for grid display
- `_includes/` - Custom template includes (person-grid.html, resource-grid.html, footer.html)
- `index.md` - Homepage
- `assets/` - Images, CSS, and other assets

### Managing People

If you are not comfortable with GitHub, you can [open a new Issue on the GitHub repository](https://github.com/bristol-glaciology/bristol-glaciology.github.io/issues) and select 'Add Person to Website' as the template, which provides a handy form to act off of.

If you know what you are doing, it is possible to create or delete markdown files in `_people/`:

```markdown
---
title: "First Last"
last_name: "Last"
type: "faculty"  # or "postdoc", "phd", "mscr"
excerpt: "**Job Title**"
image: /assets/images/people/first-last.jpg
profile_url: "https://bristol.ac.uk/profile"
---
```

Notes:

 - These markdown files are by convention named in the format `firstname-lastname.md`.
 - Images also need to be added in the `/assets/images/people/` directory in the format `firstname-lastname.jpg`, and are recommended to be square aspect ratio, `jpg` format, and ideally between 400x400 and 800x800 pixels in size.
 - The default recommendation is for `profile_url` to link to your People page (for staff) and Pure page (for PGRs, who do not universally have a People page). However, you could also choose to link to your personal website etc. if desirable.

People are automatically sorted alphabetically by last name and grouped by type on the People page.


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

### Managing Resources

Resource pages are in `_pages/resources/` and displayed as a grid via the `_resources/` collection.

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

## Customization

To customize the site further:
- Edit `_config.yml` for site-wide settings
- Modify page frontmatter for individual page settings
- Add custom CSS in `assets/css/main.scss`

## More Information

- [Minimal Mistakes Documentation](https://mmistakes.github.io/minimal-mistakes/)
- [Jekyll Documentation](https://jekyllrb.com/)
