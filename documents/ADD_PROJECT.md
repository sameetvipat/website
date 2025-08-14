# Add a new project (Projects page)

Projects are rendered from `static/projects.html`.

## Steps

1. Open `static/projects.html`.
2. Inside the grid container (`<div class="section-gap projects-grid">`), copy an existing project card block and paste it below the last one.

### Example card to duplicate

```html
<article class="project-card">
  <h2 class="project-title">Project Name</h2>
  <p class="project-description">
    Short one‑sentence description of the project.
  </p>
  <div class="project-tags">
    <span class="project-tag">Tech 1</span>
    <span class="project-tag">Tech 2</span>
  </div>
  <div class="project-links">
    <a href="https://github.com/your/repo" class="project-link">View Source</a>
    <a href="https://example.com" class="project-link">Live Demo</a>
  </div>
</article>
```

3. Edit the title, description, tags, and links.
4. Save and refresh the browser (or run `hugo server -D`).

## Notes

- Styles for cards, titles, tags, and links live in `static/css/site.css`.
- The grid is responsive and controlled by the `.projects-grid` utility.
- You can omit the “Live Demo” link if it isn’t applicable.
