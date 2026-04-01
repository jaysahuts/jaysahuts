# Jay Structure — Personal Website

Built with Jekyll, hosted on GitHub Pages.

## 🚀 Setup & Deployment

### 1. Create GitHub Repository
1. Go to [github.com](https://github.com) and create a new repo
2. Name it exactly: `yourusername.github.io` (replace with your GitHub username)
3. Set it to **Public**

### 2. Update Config
Open `_config.yml` and update:
```yaml
url: "https://yourusername.github.io"   # ← your GitHub username
social:
  youtube: https://youtube.com/@YourChannel
  podcast: https://open.spotify.com/show/yourshow
  linkedin: https://linkedin.com/in/yourprofile
```

### 3. Push to GitHub
```bash
git init
git add .
git commit -m "Initial site setup"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### 4. Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **(root)**
4. Save — your site will be live at `https://yourusername.github.io` in ~60 seconds

---

## ✍️ Writing Articles

Create a new file in `_posts/` with this naming format:

```
YYYY-MM-DD-your-article-title.md
```

### Article Template
```markdown
---
layout: post
title: "Your Article Title Here"
date: 2025-04-01
category: engineering        # engineering | scripture | architecture
tags: [tag1, tag2, tag3]
excerpt: "One sentence summary that shows on article cards."
---

Your article content starts here. Write in normal Markdown.

## Heading

Paragraph text...
```

### Categories
| Value | Colour | Channel |
|---|---|---|
| `engineering` | Amber | Construction & Engineering |
| `scripture` | Blue | Bible & Scripture |
| `architecture` | Teal | Architecture Marvels |

---

## 🔧 Local Development (Optional)

```bash
# Install Ruby & Bundler first
gem install bundler
bundle install
bundle exec jekyll serve
# → Open http://localhost:4000
```

---

## 📁 File Structure

```
├── _config.yml          # Site settings — update this first
├── _layouts/
│   ├── default.html     # Base template (header + footer)
│   └── post.html        # Article page template
├── _posts/              # ← Drop your articles here
├── assets/css/
│   └── main.css         # All styles
├── index.html           # Homepage
├── articles.html        # All articles with filter
├── about.md             # About page
└── Gemfile              # Ruby dependencies
```
