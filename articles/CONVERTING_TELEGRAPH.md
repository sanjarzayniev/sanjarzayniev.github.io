# Converting Telegraph Articles to Markdown

This guide will help you convert your Telegraph articles to Markdown format for this website.

## Article Format

Each article should follow this structure:

```markdown
---
title: "Your Article Title"
date: "2025-01-15"
excerpt: "A brief description of your article (1-2 sentences)"
---

# Your Article Title

Your article content goes here in Markdown format.

## Section Heading

You can use standard Markdown syntax:
- **Bold text**
- *Italic text*
- Lists
- Code blocks
- Links
- Images
- And more!
```

## Steps to Convert

1. **Copy your Telegraph article content**
   - Open your Telegraph article
   - Copy all the text content

2. **Create a new markdown file**
   - Create a new file in the `articles` folder
   - Name it something descriptive, e.g., `my-article.md`
   - Use lowercase and hyphens for the filename

3. **Add frontmatter**
   - Add the frontmatter section at the top (between `---` lines)
   - Fill in: title, date (YYYY-MM-DD format), and excerpt

4. **Convert content to Markdown**
   - Convert headings: Use `#` for main heading, `##` for subheadings, etc.
   - Convert formatting: `**bold**`, `*italic*`, `` `code` ``
   - Convert lists: Use `-` for bullet points, `1.` for numbered lists
   - Convert links: `[link text](url)`
   - Convert code blocks: Use triple backticks with language name

5. **Update articles.json**
   - Open `articles/articles.json`
   - Add a new entry to the `articles` array with your article info

## Example Conversion

### Telegraph Format:
```
Title: My First Article
Date: January 15, 2025

This is my article about automation testing.

Key Points:
- Point 1
- Point 2
```

### Markdown Format:
```markdown
---
title: "My First Article"
date: "2025-01-15"
excerpt: "An article about automation testing"
---

# My First Article

This is my article about automation testing.

## Key Points

- Point 1
- Point 2
```

## Need Help?

If you have specific Telegraph articles you'd like help converting, share the content and I can help format them into Markdown!




