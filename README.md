# Alex Lin - Personal Website

A minimalist personal website built with Jekyll and deployed on GitHub Pages.

## About

This is my personal website showcasing who I am, my vision, beliefs, and the work I'm doing at Axiom Asia and Edgera Partners.

## Tech Stack

- **Jekyll** - Static site generator
- **GitHub Pages** - Hosting and deployment
- **Markdown** - Content management

## Local Development

### Prerequisites

- Ruby (version 2.5 or higher)
- RubyGems
- GCC and Make

### Setup

1. Install Jekyll and Bundler:
```bash
gem install jekyll bundler
```

2. Create a Gemfile in the project root:
```ruby
source "https://rubygems.org"
gem "jekyll", "~> 4.3"
gem "jekyll-feed", "~> 0.12"
```

3. Install dependencies:
```bash
bundle install
```

4. Run the development server:
```bash
bundle exec jekyll serve
```

5. Visit `http://localhost:4000` in your browser

## Editing Content

All content is stored in markdown files in the `_content/` directory:

- `_content/about.md` - About Me section
- `_content/vision.md` - Vision & Beliefs section
- `_content/work.md` - Work & Projects section
- `_content/contact.md` - Contact information

Simply edit these files and push to GitHub - the site will automatically rebuild and deploy.

## Deployment

This site is configured for GitHub Pages deployment:

1. Push your changes to the `main` branch
2. Go to repository Settings > Pages
3. Set Source to "Deploy from a branch"
4. Select branch: `main`, folder: `/ (root)`
5. Save and wait a few minutes for deployment

Your site will be available at: `https://[username].github.io/aboutme/`

## Customization

- **Colors**: Edit CSS variables in `assets/css/main.css` (lines 9-15)
- **Typography**: Modify font settings in `assets/css/main.css` (line 24)
- **Site info**: Update `_config.yml` with your details
- **Layout**: Modify `index.html` and `_layouts/default.html`

## Structure

```
aboutme/
├── _content/           # Markdown content files
├── _layouts/           # HTML templates
├── assets/
│   ├── css/           # Stylesheets
│   └── js/            # JavaScript files
├── _config.yml        # Jekyll configuration
├── index.html         # Main page
└── README.md          # This file
```

## License

All rights reserved.
