# Blog Workflow - Quick Reference

## Adding a New Blog Post

### Method 1: Quick Start (Recommended)

1. **Copy the template:**
   ```bash
   cp articles/article-template.md articles/my-article-name.md
   ```

2. **Edit the file:**
   - Update frontmatter (title, date, excerpt)
   - Write your content in Markdown
   - Save the file

3. **That's it!** The article will appear automatically.

### Method 2: With Auto-Indexing

After adding articles, optionally regenerate the index for faster loading:

```bash
node articles/generate-index.js
```

## File Structure

```
articles/
├── article-template.md      # Template for new articles
├── articles.json            # Auto-generated index (optional)
├── generate-index.js        # Script to generate index
├── WRITING_GUIDE.md         # Detailed writing guide
└── *.md                     # Your articles
```

## Frontmatter Template

```markdown
---
title: "Your Article Title"
date: "2025-01-15"
excerpt: "Brief description (1-2 sentences)"
category: "Technology"  # Optional
tags: "linux, tutorial"  # Optional, comma-separated
---
```

## Best Practices

1. ✅ Use descriptive filenames: `linux-disk-partition-guide.md`
2. ✅ Always include title, date, and excerpt in frontmatter
3. ✅ Write clear, concise excerpts
4. ✅ Use categories to organize articles
5. ✅ Add relevant tags for discoverability
6. ✅ Test locally before pushing

## Maintenance

- **No manual JSON editing needed** - the system reads frontmatter directly
- **Auto-sorting** - Articles sorted by date (newest first)
- **Backward compatible** - Works with or without articles.json
- **Scalable** - Handles hundreds of articles efficiently

## Troubleshooting

**Article not showing?**
- Check frontmatter format (must have `---` at start and end)
- Verify date format is YYYY-MM-DD
- Check browser console for errors

**Want to regenerate index?**
```bash
node articles/generate-index.js
```

**Need help?**
- See `articles/WRITING_GUIDE.md` for detailed guide
- See `articles/README.md` for more information

