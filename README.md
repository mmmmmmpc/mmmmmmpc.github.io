# Miguel Pérez Colino - Personal Website

This repository contains the source code for the personal website of Miguel Pérez Colino, a Technology Enthusiast and Open Source Advocate. The site is built using [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme.

## Getting Started

### Prerequisites

- Ruby
- Bundler

### Installation

To install the necessary dependencies, run:

```bash
bundle install
```

### Building and Previewing

To build the site and start a local development server, run:

```bash
bundle exec jekyll serve
```

The site will be accessible at `http://localhost:4000`.

Alternatively, if you only want to build the site without serving it:

```bash
bundle exec jekyll build
```

To preview the built site in the `_site` directory using a different server:

```bash
python3 -m http.server 8000 --directory _site
```

## Project Structure

- `_data/`: Configuration data for navigation, sidebar, etc.
- `_includes/`: Reusable HTML snippets used in layouts and pages.
- `_layouts/`: Page and post templates.
- `_pages/`: Main site pages (e.g., About, Projects).
- `_posts/`: Blog posts in Markdown format.
- `_sass/`: SCSS stylesheets.
- `assets/`: Images, JavaScript, and other static assets.
- `_config.yml`: Main Jekyll configuration file.

## License

This project is licensed under the [CC0 1.0 Universal](LICENSE) license.
