# Articles Directory

This directory contains all blog articles in Markdown format.

## Quick Start

### Adding a New Article

1. **Copy the template:**
   ```bash
   cp article-template.md my-new-article.md
   ```

2. **Edit the frontmatter** (the section between `---` at the top):
   - Set `title`: Your article title
   - Set `date`: Publication date (YYYY-MM-DD)
   - Set `excerpt`: Brief description (1-2 sentences)
   - Optionally add `category` and `tags`

3. **Write your content** in Markdown below the frontmatter

4. **Update the index** (optional but recommended):
   ```bash
   node generate-index.js
   ```

That's it! Your article will appear on the blog.

## File Structure

- `*.md` - Article markdown files
- `articles.json` - Auto-generated index (optional, can be regenerated)
- `article-template.md` - Template for new articles
- `generate-index.js` - Script to auto-generate articles.json
- `WRITING_GUIDE.md` - Detailed writing guide
- `CONVERTING_TELEGRAPH.md` - Guide for converting Telegraph articles

## Frontmatter Format

```markdown
---
title: "Your Article Title"
date: "2025-01-15"
excerpt: "Brief description of your article"
category: "Technology"  # Optional
tags: "linux, tutorial"  # Optional, comma-separated
---
```

## Auto-Generating Index

The `generate-index.js` script automatically scans all `.md` files and creates `articles.json`:

```bash
node articles/generate-index.js
```

This is useful when:
- You add multiple articles at once
- You want to ensure articles.json is up to date
- You're setting up the blog for the first time

**Note:** The blog will work even without running this script - it will read frontmatter directly from markdown files. The script just makes the initial load faster.

## Best Practices

1. **File naming**: Use lowercase, hyphens, be descriptive
   - ✅ `linux-disk-partition-guide.md`
   - ❌ `article1.md` or `My Article.md`

2. **Always include frontmatter** with at least title, date, and excerpt

3. **Write clear excerpts** - these appear in article listings

4. **Use categories** to organize related articles

5. **Add relevant tags** for better discoverability

6. **Test locally** before pushing to GitHub

## Maintenance

- Articles are automatically sorted by date (newest first)
- The system is backward compatible - old articles without categories/tags still work
- You can add articles without updating articles.json - the system will read frontmatter directly
