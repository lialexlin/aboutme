# Claude Configuration

## User Profile
**Name:** Alex Lin
**Professional Roles:**
- Investment Analyst at Axiom Asia (private equity fund-of-funds)
- Founder & Managing Partner at Edgera Partners (programmatic holdco for Taiwan SME acquisitions)
- Beginner programmer learning development and architecture

## Project: Personal Website

### Overview
This is a personal website built with Jekyll and deployed on GitHub Pages. The site showcases Alex's professional background, vision, beliefs, and ongoing work.

### Design Philosophy
- **Minimalist aesthetic**: Clean, modern design using only white, gray, and black colors
- **Content-focused**: Simple single-page layout with smooth scrolling navigation
- **Easy maintenance**: All content in markdown files for simple editing
- **Responsive**: Mobile-friendly design that works on all devices

### Tech Stack
- **Jekyll**: Static site generator with native GitHub Pages support
- **Markdown**: All content stored in `.md` files in `_content/` directory
- **CSS**: Custom minimalist styling with CSS variables for easy customization
- **JavaScript**: Minimal animations (fade-in effects, smooth scrolling)

### File Structure
```
_content/          - Markdown content files (edit these to update site)
  ├── about.md     - About Me section
  ├── vision.md    - Vision & Beliefs section
  ├── work.md      - Work & Projects section
  └── contact.md   - Contact information

_layouts/          - HTML templates
  └── default.html - Base layout template

assets/
  ├── css/main.css - Minimalist styling
  └── js/main.js   - Fade-in animations and smooth scroll

_config.yml        - Site configuration
index.html         - Main single-page layout
```

### Workflow for Updates

1. **Update content**: Edit markdown files in `_content/` folder
2. **Test locally** (optional):
   ```bash
   bundle exec jekyll serve
   ```
3. **Deploy**: Push to GitHub - auto-deploys to GitHub Pages

### Customization Notes

**Color Scheme** (in `assets/css/main.css`):
- Background: `#ffffff` (white)
- Text: `#4a4a4a` (gray)
- Headings: `#1a1a1a` (near-black)
- Borders: `#e0e0e0` (light gray)
- Accent: `#2a2a2a` (dark gray)

**Typography**: System fonts for fast loading and native feel

**Animations**: Subtle fade-in on scroll, smooth navigation transitions

### Next Steps

1. Fill in content in the markdown files:
   - Update `_content/about.md` with your bio and background
   - Fill in `_content/vision.md` with your vision and beliefs
   - Complete `_content/work.md` with detailed project information
   - Add real contact links in `_content/contact.md`

2. Update site configuration in `_config.yml`:
   - Add your real email
   - Update description if needed

3. Set up GitHub Pages:
   - Initialize git repository: `git init`
   - Create GitHub repository (e.g., `aboutme`)
   - Push code to GitHub
   - Enable GitHub Pages in repository settings

4. Optional enhancements:
   - Add custom domain
   - Include profile photo
   - Add project screenshots
   - Integrate analytics (if desired)

## Code and Documentation Standards

### Code Quality Rules
- **NO EMOJIS in code**: Never use emoji characters in code (scripts, functions, variables, comments, print statements). Emojis often cause encoding errors, especially on Windows. Use plain text like [OK], [ERROR], [WARNING] instead.
- **Read before adding**: Before adding new code or documentation sections, ALWAYS read the entire existing file first to understand structure and find the appropriate location. Never just append new sections at the end - integrate them logically.
- **Minimal documentation**: Do NOT create standalone documentation files (like `summary.md`, `report.md`, etc.) unless absolutely necessary. Instead, update the project-level CLAUDE.md file with relevant information. Only create separate docs when:
  - User explicitly requests it
  - Documentation is large enough to warrant separation (>500 lines)
  - It's a formal deliverable (like conflict reports, extraction outputs)

## Technical Notes

### File System Navigation on Windows
When working with Windows paths in bash commands:
- **Use forward slashes**: `C:/Users/lilin/...` instead of backslashes
- **Use Unix commands**: `ls`, `grep` instead of Windows `dir`, `findstr`
- **Example**: `ls "C:/Users/lilin/Axiom Asia Private Capital Pte Ltd/Axiom Admin - Axiom IV/GP Data/" | grep -i LAPAM`
