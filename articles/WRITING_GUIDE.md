# Writing Guide for Your Blog

## Quick Start: Adding a New Article

1. **Copy the template:**
   ```bash
   cp articles/article-template.md articles/my-new-article.md
   ```

2. **Edit the frontmatter** at the top of the file:
   ```markdown
   ---
   title: "Your Article Title"
   date: "2025-01-15"
   excerpt: "Brief description"
   category: "Technology"  # Optional
   tags: "linux, tutorial"  # Optional, comma-separated
   ---
   ```

3. **Write your content** in Markdown below the frontmatter

4. **Update the index** (if using the script):
   ```bash
   node articles/generate-index.js
   ```

That's it! Your article will appear automatically.

## Frontmatter Fields

- **title** (required): Article title
- **date** (required): Publication date in YYYY-MM-DD format
- **excerpt** (required): Short description (1-2 sentences)
- **category** (optional): Article category (e.g., "Technology", "Tutorial", "Personal")
- **tags** (optional): Comma-separated tags (e.g., "linux, ubuntu, guide")

## Markdown Tips

- Use `#` for main heading (will be removed if it matches title)
- Use `##` for section headings
- Use `**bold**` for emphasis
- Use code blocks with language: ` ```bash ` for bash, ` ```javascript ` for JS, etc.
- Use `> ` for blockquotes

## File Naming

- Use lowercase
- Use hyphens instead of spaces
- Be descriptive: `linux-disk-partition-guide.md`
- Keep it short but clear

## Best Practices

1. Always include frontmatter with title, date, and excerpt
2. Write clear, descriptive titles
3. Keep excerpts concise (1-2 sentences)
4. Use categories to organize related articles
5. Add relevant tags for better discoverability
6. Test your article locally before pushing




