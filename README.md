# NeurOptim - Neuromorphic Optimization Research

Website repository for the NeurOptim research team at [neuroptim.org](https://neuroptim.org).

## About

This is the webpage for the research team dealing with projects related to neuromorphic optimization. The main idea is to centralize all the efforts from different collaborators in the field.

## Structure

This site uses [Jekyll](https://jekyllrb.com/) for easy customization and maintenance.

```
├── _config.yml          # Site configuration and settings
├── _layouts/            # Page templates
│   └── default.html     # Main layout template
├── _includes/           # Reusable components
│   ├── header.html      # Navigation header
│   ├── footer.html      # Page footer
│   ├── hero.html        # Hero section
│   └── research.html    # Research cards
├── _sass/               # Modular SCSS stylesheets
│   ├── _variables.scss  # Colors, fonts, breakpoints
│   ├── _base.scss       # Reset and typography
│   ├── _header.scss     # Navigation styles
│   ├── _hero.scss       # Hero section styles
│   ├── _about.scss      # About section styles
│   ├── _research.scss   # Research cards styles
│   ├── _collaborators.scss
│   ├── _footer.scss     # Footer styles
│   └── _responsive.scss # Media queries
├── assets/
│   └── css/
│       └── main.scss    # Main stylesheet (imports partials)
├── index.html           # Homepage content
├── Gemfile              # Ruby dependencies
└── CNAME                # Custom domain
```

## Customization

### Colors and Theme

Edit `_sass/_variables.scss` to change the color scheme:

```scss
$primary-color: #2c3e50;
$secondary-color: #3498db;
$accent-color: #e74c3c;
```

### Navigation

Edit `_config.yml` to modify navigation links:

```yaml
navigation:
  - title: About
    url: "#about"
  - title: Research
    url: "#research"
```

### Research Areas

Add or modify research areas in `_config.yml`:

```yaml
research_areas:
  - title: Your Research Area
    description: Description of your research focus.
```

### Adding New Pages

1. Create a new `.html` or `.md` file in the root directory
2. Add front matter at the top:

```yaml
---
layout: default
title: Page Title
---
```

3. Add your content below the front matter
4. Add a link in `_config.yml` navigation if needed

## Development

### Prerequisites

- Ruby (2.7 or higher)
- Bundler

### Local Setup

1. Install dependencies:
   ```bash
   bundle install
   ```

2. Run the development server:
   ```bash
   bundle exec jekyll serve
   ```

3. Open [http://localhost:4000](http://localhost:4000) in your browser.

The site will auto-rebuild when you make changes (except to `_config.yml`).

### GitHub Pages

This site is automatically built and deployed by GitHub Pages when changes are pushed to the main branch.

## Contributing

We welcome contributions from collaborators. Please feel free to submit issues or pull requests.

### Style Guidelines

- Keep content focused and accessible
- Test changes locally before submitting PRs
- Follow the existing code structure and naming conventions
